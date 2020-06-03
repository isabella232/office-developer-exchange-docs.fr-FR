---
title: Authentification et EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 9a83df96-aca0-42b3-b8f5-2b414f0363f1
description: Cette page contient des informations pour vous aider à choisir la norme d'authentification correcte pour votre application EWS qui cible Exchange.
localization_priority: Priority
ms.openlocfilehash: 69018b6f88fc80e1e18edd96ed0e16d52064572d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528481"
---
# <a name="authentication-and-ews-in-exchange"></a>Authentification et EWS dans Exchange

Cette page contient des informations pour vous aider à choisir la norme d’authentification correcte pour votre application EWS qui cible Exchange.
  
L'authentification est un élément clé de votre application EWS (Exchange Web Services). Exchange Online, Exchange Online en tant qu'application Office 365 et les versions locales d'Exchange en commençant par Exchange Server 2013 prennent en charge les protocoles d'authentification web standard pour vous aider à sécuriser les communications entre votre application et le serveur Exchange.
  
Si vous ciblez Exchange Online, la méthode d'authentification que vous choisissez doit utiliser HTTPS pour chiffrer les demandes et les réponses que votre application envoie. Bien que vous puissiez utiliser HTTP avec les serveurs Exchange locaux, nous vous recommandons d'utiliser HTTPS pour toute demande que votre application envoie à un point de terminaison EWS de façon à sécuriser convenablement les communications entre votre application et un serveur Exchange.
  
Exchange propose les options d'authentification suivantes : 
  
- OAuth 2.0 (Exchange Online uniquement)
    
- NTLM (Exchange en mode local uniquement)
    
- De base (déconseillé)
    
La méthode d'authentification que vous choisissez dépend des exigences de sécurité de votre organisation, selon que vous utilisez Exchange Online ou Exchange en mode local et que vous avez accès à un fournisseur tiers qui peut émettre des jetons OAuth. Cet article fournit des informations qui vous aideront à sélectionner la norme d'authentification qui convient le mieux à votre application.
  
## <a name="oauth-authentication"></a>Authentification OAuth

Il est recommandé que toutes les nouvelles applications utilisent la norme OAuth pour se connecter aux services Exchange Online. La supériorité de ce mécanisme sur l'authentification de base vaut bien le travail supplémentaire de mise en œuvre d'OAuth dans votre application. Pour information, toutefois, il existe également un certain nombre d'inconvénients que vous devez connaître.
  
**Tableau 1. Avantages et inconvénients de l'utilisation d'OAuth**

|**Avantages**|**Inconvénients**|
|:-----|:-----|
| OAuth est un protocole d'authentification standard.<br/><br/>L'authentification est gérée par un fournisseur tiers. Votre application ne collecte pas et ne stocke pas les informations d'identification Exchange.<br/><br/>Cette solution est plus confortable, car votre application reçoit uniquement un jeton opaque qui émane du fournisseur d'authentification. Par conséquent, une violation de la sécurité dans votre application exposerait uniquement le jeton, et non pas les informations d'identification Exchange de l'utilisateur.  <br/> | OAuth s'appuie sur un fournisseur d'authentification tiers. Cela peut impliquer des coûts supplémentaires à votre organisation ou vos clients.<br/><br/>La norme OAuth est plus difficile à mettre en œuvre que l'authentification de base.<br/><br/>Pour mettre en œuvre OAuth, vous devez intégrer votre application au fournisseur d'authentification et au serveur Exchange.  <br/> |
   
Pour minimiser les inconvénients, vous pouvez utiliser la [bibliothèque d'authentification Microsoft Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL) afin d'authentifier les utilisateurs aux services de domaine Active Directory (AD DS) dans le cloud ou localement et afin d'obtenir des jetons d'accès et de sécuriser les appels vers un serveur Exchange. Exchange Online requiert des jetons émis par le service Azure Active Directory, qui est pris en charge par la bibliothèque ADAL ; toutefois, vous pouvez utiliser n'importe quelle bibliothèque tierce. 
  
Pour en savoir plus sur l'utilisation de l'authentification OAuth dans votre application EWS, consultez les ressources suivantes :
  
- [Essai Office 365](https://docs.microsoft.com/office/developer-program/office-365-developer-program) pour configurer un serveur Exchange à utiliser pour tester votre application cliente.
    
- [Bibliothèque d'authentification Azure AD pour .NET](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)
    
- [Configurer Azure Active Directory](https://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx) pour permettre à votre application d’utiliser des jetons OAuth pour l’authentification.
    
- Consultez des exemples de code dans [Authentifier une application EWS à l'aide d'OAuth](how-to-authenticate-an-ews-application-by-using-oauth.md) pour étudier un exemple de programme. 
    
## <a name="ntlm-authentication"></a>Authentification NTLM

L'authentification NTLM est disponible uniquement pour les serveurs Exchange locaux. Pour les applications qui s'exécutent dans le pare-feu de l'entreprise, l'intégration entre l'authentification NTLM et .NET Framework fournit un moyen prédéfini d'authentifier votre application. 
  
**Tableau 2. Avantages et inconvénients de l'utilisation de l'authentification NTLM**

|**Avantages**|**Inconvénients**|
|:-----|:-----|
| Prêt à l'emploi avec votre serveur Exchange. Vous pouvez configurer l'accès aux services Exchange en utilisant une [applet de commande Exchange Management Shell](how-to-control-access-to-ews-in-exchange.md).  <br/><br/>Utilise l'objet .NET Framework [CredentialCache](https://msdn2.microsoft.com/library/615e0wsd) afin d'obtenir automatiquement les informations d'identification de l'utilisateur.<br/><br/>[exemples de code disponibles](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c) emploient les informations d'identification de l'utilisateur connecté pour l'authentifier auprès d'un serveur d'Exchange local.  <br/> | Les utilisateurs doivent être connectés à un domaine pour utiliser l'authentification NTLM.<br/><br/>Il peut être difficile d'accéder aux comptes de messagerie qui ne sont pas associés au compte de domaine de l'utilisateur.<br/><br/>Les applications de service doivent posséder un compte de domaine pour tirer parti de l’authentification NTLM.  <br/> |

   
## <a name="basic-authentication"></a>Authentification de base

L'authentification de base fournit un niveau de sécurité rudimentaire à votre application cliente. Nous recommandons que toutes les nouvelles applications utilisent NTLM ou le protocole OAuth pour l'authentification ; toutefois, l'authentification de base peut être le bon choix pour votre application dans certaines circonstances.
  
**Tableau 3. Avantages et inconvénients de l'utilisation de l'authentification de base**

|**Avantages**|**Inconvénients**|
|:-----|:-----|
| Prêt à l'emploi avec votre serveur Exchange. Vous pouvez configurer l'accès aux services Exchange en utilisant une [applet de commande Exchange Management Shell](how-to-control-access-to-ews-in-exchange.md).  <br/><br/>Les applications Windows peuvent utiliser les informations d'identification de l'utilisateur connecté par défaut.<br/><br/>Nombreux sont les [exemples de code](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c) qui illustrent la façon d'appeler EWS à l'aide de l'authentification de base.  <br/> | Nécessite que l'application collecte et stocke les informations d'identification de l'utilisateur.<br/><br/>Vous devez désactiver l’authentification NTLM si vous souhaitez forcer tous les utilisateurs à utiliser l’authentification de base.<br/><br/>En cas de violation de la sécurité dans votre application, ce mécanisme peut exposer l'adresse de messagerie et le mot de passe de l'utilisateur à un utilisateur malveillant.  <br/> |
   
Vous devez décider si l'authentification de base répond aux exigences de sécurité de votre organisation et des clients. L'authentification de base peut être judicieuse si vous souhaitez éviter les tâches de configuration fastidieuses, par exemple pour les applications de démonstration ou de test simples.
  
## <a name="see-also"></a>Voir aussi

- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)   
- [Ajouter une authentification à votre application web à l’aide de Microsoft Azure AD](https://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx)    
- [Contrôler l’accès à EWS dans Exchange](how-to-control-access-to-ews-in-exchange.md)    
- [Contrôler l’accès des applications clientes à EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md)   
- [Types de jetons et de revendications pris en charge](https://msdn.microsoft.com/library/9d35e4bc-7b72-49d1-b723-5464eee6be2c%28Office.15%29.aspx)
 