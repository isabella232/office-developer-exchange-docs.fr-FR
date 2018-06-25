---
title: API REST Office 365 pour la messagerie, les calendriers et les contacts
manager: sethgros
ms.date: 4/29/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Découvrez des informations sur les API Office 365 que vous pouvez utiliser pour accéder aux messages, aux calendriers et aux contacts dans Office 365 ou Exchange Online.
ms.openlocfilehash: d42d3ff0b68dfbf23d5a4eebb826a6d39a4ac116
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755059"
---
# <a name="office-365-rest-apis-for-mail-calendars-and-contacts"></a><span data-ttu-id="503ab-103">API REST Office 365 pour la messagerie, les calendriers et les contacts</span><span class="sxs-lookup"><span data-stu-id="503ab-103">Office 365 REST APIs for mail, calendars, and contacts</span></span>

<span data-ttu-id="503ab-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez des informations sur les API Office 365 que vous pouvez utiliser pour accéder aux messages, aux calendriers et aux contacts dans Office 365 ou Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="503ab-104">Find information about the Office 365 APIs that you can use to access mail, calendars, and contacts in Office 365 or Exchange Online.</span></span>
  
<span data-ttu-id="503ab-p101">Office 365 et Exchange Online proposent une nouvelle façon de travailler avec la messagerie, les calendriers et contacts. Les API REST Courrier, Calendrier et Contact constituent un moyen puissant et facile à utiliser d'accéder aux données Exchange et de les manipuler. Ces API sont basées sur des normes ouvertes : OAuth version 2.0 pour l'authentification, OData version 4.0 et JSON pour l'abstraction des données. Elles offrent les avantages suivants :</span><span class="sxs-lookup"><span data-stu-id="503ab-p101">Office 365 and Exchange Online provide a new way to work with email, calendars, and contacts. The Mail, Calendar, and Contact REST APIs provide a powerful, easy-to-use way to access and manipulate Exchange data. These APIs are based on open standards: OAuth version 2.0 for authentication, and OData version 4.0 and JSON for data abstraction. This provides the following advantages:</span></span>
  
- <span data-ttu-id="503ab-109">Comme ces API exigent OAuth pour l'authentification, votre application n'a pas à gérer ou stocker les informations d'identification de l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="503ab-109">Because these APIs require OAuth for authentication, your application does not have to handle or store user credentials.</span></span>
    
- <span data-ttu-id="503ab-p102">OAuth permet de demander des autorisations fortement étendues aux données utilisateur. Par exemple, vous pouvez concevoir votre application afin de demander l'autorisation et la lecture seule du calendrier d'un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="503ab-p102">OAuth makes it possible to request tightly scoped permissions to user data. For example, you might design your application to request permission and read only a user's calendar.</span></span>
    
## <a name="work-with-email-and-mail-folders"></a><span data-ttu-id="503ab-112">Travailler avec le courrier et les dossiers de messagerie</span><span class="sxs-lookup"><span data-stu-id="503ab-112">Work with email and mail folders</span></span>

<span data-ttu-id="503ab-p103">Vous pouvez utiliser l'[API Courrier](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) pour obtenir, créer, mettre à jour, supprimer, déplacer, copier et envoyer des messages électroniques. Vous pouvez également obtenir, créer, mettre à jour et supprimer des dossiers de messagerie.</span><span class="sxs-lookup"><span data-stu-id="503ab-p103">You can use the [Mail API](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) to get, create, update, delete, move, copy, and send email. You can also get, create, update, and delete mail folders.</span></span> 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a><span data-ttu-id="503ab-115">Travailler avec des événements, des calendriers et des groupes de calendriers</span><span class="sxs-lookup"><span data-stu-id="503ab-115">Work with events, calendars, and calendar groups</span></span>

<span data-ttu-id="503ab-p104">Vous pouvez utiliser l'[API Calendrier](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) pour obtenir, créer, mettre à jour et supprimer des événements. Vous pouvez également obtenir, créer, mettre à jour et supprimer des calendriers et des groupes de calendriers.</span><span class="sxs-lookup"><span data-stu-id="503ab-p104">You can use the [Calendar API](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) to get, create, update, and delete events. You can also get, create, update, and delete calendar groups and calendars.</span></span> 
  
## <a name="work-with-contacts-and-contact-folders"></a><span data-ttu-id="503ab-118">Travailler avec les contacts et les dossiers de contacts</span><span class="sxs-lookup"><span data-stu-id="503ab-118">Work with contacts and contact folders</span></span>

<span data-ttu-id="503ab-p105">Vous pouvez utiliser l'[API Contacts](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) pour obtenir, créer, mettre à jour et supprimer des contacts dans la boîte aux lettres d'un utilisateur. Vous pouvez également obtenir les dossiers de contacts.</span><span class="sxs-lookup"><span data-stu-id="503ab-p105">You can use the [Contacts API](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) to get, create, update, and delete contacts in a user's mailbox. You can also get contact folders.</span></span> 
  
## <a name="work-with-file-providers"></a><span data-ttu-id="503ab-121">Utiliser des fournisseurs de fichier</span><span class="sxs-lookup"><span data-stu-id="503ab-121">Work with file providers</span></span>

<span data-ttu-id="503ab-122">Vous pouvez utiliser l'[API REST de fournisseurs de fichiers](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) pour obtenir, créer, mettre à jour et supprimer des informations sur les fournisseurs de fichiers pris en charge, tels que votre boîte aux lettres, Dropbox, etc.</span><span class="sxs-lookup"><span data-stu-id="503ab-122">You can use the [File Providers REST API](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) to get, create, update, and delete information about supported file providers, such as mailbox, Dropbox, and so on.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="503ab-123">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="503ab-123">Next steps</span></span>

<span data-ttu-id="503ab-p106">Accédez à la page [Développement sur la plateforme Office 365](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx) pour obtenir plus d'informations sur les API Courrier, Calendrier et Contacts, notamment des conseils pour la configuration de votre environnement et la prise en main des API. Veillez également à consulter les [projets de démarrage et exemples de codes](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx) pour voir ces API en action.</span><span class="sxs-lookup"><span data-stu-id="503ab-p106">Head over to the [Developing on the Office 365 platform](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx) page to get more information about the Mail, Calendar, and Contacts APIs, including guidance for setting up your environment and getting started with the APIs. Also be sure to check out the [starter projects and code samples](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx) to see these APIs in action.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="503ab-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="503ab-126">See also</span></span>


- [<span data-ttu-id="503ab-127">Développement sur la plateforme Office 365</span><span class="sxs-lookup"><span data-stu-id="503ab-127">Developing on the Office 365 platform</span></span>](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx)
    
- [<span data-ttu-id="503ab-128">Création d'une application ASP.NET MVC Office 365</span><span class="sxs-lookup"><span data-stu-id="503ab-128">Building an Office 365 ASP.NET MVC app</span></span>](http://msdn.microsoft.com/office/office365/howto/Build-your-first-ASPNET-MVC-app%28Office.15%29.aspx)
    
- [<span data-ttu-id="503ab-129">Opérations REST de messagerie</span><span class="sxs-lookup"><span data-stu-id="503ab-129">Mail REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="503ab-130">Opérations REST de calendrier</span><span class="sxs-lookup"><span data-stu-id="503ab-130">Calendar REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="503ab-131">Opérations REST de contacts</span><span class="sxs-lookup"><span data-stu-id="503ab-131">Contacts REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="503ab-132">Projets de démarrage et exemples de codes des API Office 365</span><span class="sxs-lookup"><span data-stu-id="503ab-132">Office 365 APIs starter projects and code samples</span></span>](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx)
    

