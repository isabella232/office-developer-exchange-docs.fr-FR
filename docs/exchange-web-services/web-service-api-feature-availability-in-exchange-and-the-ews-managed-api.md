---
title: Disponibilité des fonctionnalités Web service API dans Exchange et de l'API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 07d3e6e8-d549-4ad7-baa4-bc531dfb7dd2
description: Découvrez les fonctionnalités EWS et d’API de service web disponibles dans chaque version de Exchange et l’API gérée EWS.
ms.openlocfilehash: 6fc0c40410be543b149885c7b0785a2c6c8828af
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544471"
---
# <a name="web-service-api-feature-availability-in-exchange-and-the-ews-managed-api"></a>Disponibilité des fonctionnalités Web service API dans Exchange et de l'API managée EWS

Découvrez les fonctionnalités EWS et d’API de service web disponibles dans chaque version de Exchange et l’API gérée EWS.
  
Exchange applications clientes ciblent souvent de nombreuses versions de Exchange. Pour cette raison, vous pouvez concevoir votre application afin de pouvoir activer et désactiver les fonctionnalités [clientes EWS](ews-client-design-overview-for-exchange.md#EWSFeatures) en fonction de la version de Exchange qui héberge la boîte aux lettres de vos utilisateurs. Cet article fournit des informations sur les fonctionnalités d’API de service disponibles dans différentes versions de Exchange et de l’API gérée EWS. Utilisez ces informations pour concevoir votre application afin qu’elle s’applique largement aux clients exécutant plusieurs versions de Exchange. 
  
Pour plus d’informations sur les différences entre les versions de Exchange, examinez les fichiers de schéma EWS et la documentation de [référence associée.](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx)
  
## <a name="api-features-by-exchange-version"></a>Fonctionnalités d’API Exchange version
<a name="bk_apifeatures"> </a>

Les EXCHANGE de service web, y compris EWS et la découverte automatique, sont développées avec la compatibilité multi-version à l’esprit. Par conséquent, une application qui cible Exchange 2007 fonctionne également par rapport aux versions de Exchange à partir de Exchange 2013, y compris Exchange Online et Exchange Online dans le cadre de Office 365. 
  
Le tableau suivant indique les fonctionnalités d’API disponibles dans chaque version de Exchange et les versions de l’API gérée EWS à partir de la version 2.0. Étant donné que votre application peut cibler plusieurs versions de Exchange, il vous sera utile de savoir quelles versions peuvent prendre en charge les fonctionnalités implémentées par votre client. Vous pouvez utiliser le service de découverte automatique pour découvrir la version de Exchange cible d’un client pour un utilisateur afin de pouvoir activer et désactiver des fonctionnalités selon qu’elles sont disponibles pour vos utilisateurs.
  
**Tableau 1. Disponibilité des fonctionnalités de service Web dans les versions de Exchange et de l’API gérée EWS**

|Fonctionnalité d’API|Exchange Online (Office 365)|API managée EWS|Exchange 2013|Exchange 2010 SP2|Exchange 2010 SP1|Exchange 2010|Exchange 2007 SP1|Exchange 2007|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Résolution de nom ambigu  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Gestion des applications pour Outlook de gestion  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Accès aux boîtes aux lettres d’archivage](archiving-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Découverte automatique (POX)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Découverte automatique (SOAP)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Réponses automatiques (OOF)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Disponibilité  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Disponibilité (Salles)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Transfert en bloc  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> ||||
|Groupes de contacts  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Gestion des conversations  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Précision date/heure  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|Déléguer la gestion  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Développement de listes de distribution  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Accès au benne](deleting-items-by-using-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[eDiscovery](ediscovery-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|Fuseaux horaires améliorés  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Autorisations d’accès aux dossiers  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Conversion d’identificateur](ews-identifiers-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Gestion de la boîte de réception](inbox-management-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Accès aux éléments et aux dossiers](folders-and-items-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Événements de boîte aux lettres (pull-push)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Événements de boîte aux lettres (diffusion en continu)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Mailtips  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Expiration du mot de passe  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|[Personas](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|Publier des éléments  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Accès aux dossiers publics](public-folder-access-with-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Stratégies de rétention  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Recherche (indexée)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Recherche (store)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Synchronisation](mailbox-synchronization-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Magasin de contacts unifié](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|[Service Web de messagerie unifiée](https://msdn.microsoft.com/library/83afea8a-c716-41df-9eb2-e1000357afb6%28Office.15%29.aspx) <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Messagerie unifiée (basée sur EWS)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Objets de configuration utilisateur](persistent-application-settings-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Photos de l'utilisateur](how-to-get-user-photos-by-using-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
   
Pour plus d’informations sur les fonctionnalités de service web disponibles dans différentes versions de Exchange, voir les opérations [EWS,](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx)le [service](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)de découverte automatique et les méthodes [ExchangeService.](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice_methods%28v=exchg.80%29.aspx)
  
## <a name="to-learn-more"></a>Pour en savoir plus
<a name="bk_apifeatures"> </a>

Si vous souhaitez approfondir la compréhension des différences spécifiques entre Exchange versions, vous pouvez :
  
- Explorez le [schéma EWS pour](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx) examiner plus en détail les différences entre chaque version d’EWS. 
    
- Téléchargez [EWSEditor](http://ewseditor.codeplex.com/). Vous pouvez utiliser EWSEditor pour spécifier différentes versions de schéma cible et soumettre des requêtes en fonction de la version de schéma cible.
    
## <a name="see-also"></a>Voir aussi

- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)   
- [Prise en main des applications clientes d'API managée EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Nouveautés d’EWS et d’autres services web dans Exchange](whats-new-in-ews-and-other-web-services-in-exchange.md)
    

