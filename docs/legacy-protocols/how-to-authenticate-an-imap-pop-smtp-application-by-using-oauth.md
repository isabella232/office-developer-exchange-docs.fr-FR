---
title: Authentification d’une connexion IMAP, POP ou SMTP à l’aide du protocole OAuth
description: Découvrez comment utiliser l’authentification OAuth avec vos applications IMAP, POP et SMTP.
author: svpsiva
ms.date: 02/19/2020
ms.audience: Developer
ms.openlocfilehash: f83a932790cde558e741ece1e87403103aff18fd
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012558"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a>Authentification d’une connexion IMAP, POP ou SMTP à l’aide du protocole OAuth

Découvrez comment utiliser l’authentification OAuth pour vous connecter à des protocoles IMAP, POP ou SMTP et accéder aux données de courrier électronique pour les utilisateurs d’Office 365.

> La prise en charge OAuth2 pour IMAP, POP, les protocoles SMTP, comme décrit ci-dessous, n’est pas prise en charge pour les utilisateurs de Outlook.com.

Si vous n’êtes pas familiarisé avec OAuth 2,0, lisez la [rubrique vue d’ensemble de la plateforme d’identité Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview). Ce document présente les différents composants de la plateforme d’identité Microsoft, y compris les kits de développement logiciel (SDK).

Vous pouvez utiliser le service d’authentification OAuth fourni par Azure Active Directory pour permettre à votre application de se connecter à des protocoles IMAP, POP ou SMTP pour accéder à Exchange Online dans Office 365. Pour utiliser OAuth avec votre application, vous devez :

1. [Enregistrez votre application](#register-your-application) auprès d’Azure Active Directory.
1. [Configurez votre application](#configure-your-application) dans Azure Active Directory.
1. [Obtenir un jeton d’accès](#get-an-access-token) à partir d’un serveur de jetons.
1. [Authentifier les demandes de connexion](#authenticate-connection-requests) avec un jeton d’accès.

## <a name="register-your-application"></a>Inscrire votre application

Pour utiliser OAuth, une application doit être inscrite auprès d’Azure Active Directory.

Suivez les instructions indiquées dans [enregistrer une application avec la plateforme d’identité Microsoft](/azure/active-directory/develop/quickstart-register-app) pour créer une application.

## <a name="configure-your-application"></a>Configurer votre application

Suivez les instructions indiquées dans la [configuration d’une application cliente pour accéder aux API Web](/azure/active-directory/develop/quickstart-configure-app-access-web-apis) .

Assurez-vous d’ajouter une ou plusieurs des étendues d’autorisation suivantes qui correspondent aux protocoles que vous souhaitez intégrer. Dans l’Assistant **Ajouter une autorisation** , sélectionnez **Microsoft Graph** , puis **autorisations déléguées** pour trouver les étendues d’autorisation suivantes.

| Protocole  | Étendue d’autorisation        |
|-----------|-------------------------|
| IMAP      | `IMAP.AccessAsUser.All` |
| POP       | `POP.AccessAsUser.All`  |
| AUTHENTIFICATION SMTP | `SMTP.Send`             |

## <a name="get-an-access-token"></a>Obtenir un jeton d’accès

Vous pouvez utiliser l’une de nos [bibliothèques clientes MSAL](/azure/active-directory/develop/msal-overview) pour récupérer un jeton d’accès à partir de votre application cliente.

Vous pouvez également sélectionner un flux approprié dans la liste suivante et suivre les étapes correspondantes pour appeler les API REST de la plateforme d’identité sous-jacente et récupérer un jeton d’accès.

1. [Flux de code d’autorisation OAuth2](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [Flux d’octroi d’autorisation d’appareil OAuth2](/azure/active-directory/develop/v2-oauth2-device-code)

L’accès OAuth aux protocoles IMAP, POP et SMTP AUTH via le flux d’octroi d’informations d’identification du client OAuth2 n’est pas pris en charge. Si votre application a besoin d’un accès permanent à toutes les boîtes aux lettres dans une organisation Microsoft 365, nous vous recommandons d’utiliser les API Microsoft Graph autorisant l’accès sans utilisateur, d’activer des autorisations granulaires et de permettre aux administrateurs d’étendre ce type d’accès à un ensemble spécifique de boîtes aux lettres.

Veillez à spécifier les étendues complètes, y compris les URL de ressource Outlook, lorsque vous autorisez votre application et que vous demandez un jeton d’accès.

| Protocole  | Chaîne d’étendue d’autorisation |
|-----------|-------------------------|
| IMAP      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| POP       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| AUTHENTIFICATION SMTP | `https://outlook.office.com/SMTP.Send`             |

En outre, vous pouvez demander une étendue [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) . Lorsqu’un utilisateur approuve l’étendue offline_access, votre application peut recevoir des jetons d’actualisation à partir du point de terminaison du jeton de plateforme d’identité Microsoft. Les jetons d’actualisation sont à durée de vie longue. Votre application peut obtenir de nouveaux jetons d’accès car les plus anciens arrivent à expiration.

## <a name="authenticate-connection-requests"></a>Authentifier les demandes de connexion

Vous pouvez établir une connexion aux serveurs de messagerie Office 365 à l’aide des [paramètres de messagerie IMAP et pop pour Office 365](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353).

### <a name="sasl-xoauth2"></a>XOAUTH2 SASL

L’intégration OAuth avec nécessite que votre application utilise le format SASL XOAUTH2 pour coder et transmettre le jeton d’accès. SASL XOAUTH2 encode le nom d’utilisateur, le jeton d’accès au format suivant :

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

`^A`représente un **contrôle**  +  **a** ( `%x01` ).

Par exemple, le format XOAUTH2 SASL pour accéder à un `test@contoso.onmicrosoft.com` jeton d’accès `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` est le suivant :

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

Après le codage Base64, cela traduit la chaîne suivante. Notez que les sauts de ligne sont insérés pour des raisons de lisibilité.

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="sasl-xoauth2-authentication-for-shared-mailboxes-in-office-365"></a>Authentification SASL XOAUTH2 pour les boîtes aux lettres partagées dans Office 365

Dans le cas d’un accès partagé aux boîtes aux lettres à l’aide d’OAuth, l’application doit obtenir le jeton d’accès au nom d’un utilisateur, mais remplacer le champ nom d’utilisateur dans la chaîne codée SASL XOAUTH2 par l’adresse e-mail de la boîte aux lettres partagée. 

### <a name="imap-protocol-exchange"></a>Échange de protocole IMAP

Pour authentifier une connexion de serveur IMAP, le client doit répondre par une `AUTHENTICATE` commande au format suivant :

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

Exemple d’échange de messages client-serveur entraînant une réussite de l’authentification :

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

Exemple d’échange de messages client-serveur entraînant un échec d’authentification :

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a>Échange de protocole POP

Pour authentifier une connexion de serveur POP, le client doit répondre par une `AUTH` commande divisée en deux lignes au format suivant :    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

Exemple d’échange de messages client-serveur entraînant une réussite de l’authentification :    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYX   
JlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0  
Q2cBAQ==    
S: +OK User successfully authenticated. 
[connection continues...]   
``` 

Exemple d’échange de messages client-serveur entraînant un échec d’authentification :    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a>Échange de protocole SMTP

Pour authentifier une connexion de serveur SMTP, le client doit répondre par une `AUTH` commande au format suivant :

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

Exemple d’échange de messages client-serveur entraînant une réussite de l’authentification :

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 235 2.7.0 Authentication successful
[connection continues...]
```

Exemple d’échange de messages client-serveur entraînant un échec d’authentification :

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 535 5.7.3 Authentication unsuccessful [SN2PR00CA0018.namprd00.prod.outlook.com]
```

## <a name="see-also"></a>Voir aussi

- [Authentification et EWS dans Exchange](../exchange-web-services/authentication-and-ews-in-exchange.md)
- [IMAP, paramètres de connexion POP](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)
- [Internet Message Access Protocol](https://tools.ietf.org/html/rfc3501)
- [Protocole post Office](https://tools.ietf.org/html/rfc1081)
- [Extension de service SMTP pour l’authentification](https://tools.ietf.org/html/rfc4954)
