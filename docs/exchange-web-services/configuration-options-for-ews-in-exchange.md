---
title: Options de configuration pour EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f6562639-9366-4a13-9fdb-2fa737833329
description: Trouvez des informations sur les paramètres de configuration que vous pouvez accéder à votre client EWS et les paramètres configurables Exchange susceptibles d’affecter votre client EWS.
ms.openlocfilehash: d6c2866abf3dc16c77d84355afb9d86b0a9934c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754766"
---
# <a name="configuration-options-for-ews-in-exchange"></a>Options de configuration pour EWS dans Exchange

Trouvez des informations sur les paramètres de configuration que vous pouvez accéder à votre client EWS et les paramètres configurables Exchange susceptibles d’affecter votre client EWS. 
  
De nombreux paramètres de configuration peuvent affecter votre application cliente EWS possible. Ces paramètres de configuration sont : 
  
- En lecture seule ou en lecture-écriture à partir du client.
    
- Accessible sur le serveur Exchange qui héberge votre service EWS.
    
Un client peut accéder aux paramètres sur un serveur Exchange sur site, Exchange Online et Exchange Online dans le cadre d’Office 365. Tous les paramètres du serveur Exchange sur site sont disponibles pour les administrateurs Exchange ; Toutefois, tous ces paramètres sont disponibles pour les administrateurs de client Exchange Online. Cet article décrit les clients de paramètres de configuration, les administrateurs Exchange Server et Exchange Online client les administrateurs peuvent accéder.
  
## <a name="configuration-settings-that-clients-can-access"></a>Paramètres de configuration que les clients peuvent accéder

Votre application client peut obtenir et définir le nombre d’options de configuration du serveur Exchange. Paramètres de configuration nécessaires à toutes les applications EWS sont fournies par le service de découverte automatique. Autres paramètres de configuration sont utilisés pour les scénarios d’application spécifiques. 
  
**Le tableau 1. Fonctionnalités du service Web qui fournissent des options de configuration pour les clients EWS**

|**Fonctionnalité**|**Description**|
|:-----|:-----|
|Service de découverte automatique  <br/> |Le [service de découverte automatique](autodiscover-for-exchange.md) fournit des applications avec des informations de configuration de votre client afin que votre client peut se configurer automatiquement pour communiquer avec EWS.  <br/> |
|Informations de configuration personnalisées stockées dans une boîte aux lettres  <br/> |Vous pouvez utiliser une des options pour [stocker les informations de configuration personnalisées](persistent-application-settings-in-ews-in-exchange.md) dans votre boîte aux lettres : objets de configuration utilisateur, des éléments personnalisés ou les propriétés étendues.  <br/> |
|Gestion des délégués  <br/> | EWS fournit des opérations pour la gestion de l’accès délégué à une boîte aux lettres. Les délégués sont des utilisateurs qui disposent de l’autorisation d’accéder aux boîtes aux lettres d’un autre utilisateur.<br/><br/>  Vous pouvez utiliser les [opérations de gestion de délégué](http://msdn.microsoft.com/en-us/library/bb409286%28v=exchg.150%29.aspx#bk_delegate_management) pour permettre la gestion de délégué à l’aide de EWS, ou, si vous utilisez l’API managée EWS, vous pouvez utiliser les méthodes suivantes :<br/><br/>- [ExchangeService.AddDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.GetDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getdelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.UpdateDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.RemoveDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |
|configuration de recherche de découverte électronique  <br/> |applications clientes de découverte électronique peuvent obtenir des [informations de configuration de recherche](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) qui inclut une requête de recherche eDiscovery, une liste des boîtes aux lettres de recherche, et conserve l’identificateur de boîte aux lettres sur place.  <br/> |
|Autorisations de dossier  <br/> |Limitent les autorisations de dossiers qu’un utilisateur peut effectuer dans un dossier public, et dans le cas d’accès délégué, qu’un délégué peut faire dans le dossier d’un autre utilisateur. Vous pouvez utiliser la méthode [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) ou l' [opération GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour accéder à l’ensemble de l’autorisation de chaque dossier, y compris les dossiers publics, des dossiers privés partagés ou des dossiers auxquels les utilisateurs ont accès délégué.  <br/> |
|Conseils, la messagerie unifiée ou les règles de protection de messagerie  <br/> |L' [opération GetServiceConfiguration](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) fournit des [informations de configuration de service](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) en lecture seule pour des conseils de messagerie, la messagerie unifiée et les règles de protection.  <br/> |
   
## <a name="configuration-settings-that-administrators-can-access-on-the-exchange-server"></a>Paramètres de configuration que les administrateurs peuvent accéder sur le serveur Exchange

La plupart des scénarios d’application client ne nécessitent pas de modifications apportées aux paramètres de configuration du serveur ; Toutefois, certains scénarios de le faire. Par exemple, pour activer une application de niveau intermédiaire agir en tant qu’utilisateur, vous devez définir l’emprunt d’identité Exchange sur le serveur. Notez que certains paramètres accessibles uniquement sur des serveurs Exchange locaux. Si vous ciblez Exchange Online, votre application cliente devront travailler avec les paramètres par défaut.
  
**Le tableau 2. Options de configuration de serveur Exchange qui affectent les clients EWS**

|**Fonctionnalité**|**Accessible à partir d’Exchange Online ?**|**Pour plus d’informations, voir...**|
|:-----|:-----|:-----|
|Paramètres de répertoire virtuel (y compris l’authentification)  <br/> |Non  <br/> |[Get-WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa998810%28v=exchg.150%29.aspx) <br/> [Set-WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx) <br/> |
|Découverte automatique  <br/> |Non  <br/> |[Get-AutodiscoverVirtualDirectory](http://technet.microsoft.com/en-us/library/aa996819%28v=exchg.150%29.aspx) <br/> [Set-AutodiscoverVirtualDirectory](http://technet.microsoft.com/en-us/library/aa998601%28v=exchg.150%29.aspx) <br/> |
|Conformité  <br/> |Oui  <br/> |[L’archivage](http://technet.microsoft.com/en-us/library/dd979800%28v=exchg.150%29.aspx) <br/> [découverte électronique](http://technet.microsoft.com/en-us/library/dd298021%28v=exchg.150%29.aspx) <br/> [Blocage de rétention](http://technet.microsoft.com/en-us/library/dd335168%28v=exchg.150%29.aspx) <br/> [Protection contre la perte de données](http://technet.microsoft.com/en-us/library/jj150527%28v=exchg.150%29.aspx) <br/> |
|Gestion des délégués  <br/> |Oui  <br/> |[Gérer les autorisations pour les destinataires](http://technet.microsoft.com/en-us/library/jj919240%28v=exchg.150%29.aspx) <br/> |
|Emprunt d’identité Exchange  <br/> |Oui  <br/> |[Configurer l’emprunt d’identité Exchange](http://msdn.microsoft.com/en-us/library/bb204095%28EXCHG.140%29.aspx) <br/> |
|Conseils, la messagerie unifiée ou les règles de protection de messagerie  <br/> |Oui  <br/> |[Les infos-courrier](http://technet.microsoft.com/en-us/library/jj649091%28v=exchg.150%29.aspx) <br/> [Cmdlets de messagerie unifiée](http://technet.microsoft.com/en-us/library/aa997665%28v=exchg.150%29.aspx) <br/> [Règles de Protection d’Outlook](http://technet.microsoft.com/en-us/library/dd638178%28v=exchg.150%29.aspx) <br/> |
|Limitation  <br/> |Non  <br/> |[Paramètres de limitation](ews-throttling-in-exchange.md) <br/> |
|Agent utilisateur de filtrage  <br/> |Oui  <br/> |[Agent utilisateur de filtrage](how-to-control-access-to-ews-in-exchange.md) <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Obtenir des informations de configuration de service à l’aide de EWS dans Exchange](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)   
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)   
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    

