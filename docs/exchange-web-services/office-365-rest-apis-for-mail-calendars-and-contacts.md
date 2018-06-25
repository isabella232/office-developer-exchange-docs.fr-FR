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
# <a name="office-365-rest-apis-for-mail-calendars-and-contacts"></a>API REST Office 365 pour la messagerie, les calendriers et les contacts

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez des informations sur les API Office 365 que vous pouvez utiliser pour accéder aux messages, aux calendriers et aux contacts dans Office 365 ou Exchange Online.
  
Office 365 et Exchange Online proposent une nouvelle façon de travailler avec la messagerie, les calendriers et contacts. Les API REST Courrier, Calendrier et Contact constituent un moyen puissant et facile à utiliser d'accéder aux données Exchange et de les manipuler. Ces API sont basées sur des normes ouvertes : OAuth version 2.0 pour l'authentification, OData version 4.0 et JSON pour l'abstraction des données. Elles offrent les avantages suivants :
  
- Comme ces API exigent OAuth pour l'authentification, votre application n'a pas à gérer ou stocker les informations d'identification de l'utilisateur.
    
- OAuth permet de demander des autorisations fortement étendues aux données utilisateur. Par exemple, vous pouvez concevoir votre application afin de demander l'autorisation et la lecture seule du calendrier d'un utilisateur.
    
## <a name="work-with-email-and-mail-folders"></a>Travailler avec le courrier et les dossiers de messagerie

Vous pouvez utiliser l'[API Courrier](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) pour obtenir, créer, mettre à jour, supprimer, déplacer, copier et envoyer des messages électroniques. Vous pouvez également obtenir, créer, mettre à jour et supprimer des dossiers de messagerie. 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a>Travailler avec des événements, des calendriers et des groupes de calendriers

Vous pouvez utiliser l'[API Calendrier](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) pour obtenir, créer, mettre à jour et supprimer des événements. Vous pouvez également obtenir, créer, mettre à jour et supprimer des calendriers et des groupes de calendriers. 
  
## <a name="work-with-contacts-and-contact-folders"></a>Travailler avec les contacts et les dossiers de contacts

Vous pouvez utiliser l'[API Contacts](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) pour obtenir, créer, mettre à jour et supprimer des contacts dans la boîte aux lettres d'un utilisateur. Vous pouvez également obtenir les dossiers de contacts. 
  
## <a name="work-with-file-providers"></a>Utiliser des fournisseurs de fichier

Vous pouvez utiliser l'[API REST de fournisseurs de fichiers](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) pour obtenir, créer, mettre à jour et supprimer des informations sur les fournisseurs de fichiers pris en charge, tels que votre boîte aux lettres, Dropbox, etc. 
  
## <a name="next-steps"></a>Étapes suivantes

Accédez à la page [Développement sur la plateforme Office 365](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx) pour obtenir plus d'informations sur les API Courrier, Calendrier et Contacts, notamment des conseils pour la configuration de votre environnement et la prise en main des API. Veillez également à consulter les [projets de démarrage et exemples de codes](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx) pour voir ces API en action. 
  
## <a name="see-also"></a>Voir aussi


- [Développement sur la plateforme Office 365](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx)
    
- [Création d'une application ASP.NET MVC Office 365](http://msdn.microsoft.com/office/office365/howto/Build-your-first-ASPNET-MVC-app%28Office.15%29.aspx)
    
- [Opérations REST de messagerie](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx)
    
- [Opérations REST de calendrier](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx)
    
- [Opérations REST de contacts](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx)
    
- [Projets de démarrage et exemples de codes des API Office 365](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx)
    

