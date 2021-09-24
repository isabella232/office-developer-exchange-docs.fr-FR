---
title: Fonctionnalités EWS dans les versions de produit Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 186c51dc-ec33-4a5d-b739-c9fcb1d4cdd3
description: EWS implémente de nouvelles fonctionnalités dans les nouvelles version de produits. Utilisez les informations de cet article pour déterminer si la version de Exchange que vous ciblez inclut la prise en charge des données ou des fonctionnalités à qui vous avez besoin d’accéder.
ms.openlocfilehash: bccd0e84fc28f8a7366f0463e555cceec71aa181
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512281"
---
# <a name="ews-functionality-in-exchange-product-versions"></a>Fonctionnalités EWS dans les versions de produit Exchange

EWS implémente de nouvelles fonctionnalités dans les nouvelles version de produits. Utilisez les informations de cet article pour déterminer si la version de Exchange que vous ciblez inclut la prise en charge des données ou des fonctionnalités à qui vous avez besoin d’accéder. 
  
Le tableau suivant répertorie les versions Exchange qui incluent EWS et les principales fonctionnalités introduites dans chaque version.
  
## <a name="ews-features-by-product-version"></a>Fonctionnalités EWS par version de produit

|**Version du produit**|**Composants**|
|:-----|:-----|
|Office 365 et Exchange Online |Inclut toutes les fonctionnalités de la version actuelle de Exchange en plus des nouvelles fonctionnalités ajoutées pour les clients en ligne.  |
|Exchange 2013 SP1 | Inclut toutes les fonctionnalités introduites dans Exchange 2013. Les fonctionnalités suivantes ont été introduites dans Exchange 2013 SP1 :<ul><li>Les reçus de lecture peuvent maintenant être suspendus pour les mises à jour et suppressions.</li><li>Vous pouvez obtenir des [informations d’approbation de transport](https://msdn.microsoft.com/library/43a89f71-8002-4cb0-b3c8-1c2b2597f227%28Office.15%29.aspx) modérées.</li><li>Les réponses aux vote peuvent être vues.</li><li>La [méthode SetHoldOnMailboxes](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) et l’opération [SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) acceptent tous les paramètres d’un seul objet.</li><li>Les recherches de découverte électronique peuvent spécifier une langue pour les requêtes de recherche et un format spécifique à la culture pour les plages de dates.</li><li>[L’objet StreamingSubscriptionConnection peut](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection%28v=exchg.80%29.aspx) désormais accéder aux objets [StreamingSubscription.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription%28v=exchg.80%29.aspx)</li><li>Les conversations ont un paramètre pour indiquer si elles contiennent des messages électroniques protégés par IRM.</li><li>Les participants à la réunion peuvent proposer de nouvelles heures de début et de fin pour les réunions et les inclure dans leur réponse à la réunion.</li><li>La méthode [GETUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) de découverte automatique SOAP renvoie désormais le paramètre [GroupingInformation](https://msdn.microsoft.com/library/office/dn529149%28v=exchg.150%29.aspx) utilisé pour conserver l’affinité pour un abonnement à plusieurs événements de boîte aux lettres.</li></ul> |
|Exchange 2013  | Inclut toutes les fonctionnalités introduites dans Exchange 2010 SP2. Les fonctionnalités suivantes ont été introduites dans Exchange 2013 :  <ul><li>  Archivage</li><li>eDiscovery</li><li>Personas</li><li>Stratégies de rétention</li><li>Magasin de contacts unifié</li><li>Photos de l'utilisateur</li></ul> |
|Exchange 2010 SP2  | Inclut toutes les fonctionnalités introduites dans Exchange 2010 SP1. Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP2 :  <ul><li>  Obtenir l’expiration du mot de passe</li><li>Précision date/heure</li><li>Identificateurs de propriété mis à jour pour les contacts</li><li>Nouveaux scénarios d’emprunt d’identité</li></ul> |
|Exchange 2010 SP1  | Inclut toutes les fonctionnalités introduites dans Exchange 2010. Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP1 :  <ul><li>  Créer, récupérer et modifier des règles de boîte de réception</li><li>Accès par programme à la boîte aux lettres d’archivage</li><li>Actions de conversations</li><li>Notifications de traversée du pare-feu</li><li>Fonctionnalités d’administration améliorées</li><li>Prise en charge améliorée des versions mixtes</li><li>Prise en charge de la protection de limitation</li><li>Contrôle de l’accès des applications à EWS</li><li>Prise en charge de l’authentification par certificat client</li></ul> |
|Exchange 2010  | Inclut toutes les fonctionnalités introduites dans Exchange 2007 SP1. Les fonctionnalités suivantes ont été introduites dans la version initiale de Exchange 2010 : <ul> <li>  Liste de distribution privée complète</li><li>Objets de configuration utilisateur</li><li>Éléments associés au dossier</li><li>Suivi des messages</li><li>Messagerie unifiée</li><li>Découverte automatique SOAP  </li><li>Prise en charge améliorée du fuseau horaire</li><li>Informations sur la disponibilité des ressources de salle</li><li>Recherche indexée</li><li>Accès au benne</li><li>Informations sur les infos-courrier</li></ul> |
|Exchange 2007 SP1  | Inclut toutes les fonctionnalités introduites dans Exchange 2007. Les fonctionnalités suivantes ont été introduites dans Exchange 2007 SP1 :  <ul><li>  Déléguer la gestion</li><li>Autorisations d’accès aux dossiers</li><li>Dossiers publics</li><li>Publier des éléments</li><li>Conversion d’ID</li></ul> |
|Exchange 2007  | Les fonctionnalités suivantes ont été introduites dans la version initiale de Exchange 2007 :  <ul><li>  Accès total aux éléments, dossiers et pièces jointes (créer, obtenir, mettre à jour, supprimer)</li><li>Disponibilité</li><li>Paramètres de Office’utilisation</li><li>Notifications</li><li>Synchronisation</li><li>Résolution de noms</li><li>Développement d’une liste de distribution</li><li>Rechercher</li></ul> |
   
## <a name="see-also"></a>Voir aussi

- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
- [Migration vers les technologies Exchange](../migrating-to-exchange-online-and-exchange-2013-technologies.md)
- [Explorer l'API managée EWS, l’EWS et les services web dans Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
    

