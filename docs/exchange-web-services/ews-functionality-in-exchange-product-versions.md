---
title: Fonctionnalité EWS dans les versions de produit Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 186c51dc-ec33-4a5d-b739-c9fcb1d4cdd3
description: EWS implémente de nouvelles fonctionnalités dans les nouvelles versions du produit. Utilisez les informations de cet article pour déterminer si la version d’Exchange que vous ciblez prend en charge les données ou le besoin d’accéder à des fonctionnalités.
ms.openlocfilehash: 6b676781f25eeeb90fd9ab075fbe63198766bd99
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754773"
---
# <a name="ews-functionality-in-exchange-product-versions"></a>Fonctionnalité EWS dans les versions de produit Exchange

EWS implémente de nouvelles fonctionnalités dans les nouvelles versions du produit. Utilisez les informations de cet article pour déterminer si la version d’Exchange que vous ciblez prend en charge les données ou le besoin d’accéder à des fonctionnalités. 
  
Le tableau suivant répertorie les versions d’Exchange incluant les EWS et les principales fonctionnalités qui ont été introduites dans chaque version.
  
## <a name="ews-features-by-product-version"></a>Fonctionnalités EWS par version de produit

|**Version du produit**|**Fonctionnalités**|
|:-----|:-----|
|Office 365 et Exchange Online |Inclut toutes les fonctionnalités dans la version actuelle d’Exchange, en plus de ces nouvelles fonctionnalités sont ajoutées pour les clients en ligne.  |
|Exchange 2013 SP1 | Inclut toutes les fonctionnalités introduites dans Exchange 2013. Les fonctionnalités suivantes ont été introduites dans Exchange 2013 SP1 :<ul><li>Confirmations de lecture peuvent maintenant être suspendues pour les mises à jour et suppressions.</li><li>Vous pouvez obtenir des informations d’approbation [modérés transport](http://msdn.microsoft.com/library/43a89f71-8002-4cb0-b3c8-1c2b2597f227%28Office.15%29.aspx) .</li><li>Réponses de vote peut être affiché.</li><li>La méthode [SetHoldOnMailboxes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) et [SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) opération acceptent tous les paramètres dans un seul objet.</li><li>recherches de découverte électronique peuvent spécifier une langue pour les requêtes de recherche et un format spécifique à la culture pour les plages de dates.</li><li>L’objet [StreamingSubscriptionConnection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection%28v=exchg.80%29.aspx) permettre maintenant accéder les objets [StreamingSubscription](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscription%28v=exchg.80%29.aspx) .</li><li>Conversations ont un paramètre pour indiquer s’ils contiennent des messages électroniques qui sont protégés par IRM.</li><li>Les participants aux réunions, vous pouvez proposer de début et de fin des heures pour les réunions et les inclure dans leur réponse à une réunion.</li><li>La méthode SOAP Autodiscover [GetUserSettings](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) maintenant, renvoie le [GroupingInformation](http://msdn.microsoft.com/EN-US/library/office/dn529149%28v=exchg.150%29.aspx) qui est utilisé conserve les affinités pour un abonnement aux événements plusieurs boîtes aux lettres.</li></ul> |
|Exchange 2013  | Inclut toutes les fonctionnalités introduites dans Exchange 2010 SP2. Les fonctionnalités suivantes ont été introduites dans Exchange 2013 :  <ul><li>  L’archivage</li><li>eDiscovery</li><li>Personnage</li><li>Stratégies de rétention</li><li>Magasin de contacts unifié</li><li>Photos de l’utilisateur</li></ul> |
|Exchange 2010 SP2  | Inclut toutes les fonctionnalités introduites dans Exchange 2010 SP1. Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP2 :  <ul><li>  Obtenir l’Expiration du mot de passe</li><li>Précision DateTime</li><li>Identificateurs de propriété mis à jour pour les contacts</li><li>Nouveaux scénarios de l’emprunt d’identité</li></ul> |
|Exchange 2010 SP1  | Inclut toutes les fonctionnalités introduites dans Exchange 2010. Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP1 :  <ul><li>  Créer, récupérer et modifier des règles de boîte de réception</li><li>Accès par programme aux boîtes aux lettres d’Archive</li><li>Actions de conversations</li><li>Le parcours des notifications de pare-feu</li><li>Fonctionnalités d’administration améliorée</li><li>Amélioration de la prise en charge de la version mixte</li><li>Limitation de la prise en charge de la protection</li><li>Contrôle d’accès application EWS</li><li>Prise en charge de l’authentification de certificat client</li></ul> |
|Exchange 2010  | Inclut toutes les fonctionnalités introduites dans Exchange 2007 SP1. Les fonctionnalités suivantes ont été introduites dans la version initiale d’Exchange 2010 : <ul> <li>  Liste de Distribution privée complète</li><li>Objets de Configuration utilisateur</li><li>Dossier des éléments associés</li><li>Suivi des messages</li><li>Messagerie unifiée</li><li>Découverte automatique SOAP  </li><li>Prise en charge améliorée de fuseau horaire</li><li>Informations de disponibilité de ressources de salle</li><li>Recherche indexés</li><li>Accès benne</li><li>Partage des informations</li></ul> |
|Exchange 2007 SP1  | Inclut toutes les fonctionnalités introduites dans Exchange 2007. Les fonctionnalités suivantes ont été introduites dans Exchange 2007 SP1 :  <ul><li>  Gestion des délégués</li><li>Autorisations de dossier</li><li>Dossiers publics</li><li>Publier des éléments</li><li>Conversion de l’ID</li></ul> |
|Exchange 2007  | Les fonctionnalités suivantes ont été introduites dans la version initiale d’Exchange 2007 :  <ul><li>  Accès total aux éléments, dossiers et pièces jointes (créer, obtenir, mettre à jour, supprimer)</li><li>Disponibilité</li><li>En dehors des paramètres Office</li><li>Notifications</li><li>Synchronisation</li><li>Résolution de noms</li><li>Extension de la distribution (liste)</li><li>Search</li></ul> |
   
## <a name="see-also"></a>Voir aussi

- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
- [Migration et les technologies Exchange](../migrating-to-exchange-online-and-exchange-2013-technologies.md)
- [Explorer l'API managée EWS, EWS et les services web dans Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
    

