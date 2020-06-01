---
title: Options de configuration pour EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f6562639-9366-4a13-9fdb-2fa737833329
description: Trouvez des informations sur les paramètres de configuration auxquels votre client EWS peut accéder, ainsi que les paramètres Exchange configurables qui peuvent affecter votre client EWS.
ms.openlocfilehash: 55f927b7b301bdfaa298bcd254b18a00cf1692d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456156"
---
# <a name="configuration-options-for-ews-in-exchange"></a>Options de configuration pour EWS dans Exchange

Trouvez des informations sur les paramètres de configuration auxquels votre client EWS peut accéder, ainsi que les paramètres Exchange configurables qui peuvent affecter votre client EWS. 
  
De nombreux paramètres de configuration peuvent affecter ce que votre application cliente EWS peut faire. Ces paramètres de configuration sont les suivants : 
  
- En lecture seule ou en lecture-écriture à partir du client.
    
- Accessible sur le serveur Exchange qui héberge votre service EWS.
    
Un client peut accéder aux paramètres sur Exchange Online, Exchange Online dans le cadre d’Office 365 et un serveur Exchange local. Tous les paramètres Exchange Server locaux sont disponibles pour les administrateurs Exchange ; Toutefois, tous ces paramètres ne sont pas disponibles pour les administrateurs clients Exchange Online. Cet article décrit les paramètres de configuration auxquels les clients, les administrateurs Exchange Server et les administrateurs de clients Exchange Online peuvent accéder.
  
## <a name="configuration-settings-that-clients-can-access"></a>Paramètres de configuration auxquels les clients peuvent accéder

Votre application cliente peut obtenir et définir un certain nombre d’options de configuration à partir du serveur Exchange. Les paramètres de configuration dont toutes les applications EWS ont besoin sont fournis par le service de découverte automatique. D’autres paramètres de configuration sont utilisés pour des scénarios d’application spécifiques. 
  
**Tableau 1. Fonctionnalités de service Web qui fournissent des options de configuration pour les clients EWS**

|**Fonctionnalité**|**Description**|
|:-----|:-----|
|Service de découverte automatique  <br/> |Le [service de découverte](autodiscover-for-exchange.md) automatique fournit des informations de configuration à vos applications clientes afin que votre client puisse se configurer automatiquement pour communiquer avec EWS.  <br/> |
|Informations de configuration personnalisées stockées dans une boîte aux lettres  <br/> |Vous pouvez utiliser l’une des options suivantes pour [stocker les informations de configuration personnalisées](persistent-application-settings-in-ews-in-exchange.md) dans votre boîte aux lettres : objets de configuration utilisateur, éléments personnalisés ou propriétés étendues.  <br/> |
|Gestion des délégués  <br/> | EWS fournit des opérations CRUD pour la gestion de l’accès délégué à une boîte aux lettres. Les délégués sont des utilisateurs qui ont reçu l’autorisation d’accéder à la boîte aux lettres d’un autre utilisateur.<br/><br/>  Vous pouvez utiliser les [opérations de gestion de délégué](https://msdn.microsoft.com/library/bb409286%28v=exchg.150%29.aspx#bk_delegate_management) pour activer la gestion des délégués à l’aide d’EWS ou, si vous utilisez l’API managée EWS, vous pouvez utiliser les méthodes suivantes :<br/><br/>- [ExchangeService. AddDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService. GetDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getdelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService. UpdateDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService. RemoveDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |
|configuration de la recherche eDiscovery  <br/> |les applications clientes eDiscovery peuvent obtenir des [informations de configuration](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) de la recherche qui incluent une requête de recherche de découverte électronique, une liste de boîtes aux lettres pouvant faire l’objet d’une recherche et l’identificateur de conservation des boîtes aux lettres sur place.  <br/> |
|Autorisations d’accès aux dossiers  <br/> |Les autorisations de dossier limitent ce qu’un utilisateur peut faire dans un dossier public, et dans le cas d’un accès délégué, ce qu’un délégué peut faire dans le dossier d’un autre utilisateur. Vous pouvez utiliser la méthode [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) ou l' [opération GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour accéder au jeu d’autorisations de chaque dossier, y compris les dossiers publics, les dossiers privés partagés ou les dossiers auxquels les utilisateurs ont un accès délégué.  <br/> |
|Conseils de messagerie, messagerie unifiée ou règles de protection  <br/> |L' [opération GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) fournit des informations de [configuration de service](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) en lecture seule pour les conseils de messagerie, la messagerie unifiée et les règles de protection.  <br/> |
   
## <a name="configuration-settings-that-administrators-can-access-on-the-exchange-server"></a>Paramètres de configuration auxquels les administrateurs peuvent accéder sur le serveur Exchange

La plupart des scénarios d’application cliente n’ont pas besoin de modifier les paramètres de configuration du serveur ; Toutefois, certains scénarios le font. Par exemple, pour permettre à une application intermédiaire de se comporter comme un utilisateur, vous devez définir l’emprunt d’identité Exchange sur le serveur. Notez que certains paramètres ne sont accessibles que sur les serveurs Exchange locaux. Si vous ciblez Exchange Online, il se peut que votre application cliente doive fonctionner avec les paramètres par défaut.
  
**Tableau 2. Options de configuration d’Exchange Server qui affectent les clients EWS**

|**Fonctionnalité**|**Accessible à partir d’Exchange Online ?**|**Pour plus d’informations, reportez-vous à...**|
|:-----|:-----|:-----|
|Paramètres de répertoire virtuel (y compris l’authentification)  <br/> |Non  <br/> |[Get-WebServicesVirtualDirectory](https://technet.microsoft.com/library/aa998810%28v=exchg.150%29.aspx) <br/> [Set-WebServicesVirtualDirectory](https://technet.microsoft.com/library/aa997233%28v=exchg.150%29.aspx) <br/> |
|Découverte automatique  <br/> |Non  <br/> |[Get-AutodiscoverVirtualDirectory permet](https://technet.microsoft.com/library/aa996819%28v=exchg.150%29.aspx) <br/> [Set-AutodiscoverVirtualDirectory permet](https://technet.microsoft.com/library/aa998601%28v=exchg.150%29.aspx) <br/> |
|Conformité  <br/> |Oui  <br/> |[Archivage](https://technet.microsoft.com/library/dd979800%28v=exchg.150%29.aspx) <br/> [eDiscovery](https://technet.microsoft.com/library/dd298021%28v=exchg.150%29.aspx) <br/> [Blocage de rétention](https://technet.microsoft.com/library/dd335168%28v=exchg.150%29.aspx) <br/> [Protection contre la perte de données](https://technet.microsoft.com/library/jj150527%28v=exchg.150%29.aspx) <br/> |
|Gestion des délégués  <br/> |Oui  <br/> |[Manage Permissions for Recipients](https://technet.microsoft.com/library/jj919240%28v=exchg.150%29.aspx) <br/> |
|Emprunt d’identité Exchange  <br/> |Oui  <br/> |[Configurer l’emprunt d’identité Exchange](https://msdn.microsoft.com/library/bb204095%28EXCHG.140%29.aspx) <br/> |
|Conseils de messagerie, messagerie unifiée ou règles de protection  <br/> |Oui  <br/> |[Infos-courrier](https://technet.microsoft.com/library/jj649091%28v=exchg.150%29.aspx) <br/> [Cmdlets de messagerie unifiée](https://technet.microsoft.com/library/aa997665%28v=exchg.150%29.aspx) <br/> [Règles de protection Outlook](https://technet.microsoft.com/library/dd638178%28v=exchg.150%29.aspx) <br/> |
|Limitation  <br/> |Non  <br/> |[Paramètres de limitation](ews-throttling-in-exchange.md) <br/> |
|Filtrage de l’agent utilisateur  <br/> |Oui  <br/> |[Filtrage de l’agent utilisateur](how-to-control-access-to-ews-in-exchange.md) <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Obtenir des informations de configuration de service à l’aide d’EWS dans Exchange](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)   
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)   
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    

