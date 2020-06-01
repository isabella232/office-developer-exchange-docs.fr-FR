---
title: Commencer à utiliser les services web dans Exchange
manager: sethgros
ms.date: 2/26/2019
ms.audience: Developer
ms.assetid: e1b07a92-0595-4bf1-bd6b-c07e66a8c923
description: Voici des ressources qui vous aideront à prendre en main EWS et d’autres services web dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 5980e22599585aa376890a414e0e8e7c7c5c707a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463754"
---
# <a name="start-using-web-services-in-exchange"></a>Commencer à utiliser les services web dans Exchange

Voici des ressources qui vous aideront à prendre en main EWS et d’autres services web dans Exchange.
  
Les [services web dans Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) permettent d'accéder à des données de boîtes aux lettres stockées dans Exchange Online, Exchange Online dans Office 365 et les versions locales d'Exchange, à partir d'Exchange Server 2007 et vous permettent de créer des applications personnalisées que vous pouvez utiliser pour gérer ces informations en fonction des besoins de votre organisation. Même si les possibilités de création d'applications de service web et EWS sont quasiment illimitées, certains concepts fondamentaux s'appliquent à tous les types d'application. Cette section fournit des informations sur les concepts fondamentaux à connaître pour commencer à utiliser EWS et les autres services web dans Exchange. 
  
## <a name="build-your-knowledge"></a>Approfondir ses connaissances
<a name="bk_Knowledge"> </a>

Que vous utilisiez .NET Framework ou une autre plate-forme pour développer votre application de service web, vous devez comprendre certains concepts importants avant de commencer votre projet de développement. 
  
**Tableau 1. Concepts des services web**

|**Concept**|**Résumé**|
|:-----|:-----|
|[Architecture](ews-applications-and-the-exchange-architecture.md) <br/> |Découvrez comment fonctionnent les services EWS au sein de l’architecture Exchange et les protocoles qu’ils utilisent.  <br/> |
|[Types d'applications EWS](ews-application-types.md) <br/> |Découvrez les principaux types d’applications que vous pouvez créer à l’aide des services web Exchange dans Exchange.  <br/> |
|[Accès aux services EWS](controlling-client-application-access-to-ews-in-exchange.md) <br/> |Les administrateurs Exchange peuvent limiter l’accès aux services EWS globalement pour l’ensemble de l’organisation, pour des utilisateurs individuels et pour des applications individuelles. Découvrez le niveau d’accès qui vous convient.  <br/> |
|[Configuration](setting-up-your-ews-application.md) <br/> |Découvrez les tâches que vous devez effectuer pour créer des applications qui utilisent l’API managée EWS ou EWS pour communiquer avec Exchange.  <br/> |
|[Authentification](authentication-and-ews-in-exchange.md) <br/> |Découvrez les options d’authentification pour la connexion à Exchange Online et Exchange sur site.  <br/> |
|[Découverte automatique](autodiscover-for-exchange.md) <br/> |Découvrez l'ensemble des services que vous pouvez utiliser pour détecter le point de terminaison de l'URL où un compte d'utilisateur peut accéder à des informations via EWS.  <br/> |
|[Serveur de boîtes aux lettres](https://technet.microsoft.com/library/jj150491%28v=exchg.150%29.aspx) <br/> |Découvrez le référentiel principal des informations communiquées à un client EWS. EWS a accès à un ensemble limité d’informations stockées dans les services de domaine Active Directory (AD DS).  <br/> |
|[Applications de messagerie pour Outlook et EWS](mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Découvrez les applications de messagerie pour Outlook et leur fonctionnement avec EWS dans Exchange.  <br/> |
|[API REST Office 365 pour la messagerie, les calendriers et les contacts](office-365-rest-apis-for-mail-calendars-and-contacts.md) <br/> |Découvrez les API Office 365 que vous pouvez utiliser pour accéder à la messagerie, aux calendriers et aux contacts dans Exchange Online dans le cadre d'Office 365.  <br/> |
|[API managée EWS](get-started-with-ews-managed-api-client-applications.md) <br/> |Découvrez l’API cliente privilégiée pour les développeurs .NET Framework.  <br/> |
|[EWS](get-started-with-ews-client-applications.md) <br/> |Découvrez comment créer votre première application à l’aide des demandes et des réponses XML EWS.  <br/> |
|[Fonctionnalité EWS dans les versions de produit Exchange](ews-functionality-in-exchange-product-versions.md) <br/> |Découvrez les fonctionnalités EWS disponibles dans la version d'Exchange.  <br/> |
|[Suivi et résolution des problèmes](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) <br/> |Découvrez comment effectuer le suivi des demandes et des réponses EWS pour résoudre les erreurs dans votre application d’API managées EWS.  <br/> |
   
## <a name="create-your-first-application"></a>Créer sa première application
<a name="create"> </a>

Si vous êtes prêt à développer votre première application cliente .NET Framework ou EWS, voir [Prise en main des applications clientes d'API managée EWS](get-started-with-ews-managed-api-client-applications.md) ou [Prise en main des applications clientes EWS](get-started-with-ews-client-applications.md).
  
## <a name="get-code-samples"></a>Télécharger des exemples de code
<a name="samples"> </a>

Pour trouver des exemples de code et des exemples qui vous montrent comment utiliser EWS et d’autres services web dans Exchange, consultez les ressources suivantes :
  
- [Exemples de code Exchange](https://code.msdn.microsoft.com/exchange)
    
- [CodePlex](http://www.codeplex.com/)
    
- [Documentation sur l'API Exchange](develop-web-service-clients-for-exchange.md)
    
- [Forum de développement Exchange](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment)
    
De nombreux autres exemples sont disponibles dans des blogs, les sites de démonstration de code et les forums. Nous vous recommandons également de télécharger [EWSEditor](http://ewseditor.codeplex.com/). Ce projet implémente la plupart des fonctionnalités d'EWS ; vous y trouverez des exemples de toutes les fonctionnalités EWS principales.
  
Si vous n'êtes pas développeur .NET Framework, vous y trouverez un grand nombre de bibliothèques client pour le développement EWS à l'aide de Java, Python, PHP et d'autres langages. 
  
## <a name="ask-questions-and-solve-problems"></a>Poser des questions et résoudre les problèmes
<a name="questions"> </a>

Vous avez besoin d'aide et vous n'avez pas trouvé de réponse à vos questions ? Vous pouvez effectuer une recherche sur le [forum de développement Exchange](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) pour découvrir si une autre personne a rencontré et résolu le même problème que vous. Une communauté de contributeurs a répondu à des centaines de questions sur le développement Exchange. Vous y trouverez également des sites, forums et blogs tiers qui traitent du développement Exchange qui auront peut-être la solution que vous recherchez. 
  
Contactez le [support Microsoft](https://support.microsoft.com/) si vous avez besoin d'une assistance supplémentaire. L'équipe de support pour les développeurs Exchange est constituée de professionnels chevronnés qui pourront répondre à vos questions sur le développement Exchange. 
  
## <a name="see-also"></a>Voir aussi

- [Explorer l'API managée EWS, EWS et les services web dans Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md) 
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md) 
- [Référence des services web pour Exchange](../web-service-reference/web-services-reference-for-exchange.md)
    

