---
title: Comparaison d'Exchange Online et programmation du client Exchange sur site
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3c2eabe4-52bc-461e-a6dd-f65f22f16e50
description: Découvrez les considérations relatives à la conception pour la création d’une API managée EWS ou d’une application cliente EWS fonctionnant sur Exchange Online et Exchange en local.
ms.openlocfilehash: 8b4dbae5cadfed377aa3a7179144a7cea68bc35c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456163"
---
# <a name="comparing-exchange-online-and-exchange-on-premises-client-programming"></a>Comparaison d'Exchange Online et programmation du client Exchange sur site

Découvrez les considérations relatives à la conception pour la création d’une API managée EWS ou d’une application cliente EWS fonctionnant sur Exchange Online et Exchange en local.
  
Pour l’essentiel, les clients et les services Web dans Exchange ciblés fonctionnent de la même manière, que la cible soit un serveur Exchange Online, Exchange Online dans le cadre d’Office 365 ou d’Exchange sur site. Il existe toutefois certaines exceptions et vous devez vous assurer que votre application peut les gérer. Utilisez les informations contenues dans cet article pour vous aider à concevoir votre client afin de cibler Exchange Online et Exchange en local.

<a name="autodiscover"> </a>

## <a name="autodiscover-client-programming-considerations"></a>Considérations relatives à la programmation du client de découverte automatique

La [découverte automatique](autodiscover-for-exchange.md) fournit des informations de configuration pour les clients Exchange. Une application cliente peut découvrir ses informations de configuration de trois façons différentes, selon que le client cible ou non Exchange Online ou Exchange local. 
  
**Tableau 1. Types de service de découverte automatique et applicabilité Exchange**

|**Type de service de découverte automatique**|**S’applique à**|
|:-----|:-----|
|[Découverte automatique SOAP](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online et versions d’Exchange en local à partir d’Exchange 2010  <br/> |
|[Découverte automatique POX](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online et versions d’Exchange en local à partir d’Exchange 2007  <br/> |
|[Recherche de point de connexion de service (SCP)](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) <br/> |Versions d’Exchange en local à partir d’Exchange 2007  <br/> |
   
En plus des informations de configuration du client, le service de découverte automatique SOAP et POX renvoie également la version du service Exchange et indique si le service est hébergé par Exchange Online. Ces informations sont renvoyées dans différents éléments, selon le type de découverte automatique que vous utilisez.
  
**Tableau 2. Éléments de découverte automatique qui renvoient la version de service et les informations d’hébergement Exchange Online**

|**Type de service de découverte automatique**|**Élément XML qui contient la version de service**|**Élément XML qui indique si l’utilisateur a un compte Exchange Online**|
|:-----|:-----|:-----|
|Découverte automatique SOAP  <br/> |[Paramètre (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) avec la valeur de texte **CasVersion** .  <br/> |[Paramètre (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) avec la valeur de texte **UserMSOnline** .  <br/> |
|Découverte automatique POX  <br/> |[ServerVersion (POX)](https://msdn.microsoft.com/library/2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a%28Office.15%29.aspx) <br/> |**MicrosoftOnline** <br/> |
   
Assurez-vous que votre client capture ces informations afin qu’il puisse cibler le [jeu de fonctionnalités](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md) disponible sur le serveur Exchange. Cela peut être utile pour déterminer si votre client peut s’attendre à un comportement différent selon que la boîte aux lettres de l’utilisateur se trouve dans une organisation Exchange Online ou Exchange sur site. 

<a name="testing"> </a>

## <a name="testing-and-log-files-in-applications-that-target-exchange-online"></a>Test et fichiers journaux dans les applications qui ciblent Exchange Online

Exchange Online ne fournit pas d’accès aux fichiers journaux de protocole EWS, aux compteurs de performance EWS et aux événements de service liés à EWS qui sont disponibles sur les serveurs Exchange locaux. Toutefois, l’accès à ces éléments est utile pour découvrir comment votre application se comporte lorsqu’elle interagit avec EWS. Assurez-vous de tester votre application par rapport à un serveur Exchange local de test afin de pouvoir optimiser ses performances. Si possible, vous pouvez [modifier les paramètres de limitation](https://technet.microsoft.com/library/bb232205%28v=exchg.150%29.aspx#Policies) sur votre serveur de test pour qu’ils correspondent aux paramètres de limitation pour Exchange Online, afin que vous puissiez évaluer la manière dont votre application se comporte lors de la connexion à Exchange Online. 
  
> [!TIP]
> Vous pouvez utiliser l’outil [EWSRelentless](https://ewsrelentless.codeplex.com/) pour effectuer un test de charge EWS. Vous pouvez utiliser cet outil avec un serveur de test, les journaux de protocole EWS, les compteurs de performance EWS, les événements de service et les paramètres de limitation EWS pour mieux comprendre la façon dont EWS s’exécute sous charge. 

<a name="throttling"> </a>

## <a name="throttling-settings-and-exchange-online"></a>Paramètres de limitation et Exchange Online

Les valeurs par défaut pour les [paramètres de limitation EWS](ews-throttling-in-exchange.md) sont différentes pour Exchange Online et pour Exchange en local. En outre, vous ne pouvez pas modifier les paramètres de limitation d’Exchange Online. Vous pouvez utiliser les cmdlets de l’environnement de commande Exchange Management Shell pour découvrir les paramètres de limitation pour Exchange en local ; Toutefois, ces applets de commande ne sont pas activées pour Exchange Online. 

<a name="ems"> </a>

## <a name="exchange-management-shell-cmdlets-and-configuration-settings"></a>Cmdlets et paramètres de configuration d’Exchange Management Shell

Un certain nombre d’applets de commande peuvent affecter directement ou indirectement les API de service Web dans Exchange Online et Exchange sur site. Les cmdlets ne sont pas disponibles pour les éléments suivants dans Exchange Online :
  
- Paramètres de limitation 
    
- Paramètres de répertoire virtuel 
    
- Paramètres d’authentification
    
Pour plus d’informations sur les applets de commande disponibles pour Exchange Online, voir [applets de commande PowerShell dans Exchange Online](http://help.outlook.com/140/dd575549.aspx). Pour plus d’informations sur les applets de commande disponibles pour Exchange sur site, consultez la rubrique [exchange 2013 cmdlets](https://technet.microsoft.com/library/bb124413%28v=exchg.150%29.aspx).
  
## <a name="client-affinity-and-network-load-balancers"></a>Affinité du client et programmes d’équilibrage de la charge réseau
<a name="affinity"> </a>

La plupart des communications EWS ne nécessitent pas que le client participe à la gestion de l’affinité avec Exchange. Les abonnements aux événements de boîte aux lettres exigent que le client fournisse des cookies et d’autres informations pour maintenir l’affinité avec le serveur Exchange qui gère la file d’attente des événements de boîte aux lettres d’un utilisateur. Exchange Server 2010 utilise le exchangecookie pour maintenir l’affinité du client dans les programmes d’équilibrage de la charge réseau. Exchange Online et les versions d’Exchange en local à partir d’Exchange 2013 utilisent l’en [-tête x-AnchorMailbox, l’en-tête x-PreferServerAffinity et le cookie x-BackEndOverrideCookie](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howmaintained) pour conserver l’affinité pour les notifications de boîte aux lettres. 
  
## <a name="authentication"></a>Authentification
<a name="auth"> </a>

Les clients peuvent s’authentifier auprès d’Exchange Online à l’aide de Basic ou OAuth. Les versions d’Exchange en local à partir d’Exchange 2013 utilisent NTLM par défaut ; Toutefois, il est possible de configurer Exchange localement pour utiliser également l’authentification de base. 
  
## <a name="client-latency-diagnostics"></a>Diagnostics de la latence du client
<a name="diag"> </a>

Exchange Online collecte les diagnostics de latence du client s’ils sont signalés. Cela permet à Microsoft de résoudre les problèmes de connectivité avec Exchange Online. Exchange local ne collecte pas les diagnostics de la latence du client. Si votre client cible Exchange sur site, le client ne peut pas rapporter les diagnostics de latence sur le serveur.
  
## <a name="functionality-in-the-ews-managed-api"></a>Fonctionnalités dans l’API managée EWS
<a name="ewsma"> </a>

L’API managée EWS expose certaines fonctionnalités propres à Exchange en local, telles que la recherche de connexion de point de service, ainsi que certaines fonctionnalités propres à Exchange Online, telles que le rapport de latence de client. Notez que certaines fonctionnalités peuvent être implémentées dans Exchange Online avant d’être implémentées dans l’API managée EWS. 
  
La fonctionnalité d’API managée EWS suivante s’applique uniquement à Exchange Online :
  
- Rapport de latence de client
    
- Pré-authentification de base
    
- Possibilité de demander que le RequestId soit renvoyé dans les réponses
    
## <a name="api-features-in-exchange-online-plans-and-exchange-server-editions"></a>Fonctionnalités de l’API dans les offres Exchange Online et Exchange Server
<a name="exo"> </a>

Différents ensembles de fonctionnalités peuvent être disponibles dans les différents plans Office 365 et Exchange Online, ou dans les versions standard et Enterprise d’Exchange Server. N’oubliez pas que certaines fonctionnalités de l’API peuvent ne pas être disponibles pour votre application cliente en fonction du plan Exchange Online ou de l’édition Exchange Server qui héberge la boîte aux lettres d’un utilisateur. 
  
**Tableau 3. Variations des fonctionnalités de l’API entre les plans et les éditions**

|**Fonctionnalité de l’API**|**Considérations sur la planification ou l’édition**|
|:-----|:-----|

| Accès EWS aux comptes, sauf via l’emprunt d’identité Exchange  <br/> | Non autorisé dans [Office 365 pour les entreprises — plans Kiosk](https://office.microsoft.com/business/compare-office-365-kiosk-plans-FX103178917.aspx).  <br/> |


| Messagerie unifiée (MU)  <br/> | Disponible uniquement avec Office 365 entreprise (E3) plan, Exchange Online plan 2 et Exchange Server 2013 Enterprise Edition.  <br/> | | Intégration des services de domaine Active Directory (AD DS)  <br/> | Non disponible avec Office 365 petite entreprise et Office 365 petite entreprise Premium.  <br/> | | Gestion des droits relatifs à l’information, archivage et conservation légale  <br/> | Disponible uniquement avec les plans Office 365 entreprise (E3 et E4).  <br/> | | Protection contre la perte de données  <br/> | Disponible uniquement avec les offres Office 365 entreprise plans, Exchange Online plan 2 et Exchange Server 2013 Enterprise Edition.  <br/> |
   
Étant donné que la disponibilité des fonctionnalités peut changer, nous vous recommandons de consulter les offres Exchange Online et les éditions Exchange Server pour évaluer la manière dont la disponibilité des fonctionnalités peut affecter votre client. Vous pouvez également concevoir votre client pour vérifier la disponibilité des fonctionnalités à l’aide de l' [opération GetServiceConfiguration](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) ou en envoyant des demandes de test pour les opérations qui implémentent les fonctionnalités. Si la fonctionnalité n’est pas disponible, la réponse du serveur indique en tant que telle. 
  
## <a name="other-considerations"></a>Autres considérations
<a name="other"> </a>

Vous pouvez effectuer les opérations suivantes lorsque vous ciblez Exchange sur site, mais pas Exchange Online :
  
- Créez un client qui est installé sur le serveur Exchange. 
    
- Installez des [agents de transport personnalisés](../transport-agents/transport-agents-in-exchange-2013.md) qui peuvent affecter la remise et le contenu des messages que vous créez et envoyez avec EWS et d’autres clients. 
    
## <a name="see-also"></a>Voir aussi

- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
- [Comparaison entre Exchange Online et Exchange Server 2013](https://blogs.technet.com/b/exchange/archive/2012/09/19/comparing-exchange-online-and-exchange-server-2013.aspx)  
- [Comparaison de tous les plans Office 365 pour les entreprises](https://office.microsoft.com/business/compare-all-office-365-for-business-plans-FX104051403.aspx)
- [EwsRelentless-outil de génération de charge EWS](https://ewsrelentless.codeplex.com/)
- [Disponibilité des fonctionnalités Web service API dans Exchange et de l'API managée EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
- [Limitation EWS dans Exchange](ews-throttling-in-exchange.md)
    

