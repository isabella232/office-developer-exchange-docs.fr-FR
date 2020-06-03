---
title: Disponibilité des fonctionnalités Web service API dans Exchange et de l'API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 07d3e6e8-d549-4ad7-baa4-bc531dfb7dd2
description: Découvrez les fonctionnalités d’EWS et d’API de service Web disponibles dans chaque version d’Exchange et l’API managée EWS.
ms.openlocfilehash: f15cf4784a59c18d1bb9ae20af378baed084acc3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529846"
---
# <a name="web-service-api-feature-availability-in-exchange-and-the-ews-managed-api"></a>Disponibilité des fonctionnalités Web service API dans Exchange et de l'API managée EWS

Découvrez les fonctionnalités d’EWS et d’API de service Web disponibles dans chaque version d’Exchange et l’API managée EWS.
  
Les applications clientes Exchange ciblent souvent de nombreuses versions d’Exchange. Pour cette raison, vous pouvez concevoir votre application de sorte que vous puissiez activer et désactiver les [fonctionnalités clientes EWS](ews-client-design-overview-for-exchange.md#EWSFeatures) en fonction de la version d’Exchange qui héberge la boîte aux lettres de vos utilisateurs. Cet article fournit des informations sur les fonctionnalités d’API de service disponibles dans les différentes versions d’Exchange et de l’API managée EWS. Utilisez ces informations pour concevoir votre application afin qu’elle s’applique largement aux clients exécutant plusieurs versions d’Exchange. 
  
Pour plus d’informations sur les différences entre les versions d’Exchange, consultez les fichiers de schéma EWS et la [documentation de référence](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx)associée.
  
## <a name="api-features-by-exchange-version"></a>Fonctionnalités de l’API par la version d’Exchange
<a name="bk_apifeatures"> </a>

Les API de service Web Exchange, y compris EWS et la découverte automatique, sont développées en tenant compte de la compatibilité multi-versions. Par conséquent, une application qui cible Exchange 2007 fonctionne également sur les versions d’Exchange à partir d’Exchange 2013, y compris Exchange Online et Exchange Online dans le cadre d’Office 365. 
  
Le tableau suivant indique les fonctionnalités d’API disponibles dans chaque version d’Exchange et les versions de l’API managée EWS à partir de la version 2,0. Étant donné que votre application peut cibler plusieurs versions d’Exchange, il vous sera utile de savoir quelles versions prennent en charge les fonctionnalités que votre client implémente. Vous pouvez utiliser le service de découverte automatique pour découvrir la version d’Exchange que le client cible pour un utilisateur afin de pouvoir activer et désactiver les fonctionnalités selon qu’elles sont disponibles ou non pour vos utilisateurs.
  
**Tableau 1. Disponibilité des fonctionnalités de service Web dans les versions d’Exchange et de l’API managée EWS**

|Fonctionnalité de l’API|Exchange Online (Office 365)|API managée EWS|Exchange 2013|Exchange 2010 SP2|Exchange 2010 SP1|Exchange 2010|Exchange 2007 SP1|Exchange 2007|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Résolution de noms ambigus  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Applications pour la gestion d’Outlook  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Accès aux boîtes aux lettres d’archivage](archiving-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Découverte automatique (POX)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Découverte automatique (SOAP)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Réponses automatiques (OOF)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Disponibilité  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Disponibilité (salles)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Transfert en bloc  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> ||||
|Groupes de contacts  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Gestion des conversations  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|DateTime, précision  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|Gestion des délégués  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Développement de la liste de distribution  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Accès à la benne](deleting-items-by-using-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[eDiscovery](ediscovery-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|Fuseaux horaires améliorés  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Autorisations d’accès aux dossiers  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Conversion de l’identificateur](ews-identifiers-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Gestion de la boîte de réception](inbox-management-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Accès aux éléments et aux dossiers](folders-and-items-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Événements de boîte aux lettres (extraction et émission)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Événements de boîte aux lettres (diffusion en continu)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Infos-courrier  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Expiration du mot de passe  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|[Personnages](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|Publier des éléments  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Accès aux dossiers publics](public-folder-access-with-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Stratégies de rétention  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Recherche (indexée)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Recherche (magasin)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Synchronisation](mailbox-synchronization-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Magasin de contacts unifié](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|[Service Web de messagerie unifiée](https://msdn.microsoft.com/library/83afea8a-c716-41df-9eb2-e1000357afb6%28Office.15%29.aspx) <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Messagerie unifiée (EWS)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Objets de configuration utilisateur](persistent-application-settings-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Photos de l'utilisateur](how-to-get-user-photos-by-using-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
   
Pour plus d’informations sur les fonctionnalités de service Web disponibles dans différentes versions d’Exchange, consultez les [opérations EWS](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx), le [service de découverte automatique](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)et les [méthodes ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice_methods%28v=exchg.80%29.aspx).
  
## <a name="to-learn-more"></a>Pour en savoir plus
<a name="bk_apifeatures"> </a>

Si vous souhaitez approfondir votre compréhension des différences spécifiques entre les versions d’Exchange, vous pouvez effectuer l’une des opérations suivantes :
  
- Explorez le [schéma EWS](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx) pour examiner en détail les différences entre chaque version d’EWS. 
    
- Téléchargez [EWSEditor](http://ewseditor.codeplex.com/). Vous pouvez utiliser EWSEditor pour spécifier différentes versions de schéma cible et soumettre des requêtes basées sur la version du schéma cible.
    
## <a name="see-also"></a>Voir aussi

- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)   
- [Prise en main des applications clientes d'API managée EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Nouveautés d’EWS et d’autres services Web dans Exchange](whats-new-in-ews-and-other-web-services-in-exchange.md)
    

