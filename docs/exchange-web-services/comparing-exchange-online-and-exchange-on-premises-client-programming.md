---
title: Comparaison d’Exchange Online et programmation du client Exchange sur site
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3c2eabe4-52bc-461e-a6dd-f65f22f16e50
description: Obtenir des informations sur les considérations de conception pour la création d’une API managées ou une application cliente EWS qui fonctionne par rapport à Exchange Online et Exchange sur site.
ms.openlocfilehash: 87c6ee476e06b50c339901bf61020b0fc98f8486
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754789"
---
# <a name="comparing-exchange-online-and-exchange-on-premises-client-programming"></a>Comparaison d’Exchange Online et programmation du client Exchange sur site

Obtenir des informations sur les considérations de conception pour la création d’une API managées ou une application cliente EWS qui fonctionne par rapport à Exchange Online et Exchange sur site.
  
Pour la plupart des cas, les clients et le site web services dans Exchange elles ciblent fonctionnera de la même manière que si la cible est un Exchange Online, Exchange Online dans le cadre d’Office 365, ou Exchange server sur site. Il existe toutefois des exceptions, et vous souhaiterez pour vous assurer que votre application peut gérer les. Utilisez les informations de cet article pour vous aider à concevoir votre client pour cibler les deux Exchange Online et Exchange sur site.

<a name="autodiscover"> </a>

## <a name="autodiscover-client-programming-considerations"></a>Considérations sur la programmation découverte automatique client

[Découverte automatique](autodiscover-for-exchange.md) fournit des informations de configuration pour les clients Exchange. Une application cliente peut découvrir ses informations de configuration d’une des trois manières, selon la cible si le client Exchange Online ou Exchange sur site. 
  
**Le tableau 1. Types de service de découverte automatique et l’application Exchange**

|**Type de service de découverte automatique**|**S'applique à**|
|:-----|:-----|
|[Découverte automatique SOAP](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online et les versions d’Exchange sur site commençant par Exchange 2010  <br/> |
|[Découverte automatique POX](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online et les versions d’Exchange sur site commençant par Exchange 2007  <br/> |
|[Recherche de point de connexion de service](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) <br/> |Versions d’Exchange sur site commençant par Exchange 2007  <br/> |
   
Outre les informations de configuration de client, que SOAP variole Autodiscover renvoyer la version du service Exchange et indiquer si le service est hébergé par Exchange Online. Ces informations sont renvoyées dans les différents éléments, selon le type de découverte automatique que vous utilisez.
  
**Le tableau 2. Éléments de découverte automatique qui renvoient la version et du service Exchange Online héberger des informations**

|**Type de service de découverte automatique**|**Élément XML qui contient la version du service**|**Élément XML qui indique si l’utilisateur possède un compte Exchange Online**|
|:-----|:-----|:-----|
|Découverte automatique SOAP  <br/> |Élément de [Paramètre (SOAP)](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) avec la valeur de texte **CasVersion** .  <br/> |Élément de [Paramètre (SOAP)](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) avec la valeur de texte **UserMSOnline** .  <br/> |
|Découverte automatique POX  <br/> |[ServerVersion (POX)](http://msdn.microsoft.com/library/2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a%28Office.15%29.aspx) <br/> |**MicrosoftOnline** <br/> |
   
Assurez-vous que votre client de capture ces informations afin qu’il peut cibler le [jeu de fonctionnalités](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md) qui est disponible sur le serveur Exchange. Cela peut être utile pour déterminer si votre client peut s’attendre un comportement différent selon si la boîte aux lettres de l’utilisateur se trouve dans un Exchange Online ou Exchange organisation locale. 

<a name="testing"> </a>

## <a name="testing-and-log-files-in-applications-that-target-exchange-online"></a>Test et les fichiers journaux dans les applications qui ciblent Exchange Online

Exchange Online ne fournit pas d’accès aux fichiers journaux du protocole EWS, les compteurs de performance EWS, service liés EWS événements et qui sont disponibles sur les serveurs Exchange locaux. Accès à ces est utile, toutefois, dans la découverte de la manière dont votre application effectue lorsqu’il interagit avec EWS. Assurez-vous que vous testez votre application contre un test ExchangeServer locaux afin que vous pouvez optimiser ses performances. Dans la mesure du possible, vous pouvez [Modifier les paramètres de limitation](http://technet.microsoft.com/en-us/library/bb232205%28v=exchg.150%29.aspx#Policies) sur votre serveur de test pour faire correspondre les paramètres de limitation pour Exchange Online, afin que vous pouvez évaluer le comporte de votre application lors de la connexion à Exchange Online. 
  
> [!TIP]
> Vous pouvez utiliser l’outil [EWSRelentless](https://ewsrelentless.codeplex.com/) pour effectuer un test de charge EWS. Vous pouvez utiliser cet outil avec un serveur de test, les journaux de protocole EWS, les compteurs de performance EWS, les événements du service et le paramètres de limitation de EWS pour mieux comprendre comment EWS effectue sous charge. 

<a name="throttling"> </a>

## <a name="throttling-settings-and-exchange-online"></a>Paramètres de limitation et Exchange Online

Les valeurs par défaut pour les [paramètres de limitation EWS](ews-throttling-in-exchange.md) sont différentes pour Exchange Online pour Exchange local. En outre, vous ne pouvez pas modifier Exchange Online, paramètres de limitation. Vous pouvez utiliser les applets de commande Exchange Management Shell pour découvrir les paramètres de limitation pour Exchange local ; Toutefois, ces applets de commande ne sont pas activés pour Exchange Online. 

<a name="ems"> </a>

## <a name="exchange-management-shell-cmdlets-and-configuration-settings"></a>Paramètres de configuration et les applets de commande Exchange Management Shell

Un nombre de cmdlets peut directement ou indirectement affectent les API du service web dans Exchange Online et Exchange sur site. Applets de commande ne sont pas disponibles pour les opérations suivantes dans Exchange Online :
  
- Paramètres de limitation 
    
- Paramètres de répertoire virtuel 
    
- Paramètres d’authentification
    
Pour plus d’informations sur les applets de commande qui sont disponibles pour Exchange Online, voir [applets de commande PowerShell dans Exchange Online](http://help.outlook.com/en-us/140/dd575549.aspx). Pour plus d’informations sur les applets de commande qui sont disponibles pour Exchange local, voir [applets de commande Exchange 2013](http://technet.microsoft.com/en-us/library/bb124413%28v=exchg.150%29.aspx).
  
## <a name="client-affinity-and-network-load-balancers"></a>Équilibreurs de charge réseau et l’affinité du client
<a name="affinity"> </a>

La plupart des communications EWS ne nécessite pas que le client de contribuer à la gestion de l’affinité avec Exchange. Les abonnements aux événements de boîte aux lettres ne nécessitent que le client fournissent les cookies et autres informations à mettre à jour l’affinité avec le serveur Exchange qui gère la file d’attente d’événements de boîte aux lettres pour un utilisateur. Exchange Server 2010 utilise l’exchangecookie pour conserver l’affinité du client entre les équilibreurs de charge réseau. Exchange Online et les versions d’Exchange sur site commençant par Exchange 2013 permet l' [en-tête X-AnchorMailbox, en-tête X-PreferServerAffinity et X-BackEndOverrideCookie cookie](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howmaintained) conserve les affinités pour les notifications de boîte aux lettres. 
  
## <a name="authentication"></a>Authentification
<a name="auth"> </a>

Clients peuvent s’authentifier avec Exchange Online à l’aide de base ou OAuth. Versions d’Exchange sur site commençant par Exchange 2013 utilisent NTLM par défaut ; Toutefois, il est possible de configurer Exchange locale pour utiliser l’authentification de base ainsi. 
  
## <a name="client-latency-diagnostics"></a>Diagnostics de latence de client
<a name="diag"> </a>

Exchange Online recueille les diagnostics de latence de client s’ils sont signalés. Cela permet de résoudre les problèmes de connectivité avec Exchange Online support Microsoft. Exchange sur site ne collecte pas les diagnostics de latence de client. Si votre client cible Exchange locale, le client ne peut pas signaler les diagnostics de latence sur le serveur.
  
## <a name="functionality-in-the-ews-managed-api"></a>API managée des fonctionnalités dans le EWS
<a name="ewsma"> </a>

L’API managée EWS expose certaines fonctionnalités spécifiques à Exchange sur site, telles que la recherche du service point de connexion et certaines fonctionnalités spécifiques à Exchange Online, tels que le rapport de latence de client. Notez qu’il est possible que certaines fonctionnalités à mettre en œuvre dans Exchange Online avant son implémentation dans l’API managée EWS. 
  
Les fonctionnalités d’API managées suivantes concernent uniquement vers Exchange Online :
  
- Rapport de latence de client
    
- Avant l’authentification de base
    
- La possibilité de demander que RequestId être renvoyées dans les réponses
    
## <a name="api-features-in-exchange-online-plans-and-exchange-server-editions"></a>Fonctionnalités d’API dans les plans Exchange Online et les éditions d’Exchange Server
<a name="exo"> </a>

Jeux de fonctionnalités différents soient disponibles dans les différents plans Office 365 et Exchange Online, ou dans les versions standard et enterprise d’Exchange Server. N’oubliez pas que certaines fonctionnalités d’API ne soit pas disponible pour votre application cliente en fonction de l’édition de Exchange Server qui héberge la boîte aux lettres d’un utilisateur ou un plan Exchange Online. 
  
**Le tableau 3. Variantes de fonctionnalité API parmi les plans et les éditions**

|**Fonctionnalité de l’API**|**Considérations relatives à la planification ou edition**|
|:-----|:-----|
|EWS accès aux comptes, sauf via l’emprunt d’identité Exchange  <br/> |Non autorisé dans le [Office 365 pour entreprises : plans Kiosk](http://office.microsoft.com/en-us/business/compare-office-365-kiosk-plans-FX103178917.aspx).  <br/> |
|Messagerie unifiée  <br/> |Disponible uniquement avec plan Office 365 entreprise (E3), Exchange Online Plan 2 et les éditions d’Exchange Server 2013 Enterprise.  <br/> |
|Intégration d’Active Directory domaine Services (AD DS)  <br/> |Non disponible avec le plan Office 365 petite entreprise et Office 365 petite entreprise Premium.  <br/> |
|Contient des Information Rights Management, d’archivage et juridiques.  <br/> |Disponible uniquement avec les plans Office 365 entreprise (E3 et E4).  <br/> |
|Protection contre les fuites de données  <br/> |Disponible uniquement avec les plans Office 365 pour entreprises, Exchange Online Plan 2 et Exchange Server 2013 Enterprise Edition.  <br/> |
   
Disponibilité des fonctionnalités pouvant changer, nous vous recommandons de vérifier les plans Exchange Online et les éditions d’Exchange Server pour évaluer la disponibilité des fonctionnalités peut-être affecter votre client. Vous pouvez également concevoir votre client pour vérifier la disponibilité des fonctionnalités à l’aide de l' [opération GetServiceConfiguration](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) ou envoyer des requêtes de test pour les opérations qui implémentent les fonctionnalités. Si la fonctionnalité n’est pas disponible, la réponse du serveur indique en tant que telles. 
  
## <a name="other-considerations"></a>Autres considérations
<a name="other"> </a>

Vous pouvez effectuer ce qui suit lors de ciblage Exchange local, mais pas Exchange Online :
  
- Créer un client qui est installé sur le serveur Exchange. 
    
- Installez les [agents de transport personnalisés](../transport-agents/transport-agents-in-exchange-2013.md) susceptibles d’affecter la remise et le contenu des messages que vous créez et envoyer avec EWS et d’autres clients. 
    
## <a name="see-also"></a>Voir aussi

- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
- [Comparaison d’Exchange Online et Exchange Server 2013](http://blogs.technet.com/b/exchange/archive/2012/09/19/comparing-exchange-online-and-exchange-server-2013.aspx)  
- [Comparer toutes les Office 365 pour les plans d’activité](http://office.microsoft.com/en-us/business/compare-all-office-365-for-business-plans-FX104051403.aspx)
- [EwsRelentless - outil de génération de chargement des EWS](https://ewsrelentless.codeplex.com/)
- [Disponibilité des fonctionnalités Web service API dans Exchange et de l'API managée EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
- [Limitation EWS dans Exchange](ews-throttling-in-exchange.md)
    

