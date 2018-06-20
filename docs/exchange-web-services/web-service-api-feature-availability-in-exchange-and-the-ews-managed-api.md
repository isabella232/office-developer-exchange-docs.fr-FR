---
title: Disponibilité des fonctionnalités Web service API dans Exchange et de l’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 07d3e6e8-d549-4ad7-baa4-bc531dfb7dd2
description: En savoir plus sur le service web et EWS fonctionnalités d’API sont disponibles dans chaque version d’Exchange et de l’API managée EWS.
ms.openlocfilehash: d19ab062c8d418e373e8268b1ab039e5436e71bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755076"
---
# <a name="web-service-api-feature-availability-in-exchange-and-the-ews-managed-api"></a>Disponibilité des fonctionnalités Web service API dans Exchange et de l’API managée EWS

En savoir plus sur le service web et EWS fonctionnalités d’API sont disponibles dans chaque version d’Exchange et de l’API managée EWS.
  
Applications clientes ciblent souvent plusieurs versions d’Exchange. Pour cette raison, vous pouvez souhaiter concevoir votre application de telle sorte que vous pouvez activer [les fonctionnalités de client EWS](ews-client-design-overview-for-exchange.md#EWSFeatures) et désactiver en fonction de la version d’Exchange qui héberge la boîte aux lettres de vos utilisateurs. Cet article fournit des informations sur les fonctionnalités de l’API service sont disponibles dans les différentes versions d’Exchange et de l’API managée EWS. Utilisez ces informations pour concevoir votre application s’applique globalement à clients exécutant plusieurs versions d’Exchange. 
  
Pour plus d’informations sur les différences entre les versions d’Exchange, consultez les fichiers de schéma EWS et la [documentation de référence](http://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx)associée.
  
## <a name="api-features-by-exchange-version"></a>Fonctionnalités de l’API à la version d’Exchange
<a name="bk_apifeatures"> </a>

Service web Exchange API, y compris EWS et découverte automatique, sont développées avec compatibilité des versions multiples à l’esprit. Par conséquent, une application qui cible Exchange 2007 fonctionne également avec les versions d’Exchange commençant par Exchange 2013, notamment Exchange Online et Exchange Online dans le cadre d’Office 365. 
  
Le tableau suivant indique les fonctionnalités d’API sont disponibles dans chaque version d’Exchange et les versions de l’API managée EWS depuis la version 2.0. Étant donné que votre application peut cibler plusieurs versions d’Exchange, il sera utile de savoir quelles versions prennent en charge les fonctionnalités qui implémente votre client. Vous pouvez utiliser le service de découverte automatique pour détecter la version d’Exchange cible d’un client pour un utilisateur afin que vous pouvez activer et désactiver les fonctionnalités s’ils sont disponibles pour vos utilisateurs.
  
**Le tableau 1. Disponibilité des fonctionnalités Web service dans les versions d’Exchange et de l’API managée EWS**

|Fonctionnalité de l’API|Exchange Online (Office 365)|API managée EWS|Exchange 2013|Exchange 2010 SP2|Exchange 2010 SP1|Exchange 2010|Exchange 2007 SP1|Exchange 2007|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Résolution de nom ambigu  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Applications pour la gestion d’Outlook  <br/> |X   <br/> |X   <br/> |X   <br/> ||||||
|[Accès de boîte aux lettres d’archive](archiving-in-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|[Découverte automatique (POX)](autodiscover-for-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Découverte automatique (SOAP)](autodiscover-for-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|Réponses automatiques (absence du bureau)  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Disponibilité  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Disponibilité (salles)  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|Transfert en bloc  <br/> |X   <br/> ||X   <br/> |X   <br/> |X   <br/> ||||
|Groupes de contacts  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|Gestion de la conversation  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|Précision DateTime  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||||
|Gestion des délégués  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||
|Développement de listes de distribution  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Accès benne](deleting-items-by-using-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|[découverte électronique](ediscovery-in-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> ||||||
|Fuseaux horaires avancés  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|Autorisations de dossier  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||
|[Conversion de l’identificateur](ews-identifiers-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||
|[Gestion de la boîte de réception](inbox-management-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|[Accès aux éléments et dossiers](folders-and-items-in-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Événements de boîte aux lettres (push et pull)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Événements de boîte aux lettres (diffusion en continu)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|Les infos-courrier  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|Expiration du mot de passe  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||||
|[Personnages](people-and-contacts-in-ews-in-exchange.md) <br/> |X   <br/> ||X   <br/> ||||||
|Publier des éléments  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||
|[Accès aux dossiers publics](public-folder-access-with-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||
|Stratégies de rétention  <br/> |X   <br/> |X   <br/> |X   <br/> ||||||
|[Recherche (indexé)](search-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|[Recherche (magasin)](search-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Synchronisation](mailbox-synchronization-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Magasin de contacts unifié](people-and-contacts-in-ews-in-exchange.md) <br/> |X   <br/> ||X   <br/> ||||||
|[Service Web de messagerie unifiée](http://msdn.microsoft.com/library/83afea8a-c716-41df-9eb2-e1000357afb6%28Office.15%29.aspx) <br/> |X   <br/> ||X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|(Basé sur EWS) de la messagerie unifiée  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|[Objets de configuration utilisateur](persistent-application-settings-in-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|[Photos de l’utilisateur](how-to-get-user-photos-by-using-ews-in-exchange.md) <br/> |X   <br/> ||X   <br/> ||||||
   
Vous trouverez plus d’informations sur le site web des fonctionnalités de service qui sont disponibles dans différentes versions d’Exchange en lecture sur les [opérations EWS](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx), le [service de découverte automatique](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)et les [méthodes ExchangeService](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice_methods%28v=exchg.80%29.aspx).
  
## <a name="to-learn-more"></a>Pour en savoir plus
<a name="bk_apifeatures"> </a>

Si vous souhaitez obtenir davantage de comprendre les différences entre les versions d’Exchange spécifiques, vous pouvez effectuer les opérations suivantes :
  
- Explorez le [schéma EWS](http://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx) pour étudier les différences entre chaque version de EWS plus en détail. 
    
- Télécharger [EWSEditor](http://ewseditor.codeplex.com/). Vous pouvez utiliser EWSEditor pour spécifier les versions de schéma cible différent et soumettre des requêtes en fonction de la version de schéma cible.
    
## <a name="see-also"></a>Voir aussi

- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)   
- [Prise en main des applications clientes d'API managée EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Nouveautés dans EWS et d’autres services web Exchange](whats-new-in-ews-and-other-web-services-in-exchange.md)
    

