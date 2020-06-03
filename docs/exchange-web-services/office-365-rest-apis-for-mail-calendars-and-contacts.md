---
title: API Outlook Microsoft Graph pour le courrier, les calendriers et les contacts
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Retrouvez des informations sur l’API Microsoft Graph que vous pouvez utiliser pour accéder aux messages, aux calendriers et aux contacts dans Office 365 ou Exchange Online.
localization_priority: Priority
ms.openlocfilehash: 7ca77596afb59ffab76001abd495de7328d2dd29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463866"
---
# <a name="microsoft-graph-rest-apis-for-mail-calendars-and-contacts"></a><span data-ttu-id="76e05-103">API REST Microsoft Graph pour la messagerie, les calendriers et les contacts</span><span class="sxs-lookup"><span data-stu-id="76e05-103">Microsoft Graph REST APIs for mail, calendars, and contacts</span></span>

<span data-ttu-id="76e05-104">Trouvez des informations sur les API Microsoft Graph que vous pouvez utiliser pour accéder à la messagerie, aux calendriers et aux contacts dans Office 365, Exchange Online ou Exchange Server dans des déploiements hybrides.</span><span class="sxs-lookup"><span data-stu-id="76e05-104">Find information about the Microsoft Graph APIs that you can use to access mail, calendars, and contacts in Office 365, Exchange Online, or Exchange Server in hybrid deployments.</span></span>

<span data-ttu-id="76e05-105">Office 365, Exchange Online et Exchange Server dans des déploiements hybrides offrent une nouvelle façon de travailler avec des courriers électroniques, des calendriers et des contacts.</span><span class="sxs-lookup"><span data-stu-id="76e05-105">Office 365, Exchange Online, and Exchange Server in hybrid deployments provide a new way to work with email, calendars, and contacts.</span></span> <span data-ttu-id="76e05-106">Les API REST Microsoft Graph Courrier, Calendrier et Contact sont des solutions puissantes et faciles d’utilisation pour accéder et manipuler les données Exchange.</span><span class="sxs-lookup"><span data-stu-id="76e05-106">The Microsoft Graph Mail, Calendar, and Contact REST APIs provide a powerful, easy-to-use way to access and manipulate Exchange data.</span></span> <span data-ttu-id="76e05-107">Ces API sont basées sur des normes ouvertes : OAuth version 2.0 pour l’authentification et OData version 4.0 et JSON pour l’abstraction de données.</span><span class="sxs-lookup"><span data-stu-id="76e05-107">These APIs are based on open standards: OAuth version 2.0 for authentication, and OData version 4.0 and JSON for data abstraction.</span></span> <span data-ttu-id="76e05-108">Elles offrent les avantages suivants :</span><span class="sxs-lookup"><span data-stu-id="76e05-108">This provides the following advantages:</span></span>

- <span data-ttu-id="76e05-109">Comme ces API exigent OAuth pour l'authentification, votre application n'a pas à gérer ou stocker les informations d'identification de l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="76e05-109">Because these APIs require OAuth for authentication, your application does not have to handle or store user credentials.</span></span>

- <span data-ttu-id="76e05-p102">OAuth permet de demander des autorisations fortement étendues aux données utilisateur. Par exemple, vous pouvez concevoir votre application afin de demander l’autorisation et la lecture seule du calendrier d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="76e05-p102">OAuth makes it possible to request tightly scoped permissions to user data. For example, you might design your application to request permission and read only a user's calendar.</span></span>

## <a name="work-with-email-and-mail-folders"></a><span data-ttu-id="76e05-112">Travailler avec le courrier et les dossiers de messagerie</span><span class="sxs-lookup"><span data-stu-id="76e05-112">Work with email and mail folders</span></span>

<span data-ttu-id="76e05-p103">Vous pouvez utiliser l'[API Courrier](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) pour obtenir, créer, mettre à jour, supprimer, déplacer, copier et envoyer des messages électroniques. Vous pouvez également obtenir, créer, mettre à jour et supprimer des dossiers de messagerie.</span><span class="sxs-lookup"><span data-stu-id="76e05-p103">You can use the [Mail API](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) to get, create, update, delete, move, copy, and send email. You can also get, create, update, and delete mail folders.</span></span> 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a><span data-ttu-id="76e05-115">Travailler avec des événements, des calendriers et des groupes de calendriers</span><span class="sxs-lookup"><span data-stu-id="76e05-115">Work with events, calendars, and calendar groups</span></span>

<span data-ttu-id="76e05-p104">Vous pouvez utiliser l'[API Calendrier](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) pour obtenir, créer, mettre à jour et supprimer des événements. Vous pouvez également obtenir, créer, mettre à jour et supprimer des calendriers et des groupes de calendriers.</span><span class="sxs-lookup"><span data-stu-id="76e05-p104">You can use the [Calendar API](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) to get, create, update, and delete events. You can also get, create, update, and delete calendar groups and calendars.</span></span> 
  
## <a name="work-with-contacts-and-contact-folders"></a><span data-ttu-id="76e05-118">Travailler avec les contacts et les dossiers de contacts</span><span class="sxs-lookup"><span data-stu-id="76e05-118">Work with contacts and contact folders</span></span>

<span data-ttu-id="76e05-p105">Vous pouvez utiliser l’[API Contacts](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) pour obtenir, créer, mettre à jour et supprimer des contacts dans la boîte aux lettres d’un utilisateur. Vous pouvez également obtenir les dossiers de contacts.</span><span class="sxs-lookup"><span data-stu-id="76e05-p105">You can use the [Contacts API](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) to get, create, update, and delete contacts in a user's mailbox. You can also get contact folders.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="76e05-121">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="76e05-121">Next steps</span></span>

<span data-ttu-id="76e05-122">Accédez à la page [Documentation Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/overview) pour obtenir plus d'informations sur les API Courrier, Calendrier et Contacts, notamment des conseils pour la configuration de votre environnement et la prise en main des API.</span><span class="sxs-lookup"><span data-stu-id="76e05-122">Head over to the [Microsoft Graph documentation](https://developer.microsoft.com/graph/docs/concepts/overview) page to get more information about the Mail, Calendar, and Contacts APIs, including guidance for setting up your environment and getting started with the APIs.</span></span> 

<span data-ttu-id="76e05-123">Pensez également à consulter la [prise en main rapide](https://developer.microsoft.com/graph/quick-start) et les [exemples de codes](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph) pour voir ces API en action.</span><span class="sxs-lookup"><span data-stu-id="76e05-123">Also be sure to check out the [quick starts](https://developer.microsoft.com/graph/quick-start) and [code samples](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph) to see these APIs in action.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="76e05-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="76e05-124">See also</span></span>

- [<span data-ttu-id="76e05-125">Documentation Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="76e05-125">Microsoft Graph documentation</span></span>](https://developer.microsoft.com/graph/docs/concepts/overview)   
- [<span data-ttu-id="76e05-126">Conditions requises locales pour l’API REST</span><span class="sxs-lookup"><span data-stu-id="76e05-126">On-premises requirements for the REST API</span></span>](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api)   

