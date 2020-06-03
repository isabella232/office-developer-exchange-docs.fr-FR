---
title: Fonctionnalité EWS dans les versions de produit Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 186c51dc-ec33-4a5d-b739-c9fcb1d4cdd3
description: EWS met en œuvre de nouvelles fonctionnalités dans les nouvelles versions du produit. Utilisez les informations contenues dans cet article pour déterminer si la version d’Exchange que vous ciblez inclut la prise en charge des données ou des fonctionnalités auxquelles vous avez besoin d’accéder.
ms.openlocfilehash: a8032e16cdd9100289666d8f2ce742fe054ede2e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456030"
---
# <a name="ews-functionality-in-exchange-product-versions"></a>Fonctionnalité EWS dans les versions de produit Exchange

EWS met en œuvre de nouvelles fonctionnalités dans les nouvelles versions du produit. Utilisez les informations contenues dans cet article pour déterminer si la version d’Exchange que vous ciblez inclut la prise en charge des données ou des fonctionnalités auxquelles vous avez besoin d’accéder. 
  
Le tableau suivant répertorie les versions d’Exchange qui incluent EWS et les principales fonctionnalités qui ont été introduites dans chaque version.
  
## <a name="ews-features-by-product-version"></a>Fonctionnalités EWS par version de produit

|**Version du produit**|**Composants**|
|:-----|:-----|
|Office 365 et Exchange Online |Inclut toutes les fonctionnalités de la version actuelle d’Exchange, ainsi que les nouvelles fonctionnalités ajoutées pour les clients en ligne.  |
|Exchange 2013 SP1 | Inclut toutes les fonctionnalités introduites dans Exchange 2013. Les fonctionnalités suivantes ont été introduites dans Exchange 2013 SP1 :<ul><li>Les confirmations de lecture peuvent désormais être suspendues pour les mises à jour et les suppressions.</li><li>Vous pouvez obtenir des informations d’approbation de [transport modéré](https://msdn.microsoft.com/library/43a89f71-8002-4cb0-b3c8-1c2b2597f227%28Office.15%29.aspx) .</li><li>Les réponses de vote peuvent être affichées.</li><li>La méthode [SetHoldOnMailboxes](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) et l’opération [SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) acceptent tous les paramètres d’un seul objet.</li><li>les recherches de découverte électronique peuvent spécifier une langue pour les requêtes de recherche et un format propre à la culture pour les plages de dates.</li><li>L’objet [méthode streamingsubscriptionconnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection%28v=exchg.80%29.aspx) peut désormais accéder aux objets [méthode streamingsubscription](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription%28v=exchg.80%29.aspx) .</li><li>Les conversations ont un paramètre pour indiquer si elles contiennent des messages électroniques protégés par IRM.</li><li>Les participants à la réunion peuvent proposer de nouvelles heures de début et de fin pour les réunions et les inclure dans leur réponse à la réunion.</li><li>La méthode [GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) de découverte automatique SOAP renvoie désormais le paramètre [GroupingInformation](https://msdn.microsoft.com/library/office/dn529149%28v=exchg.150%29.aspx) utilisé pour conserver l’affinité pour un abonnement aux événements avec plusieurs boîtes aux lettres.</li></ul> |
|Exchange 2013  | Inclut toutes les fonctionnalités introduites dans Exchange 2010 SP2. Les fonctionnalités suivantes ont été introduites dans Exchange 2013 :  <ul><li>  Archivage</li><li>eDiscovery</li><li>Personnages</li><li>Stratégies de rétention</li><li>Magasin de contacts unifié</li><li>Photos de l'utilisateur</li></ul> |
|Exchange 2010 SP2  | Inclut toutes les fonctionnalités introduites dans Exchange 2010 SP1. Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP2 :  <ul><li>  Obtenir l’expiration du mot de passe</li><li>DateTime, précision</li><li>Identificateurs de propriété mis à jour pour les contacts</li><li>Nouveaux scénarios d’usurpation d’identité</li></ul> |
|Exchange 2010 SP1  | Inclut toutes les fonctionnalités introduites dans Exchange 2010. Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP1 :  <ul><li>  Créer, récupérer et modifier des règles de boîte de réception</li><li>Accès par programme à la boîte aux lettres d’archivage</li><li>Actions de conversation</li><li>Notifications de traversée de pare-feu</li><li>Fonctionnalités d’administration améliorées</li><li>Prise en charge améliorée des versions mixtes</li><li>Prise en charge de la protection de la limitation</li><li>Contrôle de l’accès des applications à EWS</li><li>Prise en charge de l’authentification par certificat client</li></ul> |
|Exchange 2010  | Inclut toutes les fonctionnalités introduites dans Exchange 2007 SP1. Les fonctionnalités suivantes ont été introduites dans la version initiale d’Exchange 2010 : <ul> <li>  Liste de distribution privée complète</li><li>Objets de configuration utilisateur</li><li>Éléments associés aux dossiers</li><li>Suivi des messages</li><li>Messagerie unifiée</li><li>Découverte automatique SOAP  </li><li>Prise en charge améliorée des fuseaux horaires</li><li>Informations de disponibilité des ressources de la salle</li><li>Recherche indexée</li><li>Accès à la benne</li><li>Informations sur les infos-courrier</li></ul> |
|Exchange 2007 SP1  | Inclut toutes les fonctionnalités introduites dans Exchange 2007. Les fonctionnalités suivantes ont été introduites dans Exchange 2007 SP1 :  <ul><li>  Gestion des délégués</li><li>Autorisations d’accès aux dossiers</li><li>Dossiers publics</li><li>Publier des éléments</li><li>Conversion d’ID</li></ul> |
|Exchange 2007  | Les fonctionnalités suivantes ont été introduites dans la version initiale d’Exchange 2007 :  <ul><li>  Accès total aux éléments, aux dossiers et aux pièces jointes (créer, obtenir, mettre à jour, supprimer)</li><li>Disponibilité</li><li>Paramètres d’absence du Bureau</li><li>Notifications</li><li>Synchronisation</li><li>Résolution de noms</li><li>Expansion de liste de distribution (DL)</li><li>Rechercher</li></ul> |
   
## <a name="see-also"></a>Voir aussi

- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
- [Migration vers les technologies Exchange](../migrating-to-exchange-online-and-exchange-2013-technologies.md)
- [Explorer l'API managée EWS, EWS et les services web dans Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
    

