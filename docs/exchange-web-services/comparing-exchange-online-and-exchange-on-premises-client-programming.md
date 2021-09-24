---
title: Comparaison de programmation du client Exchange local et d’Exchange Online
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 3c2eabe4-52bc-461e-a6dd-f65f22f16e50
description: Découvrez les considérations de conception pour la création d’une API gérée EWS ou d’une application cliente EWS qui fonctionne sur Exchange Online et Exchange en local.
ms.openlocfilehash: 438965656e31eca586d06a5e0b6794c0eda87621
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512287"
---
# <a name="comparing-exchange-online-and-exchange-on-premises-client-programming"></a>Comparaison de programmation du client Exchange local et d’Exchange Online

Découvrez les considérations de conception pour la création d’une API gérée EWS ou d’une application cliente EWS qui fonctionne sur Exchange Online et Exchange en local.
  
La plupart du temps, les clients et les services web dans Exchange qu’ils ciblent fonctionnent de la même manière, que la cible soit un serveur local Exchange Online, Exchange Online dans le cadre de Office 365 ou Exchange. Toutefois, il existe certaines exceptions et vous devez vous assurer que votre application peut les gérer. Utilisez les informations de cet article pour vous aider à concevoir votre client de telle Exchange Online et Exchange en local.

<a name="autodiscover"> </a>

## <a name="autodiscover-client-programming-considerations"></a>Considérations sur la programmation du client de découverte automatique

[La découverte automatique fournit des](autodiscover-for-exchange.md) informations de configuration pour Exchange clients. Une application cliente peut découvrir ses informations de configuration de trois manières, selon que le client cible Exchange Online ou Exchange en local. 
  
**Tableau 1. Types de service de découverte automatique et applicabilité Exchange’application**

|**Type de service de découverte automatique**|**S’applique à**|
|:-----|:-----|
|[Découverte automatique SOAP](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online versions de Exchange en local à partir de Exchange 2010  <br/> |
|[Découverte automatique POX](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online versions de Exchange en local à partir de Exchange 2007  <br/> |
|[Recherche de point de connexion de service (SCP)](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) <br/> |Versions de Exchange en local à partir de Exchange 2007  <br/> |
   
Outre les informations de configuration du client, la découverte automatique SOAP et POX retourne également la version du service Exchange et indique si le service est hébergé par Exchange Online. Ces informations sont renvoyées dans différents éléments, selon le type de découverte automatique que vous utilisez.
  
**Tableau 2. Éléments de découverte automatique qui retournent la version du service et Exchange Online’hébergement**

|**Type de service de découverte automatique**|**Élément XML qui contient la version du service**|**Élément XML qui indique si l’utilisateur possède un compte Exchange Online client**|
|:-----|:-----|:-----|
|Découverte automatique SOAP  <br/> |[Élément SETTING (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) avec la **valeur de texte CasVersion.**  <br/> |[Élément Setting (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) avec la valeur de texte **UserMSOnline.**  <br/> |
|Découverte automatique POX  <br/> |[ServerVersion (POX)](https://msdn.microsoft.com/library/2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a%28Office.15%29.aspx) <br/> |**MicrosoftOnline** <br/> |
   
Assurez-vous que votre client capture ces [](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md) informations afin qu’il puisse cibler l’ensemble de fonctionnalités disponible sur Exchange serveur. Cela peut être utile pour déterminer si votre client peut s’attendre à un comportement différent selon que la boîte aux lettres de l’utilisateur se trouve dans une organisation Exchange Online ou Exchange sur site. 

<a name="testing"> </a>

## <a name="testing-and-log-files-in-applications-that-target-exchange-online"></a>Test et fichiers journaux dans les applications qui ciblent Exchange Online

Exchange Online ne fournit pas d’accès aux fichiers journaux de protocole EWS, aux compteurs de performance EWS et aux événements de service liés à EWS disponibles sur les serveurs Exchange locaux. L’accès à ces derniers est toutefois utile pour découvrir comment votre application fonctionne lorsqu’elle interagit avec EWS. Veillez à tester votre application sur un serveur Exchange afin d’optimiser ses performances. Si possible, vous pouvez modifier les [paramètres](https://technet.microsoft.com/library/bb232205%28v=exchg.150%29.aspx#Policies) de limitation sur votre serveur de test afin qu’ils correspondent aux paramètres de limitation pour Exchange Online, afin de pouvoir évaluer le comportement de votre application lorsqu’elle se connecte à Exchange Online. 
  
> [!TIP]
> Vous pouvez utiliser [l’outil EWSRelentless](https://ewsrelentless.codeplex.com/) pour effectuer un test de charge EWS. Vous pouvez utiliser cet outil avec un serveur de test, les journaux de protocole EWS, les compteurs de performance EWS, les événements de service et les paramètres de limitation EWS pour mieux comprendre les performances d’EWS sous charge. 

<a name="throttling"> </a>

## <a name="throttling-settings-and-exchange-online"></a>Paramètres et paramètres de limitation Exchange Online

Les valeurs par défaut des paramètres de limitation [EWS](ews-throttling-in-exchange.md) sont différentes pour Exchange Online et pour Exchange en local. En outre, vous ne pouvez pas modifier Exchange Online paramètres de limitation. Vous pouvez utiliser les cmdlets Exchange Management Shell pour découvrir les paramètres de limitation pour Exchange en local ; toutefois, ces cmdlets ne sont pas activées pour les Exchange Online. 

<a name="ems"> </a>

## <a name="exchange-management-shell-cmdlets-and-configuration-settings"></a>Exchange Cmdlets et paramètres de configuration de Management Shell

Un certain nombre d’cmdlets peuvent affecter directement ou indirectement les API de service web Exchange Online et Exchange en local. Les cmdlets ne sont pas disponibles pour les Exchange Online :
  
- Paramètres de limitation 
    
- Paramètres du répertoire virtuel 
    
- Paramètres d’authentification
    
Pour plus d’informations sur les cmdlets disponibles pour les Exchange Online, voir les [cmdlets PowerShell](http://help.outlook.com/140/dd575549.aspx)dans Exchange Online . Pour plus d’informations sur les cmdlets disponibles Exchange en local, voir [Exchange 2013 cmdlets](https://technet.microsoft.com/library/bb124413%28v=exchg.150%29.aspx).
  
## <a name="client-affinity-and-network-load-balancers"></a>Affinité client et équilibreurs de charge réseau
<a name="affinity"> </a>

La plupart des communications EWS ne nécessitent pas que le client participe au maintien de l’affinité avec Exchange. Les abonnements aux événements de boîte aux lettres nécessitent que le client fournisse des cookies et d’autres informations pour maintenir l’affinité avec le serveur Exchange qui maintient la file d’attente des événements de boîte aux lettres pour un utilisateur. Exchange Server 2010 utilise exchangecookie pour maintenir l’affinité client entre les équilibreurs de charge réseau. Exchange Online et les versions de Exchange en local à partir de Exchange 2013 utilisent [l’en-tête X-AnchorMailbox, l’en-tête X-PreferServerAffinity et le cookie X-BackEndOverrideCookie](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howmaintained) pour conserver l’affinité pour les notifications de boîte aux lettres. 
  
## <a name="authentication"></a>Authentification
<a name="auth"> </a>

Les clients peuvent s’authentifier auprès Exchange Online l’aide de Basic ou OAuth. Les versions de Exchange en local à partir de Exchange 2013 utilisent NTLM par défaut ; Toutefois, il est possible de configurer Exchange local pour utiliser l’authentification de base également. 
  
## <a name="client-latency-diagnostics"></a>Diagnostics de latence des clients
<a name="diag"> </a>

Exchange Online collecte les diagnostics de latence des clients s’ils sont signalés. Cela permet à Microsoft de résoudre les problèmes de connectivité avec Exchange Online. Exchange local ne collecte pas les diagnostics de latence des clients. Si votre client cible Exchange local, le client ne peut pas signaler de diagnostics de latence au serveur.
  
## <a name="functionality-in-the-ews-managed-api"></a>Fonctionnalités dans l’API gérée EWS
<a name="ewsma"> </a>

L’API gérée EWS expose certaines fonctionnalités spécifiques à Exchange en local, telles que la recherche de connexion de point de service et certaines fonctionnalités spécifiques à Exchange Online, telles que les rapports de latence des clients. Notez qu’il est possible d’implémenter certaines fonctionnalités dans Exchange Online avant d’être implémentées dans l’API gérée EWS. 
  
La fonctionnalité d’API gérée EWS suivante s’applique uniquement aux Exchange Online :
  
- Rapports de latence des clients
    
- Pré-authentification de base
    
- Possibilité de demander le retour du RequestId dans les réponses
    
## <a name="api-features-in-exchange-online-plans-and-exchange-server-editions"></a>Fonctionnalités api dans Exchange Online plans et éditions Exchange Server éditions
<a name="exo"> </a>

Différents ensembles de fonctionnalités peuvent être disponibles dans différents plans Office 365 et Exchange Online, ou dans les versions standard et d’entreprise de Exchange Server. N’ignorez pas que certaines fonctionnalités d’API peuvent ne pas être disponibles pour votre application cliente en fonction du plan Exchange Online ou de l’édition Exchange Server qui héberge la boîte aux lettres d’un utilisateur. 
   
Étant donné que la disponibilité des fonctionnalités peut changer, nous vous recommandons de vérifier les plans Exchange Online et les éditions Exchange Server pour évaluer l’impact de la disponibilité des fonctionnalités sur votre client. Vous pouvez également concevoir votre client pour vérifier la disponibilité des fonctionnalités à l’aide de l’opération [GetServiceConfiguration](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) ou en envoyant des demandes de test pour les opérations qui implémentent les fonctionnalités. Si la fonctionnalité n’est pas disponible, la réponse du serveur indique en tant que telle. 
  
## <a name="other-considerations"></a>Autres considérations
<a name="other"> </a>

Vous pouvez faire les choses suivantes lorsque vous ciblez Exchange local, mais pas Exchange Online :
  
- Créez un client installé sur le Exchange serveur. 
    
- Installez [des agents de transport](../transport-agents/transport-agents-in-exchange-2013.md) personnalisés qui peuvent affecter la remise et le contenu des messages que vous créez et envoyez avec EWS et d’autres clients. 
    
## <a name="see-also"></a>Voir aussi

- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
- [Comparaison des Exchange Online et Exchange Server 2013](https://blogs.technet.com/b/exchange/archive/2012/09/19/comparing-exchange-online-and-exchange-server-2013.aspx)  
- [Comparer tous les Office 365 pour les plans pour les entreprises](https://office.microsoft.com/business/compare-all-office-365-for-business-plans-FX104051403.aspx)
- [EwsRelentless - Outil de génération de charge EWS](https://ewsrelentless.codeplex.com/)
- [Disponibilité des fonctionnalités Web service API dans Exchange et de l'API managée EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
- [Limitation EWS dans Exchange](ews-throttling-in-exchange.md)
    

