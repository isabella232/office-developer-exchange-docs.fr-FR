---
title: Commencer à utiliser les services web dans Exchange
manager: sethgros
ms.date: 2/27/2017
ms.audience: Developer
localization_priority: Normal
ms.assetid: e1b07a92-0595-4bf1-bd6b-c07e66a8c923
description: Voici des ressources qui vous aideront à prendre en main EWS et d'autres services web dans Exchange.
ms.openlocfilehash: 2f203c5634c29105feb39220c3ebdd9624bb49ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755069"
---
# <a name="start-using-web-services-in-exchange"></a>Commencer à utiliser les services web dans Exchange

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Voici des ressources qui vous aideront à prendre en main EWS et d'autres services web dans Exchange.
  
Les [services web Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)fournissent l’accès aux données de boîtes aux lettres stockées dans Exchange Online, Exchange Online dans le cadre d’Office 365 et versions locales d’Exchange commençant par Exchange Server 2007 et vous permettent de créer des applications personnalisées que vous pouvez utiliser permet de gérer ces informations en fonction des exigences de votre organisation. Même si les possibilités de création d'applications de service web et EWS sont quasiment illimitées, certains concepts fondamentaux s'appliquent à tous les types d'application. Cette section fournit des informations sur les concepts fondamentaux à connaître pour commencer à utiliser EWS et les autres services web dans Exchange. 
  
## <a name="build-your-knowledge"></a>Approfondir ses connaissances
<a name="bk_Knowledge"> </a>

Que vous utilisiez .NET Framework ou une autre plate-forme pour développer votre application de service web, vous devez comprendre certains concepts importants avant de commencer votre projet de développement. 
  
**Tableau 1. Concepts des services web**

|**Concept**|**Résumé**|
|:-----|:-----|
|[Architecture](ews-applications-and-the-exchange-architecture.md) <br/> |Découvrez comment fonctionnent les services EWS au sein de l'architecture Exchange et les protocoles qu'ils utilisent.  <br/> |
|[Types d'applications EWS](ews-application-types.md) <br/> |Découvrez les principaux types d'applications que vous pouvez créer à l'aide des services web Exchange dans Exchange.  <br/> |
|[Accès aux services EWS](controlling-client-application-access-to-ews-in-exchange.md) <br/> |Les administrateurs Exchange peuvent limiter l'accès aux services EWS globalement pour l'ensemble de l'organisation, pour des utilisateurs individuels et pour des applications individuelles. Découvrez le niveau d'accès qui vous convient.  <br/> |
|[Configuration](setting-up-your-ews-application.md) <br/> |Découvrez les tâches que vous devez effectuer pour créer des applications qui utilisent l'API managée EWS ou EWS pour communiquer avec Exchange.  <br/> |
|[Authentification](authentication-and-ews-in-exchange.md) <br/> |Découvrez les options d'authentification pour la connexion à Exchange Online et Exchange sur site.  <br/> |
|[Découverte automatique](autodiscover-for-exchange.md) <br/> |Découvrez l'ensemble des services que vous pouvez utiliser pour détecter le point de terminaison de l'URL où un compte d'utilisateur peut accéder à des informations via EWS.  <br/> |
|[Serveur de boîtes aux lettres](http://technet.microsoft.com/en-us/library/jj150491%28v=exchg.150%29.aspx) <br/> |Découvrez le référentiel principal des informations communiquées à un client EWS. EWS a accès à un ensemble limité d'informations stockées dans les services de domaine Active Directory (AD DS).  <br/> |
|[Applications de messagerie pour Outlook et EWS](mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Découvrez les applications de messagerie pour Outlook et leur fonctionnement avec EWS dans Exchange.  <br/> |
|[API REST Office 365 pour la messagerie, les calendriers et les contacts](office-365-rest-apis-for-mail-calendars-and-contacts.md) <br/> |Découvrez les API Office 365 que vous pouvez utiliser pour accéder à la messagerie, aux calendriers et aux contacts dans Exchange Online dans le cadre d'Office 365.  <br/> |
|[API managée EWS](get-started-with-ews-managed-api-client-applications.md) <br/> |Découvrez l'API cliente privilégiée pour les développeurs .NET Framework.  <br/> |
|[EWS](get-started-with-ews-client-applications.md) <br/> |Découvrez comment créer votre première application à l'aide des demandes et des réponses XML EWS.  <br/> |
|[Fonctionnalité EWS dans les versions de produit Exchange](ews-functionality-in-exchange-product-versions.md) <br/> |Découvrez les fonctionnalités EWS disponibles dans la version d'Exchange.  <br/> |
|[Suivi et résolution des problèmes](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) <br/> |Découvrez comment effectuer le suivi des demandes et des réponses EWS pour résoudre les erreurs dans votre application d'API managées EWS.  <br/> |
   
## <a name="create-your-first-application"></a>Créer sa première application
<a name="create"> </a>

Si vous êtes prêt à développer votre première application cliente .NET Framework ou EWS, voir [Prise en main des applications clientes d'API managée EWS](get-started-with-ews-managed-api-client-applications.md) ou [Prise en main des applications clientes EWS](get-started-with-ews-client-applications.md).
  
## <a name="get-code-samples"></a>Télécharger des exemples de code
<a name="samples"> </a>

Pour trouver des exemples de code et des exemples qui vous montrent comment utiliser EWS et d'autres services web dans Exchange, consultez les ressources suivantes :
  
- [Exemples de code Exchange](http://code.msdn.microsoft.com/exchange)
    
- [CodePlex](http://www.codeplex.com/)
    
- [Documentation sur l'API Exchange](develop-web-service-clients-for-exchange.md)
    
- [Forum de développement Exchange](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment)
    
De nombreux autres exemples sont disponibles dans des blogs, les sites de démonstration de code et les forums. Nous vous recommandons également de télécharger [EWSEditor](http://ewseditor.codeplex.com/). Ce projet implémente la plupart des fonctionnalités d'EWS ; vous y trouverez des exemples de toutes les fonctionnalités EWS principales.
  
Si vous n'êtes pas développeur .NET Framework, vous y trouverez un grand nombre de bibliothèques client pour le développement EWS à l'aide de Java, Python, PHP et d'autres langages. 
  
## <a name="ask-questions-and-solve-problems"></a>Poser des questions et résoudre les problèmes
<a name="questions"> </a>

Besoin d’aide pour la réalisation des tâches et vous ne trouvez pas réponses ? Vous pouvez effectuer une recherche dans le [forum de développement Exchange](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) pour savoir si quelqu'un d'autre a rencontré et résolu le même problème. Une communauté de contributeurs a répondu à des centaines de questions sur le développement Exchange. Vous y trouverez également des sites, forums et blogs tiers qui traitent du développement Exchange qui auront peut-être la solution que vous recherchez. 
  
Contactez le [support Microsoft](https://support.microsoft.com/) si vous avez besoin d'une assistance supplémentaire. L'équipe de support pour les développeurs Exchange est constituée de professionnels chevronnés qui pourront répondre à vos questions sur le développement Exchange. 
  
## <a name="see-also"></a>Voir aussi

- [Explorer l'API managée EWS, EWS et les services web dans Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md) 
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md) 
- [Référence des services web pour Exchange](../web-service-reference/web-services-reference-for-exchange.md)
    

