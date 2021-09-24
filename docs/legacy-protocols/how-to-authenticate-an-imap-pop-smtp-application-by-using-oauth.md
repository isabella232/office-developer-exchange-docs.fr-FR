---
title: Authentifier une connexion IMAP, POP ou SMTP à l’aide d’OAuth
description: Découvrez comment utiliser l’authentification OAuth avec vos applications IMAP, POP et SMTP.
author: svpsiva
ms.date: 07/08/2021
ms.audience: Developer
ms.openlocfilehash: cfc9de18a53ce4cfdd8535f26fe3b04aab9cde55
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531322"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a>Authentifier une connexion IMAP, POP ou SMTP à l’aide d’OAuth

Découvrez comment utiliser l’authentification OAuth pour vous connecter aux protocoles IMAP, POP ou SMTP et accéder aux données de messagerie pour Office 365 utilisateurs.

> La prise en charge OAuth2 des protocoles IMAP, POP et SMTP comme décrit ci-dessous est prise en charge pour les utilisateurs Microsoft 365 (qui inclut Office sur le Web) et Outlook.com.

Si vous n’êtes pas familiarisé avec le protocole OAuth 2.0, commencez par lire le protocole [OAuth 2.0 sur Plateforme d'identités Microsoft vue d’ensemble.](/azure/active-directory/develop/active-directory-v2-protocols) Pour en savoir plus sur les bibliothèques d’authentification Microsoft (MSAL), qui implémentent le protocole OAuth 2.0 pour authentifier les utilisateurs et accéder aux API sécurisées, lisez la vue d’ensemble de [MSAL.](/azure/active-directory/develop/msal-overview)

Vous pouvez utiliser le service d’authentification OAuth fourni par Azure Active Directory pour permettre à votre application de se connecter aux protocoles IMAP, POP ou SMTP pour accéder aux Exchange Online dans Office 365. Pour utiliser OAuth avec votre application, vous devez :

1. [Inscrire votre application](#register-your-application) dans Azure Active Directory.
1. [Configurez votre application dans](#configure-your-application) Azure Active Directory.
1. [Obtenir un jeton d’accès](#get-an-access-token) à partir d’un serveur de jetons.
1. [Authentifier les demandes de connexion](#authenticate-connection-requests) à l’aide d’un jeton d’accès.

## <a name="register-your-application"></a>Inscription de votre application

Pour utiliser OAuth, une application doit être inscrite auprès de Azure Active Directory.

Suivez les instructions répertoriées dans Inscrire une application avec [le Plateforme d'identités Microsoft](/azure/active-directory/develop/quickstart-register-app) créer une application.

## <a name="get-an-access-token"></a>Obtenir un jeton d’accès

Vous pouvez utiliser l’une de [nos bibliothèques clientes MSAL](/azure/active-directory/develop/msal-overview) pour extraire un jeton d’accès de votre application cliente.

Vous pouvez également sélectionner un flux approprié dans la liste suivante et suivre les étapes correspondantes pour appeler les API REST de la plateforme d’identité sous-jacente et récupérer un jeton d’accès.

1. [Flux de code d’autorisation OAuth2](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [Flux d’octroi d’autorisation d’appareil OAuth2](/azure/active-directory/develop/v2-oauth2-device-code)

L’accès OAuth aux protocoles IMAP, POP, SMTP AUTH via le flux d’octroi d’informations d’identification du client OAuth2 n’est pas pris en charge. Si votre application a besoin d’un accès persistant à toutes les boîtes aux lettres d’une organisation Microsoft 365, nous vous recommandons d’utiliser les API Microsoft Graph qui autorisent l’accès sans utilisateur, activent des autorisations granulaires et permettent aux administrateurs d’accéder à un ensemble spécifique de boîtes aux lettres.

Veillez à spécifier les étendues complètes, y compris Outlook URL de ressources, lors de l’autorisation de votre application et de la demande d’un jeton d’accès.

| Protocole  | Chaîne d’étendue d’autorisation |
|-----------|-------------------------|
| IMAP      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| POP       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| SMTP AUTH | `https://outlook.office.com/SMTP.Send`             |

En outre, vous pouvez demander une [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) étendue. Lorsqu’un utilisateur approuve l’offline_access, votre application peut recevoir des jetons d’actualisation à partir Plateforme d'identités Microsoft point de terminaison du jeton. Les jetons d’actualisation ont une durée de vie longue. Votre application peut obtenir de nouveaux jetons d’accès à mesure que les anciens expirent.

## <a name="authenticate-connection-requests"></a>Authentifier les demandes de connexion

Vous pouvez initier une connexion à Office 365 serveurs de messagerie à l’aide des paramètres de messagerie [IMAP](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)et POP pour Office 365 .

### <a name="sasl-xoauth2"></a>SASL XOAUTH2

L’intégration d’OAuth nécessite que votre application utilise le format XOAUTH2 SASL pour le codage et la transmission du jeton d’accès. SASL XOAUTH2 code le nom d’utilisateur et le jeton d’accès ensemble au format suivant :

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

`^A`représente un **contrôle**  +  **A** ( `%x01` ).

Par exemple, le format SASL XOAUTH2 à accéder avec `test@contoso.onmicrosoft.com` un jeton d’accès `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` est :

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

Après le codage base64, cela se traduit par la chaîne suivante. Notez que des coupures de lignes sont insérées pour une plus bonne lisibilité.

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="sasl-xoauth2-authentication-for-shared-mailboxes-in-office-365"></a>Authentification SASL XOAUTH2 pour les boîtes aux lettres partagées dans Office 365

En cas d’accès aux boîtes aux lettres partagées à l’aide d’OAuth, l’application doit obtenir le jeton d’accès pour le compte d’un utilisateur, mais remplacer le champ userName dans la chaîne codée SASL XOAUTH2 par l’adresse e-mail de la boîte aux lettres partagée. 

### <a name="imap-protocol-exchange"></a>Protocole IMAP Exchange

Pour authentifier une connexion de serveur IMAP, le client devra répondre avec une `AUTHENTICATE` commande au format suivant :

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

Exemple d’échange de messages client-serveur qui se traduit par un succès d’authentification :

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

Exemple d’échange de messages client-serveur qui entraîne un échec d’authentification :

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a>Protocole POP Exchange

Pour authentifier une connexion de serveur POP, le client devra répondre avec une commande divisée en deux `AUTH` lignes au format suivant :    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

Exemple d’échange de messages client-serveur qui se traduit par un succès d’authentification :    

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

Exemple d’échange de messages client-serveur qui entraîne un échec d’authentification :    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a>Protocole SMTP Exchange

Pour authentifier une connexion de serveur SMTP, le client devra répondre avec une `AUTH` commande au format suivant :

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

Exemple d’échange de messages client-serveur qui se traduit par un succès d’authentification :

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

Exemple d’échange de messages client-serveur qui entraîne un échec d’authentification :

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
- [Paramètres de connexion IMAP, POP](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)
- [Protocole d’accès aux messages Internet](https://tools.ietf.org/html/rfc3501)
- [Protocole post-Office](https://tools.ietf.org/html/rfc1081)
- [Extension de service SMTP pour l’authentification](https://tools.ietf.org/html/rfc4954)
