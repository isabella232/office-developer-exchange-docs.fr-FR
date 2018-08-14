---
title: Limitation EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b4fff4c9-c625-4d2a-9d14-bb28a5da5baf
description: Découvrez les stratégies de limitation qui affectent EWS lorsque vous utilisez Exchange.
ms.openlocfilehash: 64393c173a6fc60cd4be969e8c7457d5b0109713
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354014"
---
# <a name="ews-throttling-in-exchange"></a>Limitation EWS dans Exchange

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez les stratégies de limitation qui affectent EWS lorsque vous utilisez Exchange.
  
**Auteurs :** Glen Scales ; Michael Mainer, Microsoft Corporation 
  
Cet article fournit des informations sur la limitation des services EWS dans Exchange Online, Exchange Online intégré à Office 365 et les versions locales d'Exchange à partir de la version d'Exchange 2010. La limitation dans Exchange garantit la fiabilité du serveur et la disponibilité en limitant la quantité de ressources serveur pouvant être consommées par un utilisateur ou une application. La limitation est une réponse réactive à la surutilisation de ressources système ayant un impact sur les fonctionnalités et la fiabilité du service. Exchange surveille en continu l'intégrité des ressources d'infrastructure critiques, telles que les bases de données de boîtes aux lettres. Lorsqu'il détecte que des facteurs de charge élevée dégradent les performances de ces ressources, les connexions EWS sont limitées proportionnellement au degré auquel chaque appelant a contribué à cette charge élevée. Il se peut qu'un utilisateur se trouve en dessous du seuil de limitation, mais qu'il rencontre tout de même des ralentissements jusqu'à ce que l'intégrité de la ressource soit revenue à un niveau opérationnel.
  
Chaque protocole d'accès client dans Exchange, y compris EWS, dispose d'une stratégie de limitation. Lors de la conception d'applications utilisant EWS, il est important de prendre en compte les stratégies de limitation afin de garantir la fiabilité des applications et l'intégrité de votre serveur Exchange. Cet article identifie les différentes stratégies de limitation et limites de service pour EWS, que vous cibliez Exchange Online ou les versions locales d'Exchange à partir de la version d'Exchange Server 2010. Selon le cas, cet article identifie également les différences de stratégie de limitation en fonction des versions d'Exchange.
  
> [!IMPORTANT]
> La configuration de la stratégie de limitation, de l'accès à cette stratégie et de la stratégie de limitation par défaut diffère entre Exchange Online et Exchange en local. Les valeurs spécifiques du paramètre de limitation sont applicables uniquement à une version spécifique d'Exchange. Étant donné que les valeurs du paramètre varient selon les versions et que les administrateurs Exchange peuvent modifier les stratégies de limitation par défaut pour les déploiements locaux, cet article ne fournit pas les valeurs du paramètre par défaut. Veillez surtout à tenir compte des considérations en matière de conception pour qu'une application fonctionne en dessous du seuil de limitation et réagisse correctement aux scénarios de limitation. 
  
Si vous êtes un développeur d'applications, vous devez factoriser la limitation dans la conception de votre application. Selon les versions d'Exchange, les valeurs par défaut des paramètres de limitation EWS varient. Les applications clientes et de service qui sont conçues pour accéder à différentes versions d'Exchange doivent prendre en compte ces paramètres, qu'il s'agisse de valeurs par défaut, de valeurs personnalisées définies par un administrateur Exchange ou, comme pour Exchange Online, de la valeur définie par défaut non détectable. Étant donné que les valeurs du paramètre de limitation ne peuvent pas être détectées par un programme, les spécifications de conception de votre client doivent inclure un plan permettant à l'application de s'adapter à différents seuils de limitation potentiels. Lorsque vous concevez des applications multithread qui accèdent à de nombreuses boîtes aux lettres, ou lorsque de nombreux clients accèdent à la même boîte aux lettres, prenez en compte les limites de simultanéité appliquées à Exchange par la stratégie par défaut. 
  
## <a name="throttling-policies-that-affect-ews"></a>Stratégies de limitation affectant EWS
<a name="bk_PolicyParameters"> </a>

Les stratégies de limitation d'Exchange affectent non seulement EWS, mais également toutes les connexions clientes au serveur Exchange, y compris les protocoles utilisés par Office Outlook, Outlook Web App et Exchange ActiveSync. 
  
La stratégie de limitation **CPUStartPercent** peut avoir un impact sur les performances des services EWS lors de l'exécution d'Exchange 2010. Lorsque l'utilisation moyenne de l'UC par les processus Exchange en cours d'exécution sur le serveur d'accès au client (y compris, mais sans s'y limiter, le processus EWS) dépasse la valeur spécifiée par cette stratégie, les demandes entrantes sont retardées afin de réduire l'utilisation de l'UC. Vous ne pouvez pas modifier la valeur de cette stratégie, mais le fait d'en avoir connaissance peut vous aider à résoudre les problèmes de performances. La logique d'échantillonnage effectuée par le serveur d'accès au client pour cette valeur correspond à une moyenne sur une fenêtre dynamique de 10 secondes. Cela permet au processus de répondre de manière appropriée aux pics de rapidité dans l'utilisation de l'UC. Lorsque ce seuil est dépassé, les connexions entrantes dans EWS sont retardées. Ce délai est plafonné à 500 millisecondes (ms) pour une utilisation de l'UC théorique à 100 % par demande EWS. Si une demande EWS par lot visant à obtenir 100 éléments est transmise, le serveur vérifie 100 fois l'utilisation de l'UC (une fois par élément) pendant un délai maximal de 50 secondes. Le délai est proportionnel de façon linéaire à l'utilisation de l'UC. Au niveau de **CPUStartPercent**, le délai est de 0 (rendement de thread), puis cette valeur augmente jusqu'à 500 ms lorsque l'utilisation de l'UC atteint 100 %. Étant donné que les stratégies de limitation s'appliquent à tous les utilisateurs d'Exchange, il est peu probable que l'utilisation de l'UC dépasse le seuil de **CPUStartPercent** sur un serveur d'accès au client Exchange, car l'utilisation de l'UC par les applications ou les utilisateurs individuels n'est pas suffisante pour avoir un impact sur le fonctionnement du serveur. 
  
Le tableau suivant répertorie les paramètres de stratégie de limitation qui affectent les applications utilisant EWS.
  
**Tableau 1 : Paramètres de stratégie de limitation qui affectent EWS**

|**Nom du paramètre de stratégie de limitation**|**S'applique à**|**Description**|
|:-----|:-----|:-----|
|**DiscoveryMaxConcurrency** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Indique le nombre de connexions de recherche de découverte simultanées qu'un utilisateur peut utiliser en même temps.  <br/> |
|**DiscoveryMaxKeywords** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Indique le nombre maximal de mots clés qu'un utilisateur peut inclure dans une recherche de découverte.  <br/> |
|**DiscoveryMaxKeywordsPerPage** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Indique le nombre de mots clés pour lesquels afficher des statistiques.  <br/> |
|**DiscoveryMaxMailboxes** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Indique le nombre maximal de boîtes aux lettres source qu'un utilisateur peut inclure dans une recherche de découverte.  <br/> |
|**DiscoveryMaxMailboxesResultsOnly** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Indique le nombre maximal de boîtes aux lettres dans lesquelles vous pouvez effectuer des recherches dans une recherche de découverte électronique inaltérable sans pouvoir afficher les statistiques.  <br/> |
|**DiscoveryPreviewSearchResultsPageSize** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Indique le nombre de messages renvoyés dans une réponse d'aperçu de recherche de découverte électronique.  <br/> |
|**EwsCutoffBalance** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Définit les limites de consommation de ressources pour l'utilisateur EWS avant de lui interdire complètement d'effectuer des opérations sur un composant spécifique.  <br/> |
|**EwsMaxBurst** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Définit la durée pendant laquelle un utilisateur EWS peut consommer un nombre élevé de ressources avant d'être limité. Cette valeur est mesurée en millisecondes. Cette valeur est définie séparément pour chaque composant.  <br/> |
|**EwsRechargeRate** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Définit la fréquence à laquelle le budget d'un utilisateur EWS est rechargé (budgétisation) pendant la période de budget.  <br/> |
|**EWSMaxSubscriptions** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Définit le nombre maximal d'abonnements à des notifications actives par émission de données, d'extraction et de diffusion en continu dont un utilisateur peut disposer en même temps sur un serveur d'accès au client spécifique. Ceci est budgétisé différemment en fonction des versions d'Exchange.  <br/> |
|**EWSFastSearchTimeoutInSeconds** <br/> |Exchange 2010  <br/> |Définit la durée en secondes des recherches rapides effectuées avec la recherche Exchange dans EWS avant leur délai d'expiration. Les recherches rapides sont effectuées à l'aide d'une chaîne de requête AQS (syntaxe de requête avancée) dans une [FindItem Operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).    <br/> |
|**EWSFindCountLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Définit le nombre maximal d'éléments d'une [FindItem Operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) ou [FindFolder Operation](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) qui peuvent exister en même temps dans la mémoire du serveur d'accès au client pour un utilisateur. La valeur par défaut de cette propriété est 1 000. Sa [valeur de secours](http://technet.microsoft.com/fr-FR/library/dd297964%28v=exchg.141%29.aspx#fallback) est 1 000.  <br/> Dans Exchange Online et les versions locales d'Exchange à partir de la version d'Exchange 2013, cette stratégie de limitation ne peut pas être interrogée ou configurée par une cmdlet. Dans Exchange Online et les versions à partir d'Exchange 2013, la limite EWSFindCountLimit pour une [recherche AQS](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md) et toute recherche Exchange avec restriction est de 250 résultats. Une recherche Exchange sans restriction renvoie jusqu'à 1 000 résultats.  <br/> |
|**EWSPercentTimeInAD** <br/> |Exchange 2010  <br/> |Définit le pourcentage de temps par minute où un utilisateur spécifique peut exécuter des demandes Active Directory.  <br/> |
|**EWSPercentTimeInCAS** <br/> |Exchange 2010  <br/> |Définit le pourcentage de temps par minute où un utilisateur spécifique peut exécuter le code de serveur d'accès au client.  <br/> |
|**EWSPercentTimeInMailboxRPC** <br/> |Exchange 2010  <br/> |Définit le pourcentage de temps par minute où un utilisateur spécifique peut exécuter des demandes RPC de boîte aux lettres.  <br/> |
|**EWSMaxConcurrency** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Définit le nombre de connexions ouvertes simultanées dont un utilisateur spécifique peut disposer sur un serveur Exchange qui utilise EWS. La valeur par défaut pour Exchange 2010 est 10. La valeur par défaut pour Exchange 2013 et Exchange Online est 27.  <br/> Cette stratégie s'applique à toutes les opérations à l'exception des notifications de diffusion en continu. Les notifications de diffusion en continu utilisent la limite **HangingConnectionLimit** pour indiquer le nombre de connexions ouvertes d'événements de diffusion en continu qui sont disponibles. Pour plus d'informations, consultez la section ayant trait aux [Les valeurs de limitation ai-je besoin de prendre en considération ?](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).  <br/> |
|**MessageRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Définit le nombre de messages pouvant être envoyés par minute.  <br/> |
|**RecipientRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Définit le nombre maximal de destinataires auxquels un utilisateur peut adresser des messages sur une période de 24 heures.  <br/> |
|**ForwardeeLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Définit le nombre maximal de destinataires pour les actions de transfert/redirection de la boîte de réception sur une période de 24 heures.  <br/> |
   
> [!CAUTION]
> Ne définissez pas de stratégie de limitation sur **null**. Sinon, la stratégie est définie comme illimitée, ce qui signifie qu'aucune stratégie de limitation n'est définie. 
  
## <a name="displaying-the-policies-that-apply-to-exchange-mailboxes"></a>Affichage des stratégies qui s'appliquent aux boîtes aux lettres Exchange
<a name="bk_PolicyCmdlets"> </a>

Vous pouvez utiliser les cmdlets de l'environnement de ligne de commande Exchange Management Shell fournies par Exchange en local pour définir et obtenir une stratégie de limitation. Exchange Online ne fournit pas l'accès aux cmdlets de stratégie de limitation.
  
Vous pouvez utiliser les cmdlets suivantes pour afficher les stratégies de limitation pour un déploiement Exchange Server local :
  
- **Get-ThrottlingPolicy**: permet d'obtenir les paramètres de limitation des clients pour une ou plusieurs stratégies de limitation. Pour plus d'informations, reportez-vous à la rubrique [Get-ThrottlingPolicy](http://technet.microsoft.com/fr-FR/library/dd351264.aspx) de TechNet. 
    
- **Get-ThrottlingPolicyAssociation**: permet d'afficher la relation entre un objet et ses stratégies de limitation associées. L'objet peut être un utilisateur avec ou sans boîte aux lettres, ou un contact. Pour plus d'informations, reportez-vous à la rubrique [Get-ThrottlingPolicyAssociation](http://technet.microsoft.com/fr-FR/library/ff459241.aspx) de TechNet. 
    
Utilisez la commande suivante pour afficher la stratégie de limitation par défaut pour Exchange 2010.
  
**Get-ThrottlingPolicy | Where-Object {$_.IsDefault -eq "True"} | format-list**
  
Utilisez la commande suivante pour afficher la stratégie de limitation globale pour Exchange 2013 (ce qui correspond à la stratégie de limitation par défaut dans Exchange 2010).
  
**Get-ThrottlingPolicy | Where-Object {$_.ThrottlingPolicyScope -eq "Global"} | format-list**
  
Utilisez la commande suivante pour afficher la stratégie de limitation associée à un utilisateur dans Exchange 2010 ou Exchange 2013. Remplacez le nom d'utilisateur john@contoso.com par le nom d'utilisateur cible pour lequel vous souhaitez obtenir des informations sur la stratégie de limitation.
  
**Get-ThrottlingPolicyAssociation john@contoso.com | format-list**
  
L'exécution de cette commande dans l'environnement de ligne de commande Exchange Management Shell entraîne un résultat semblable à ce qui suit.
  
```powershell
PS C:\>Get-ThrottlingPolicyAssociation john@contoso.com
RunspaceId               : 72153d6-9dce-2fae-8dbd-5ca5f760g2df
ObjectId                 : john
ThrottlingPolicyId       :
Name                     : john
Identity                 : FHXB-28178dom.contoso.com/Users/john
IsValid                  : True
NeedsToSuppressPii       : False
ExchangeVersion          : 0.10 (15.0.0.0)
DistinguishedName        : CN=john,CN=Users,DC=FHXB-28178dom,DC=contoso,DC=com
Guid                     : 2c10dab6-de28-1937-ad8g-535832613a08
```

> [!NOTE]
> Lorsque la propriété **ThrottlingPolicyId** est vide, la stratégie par défaut s'applique à la boîte aux lettres. 
  
Vous pouvez définir une stratégie de limitation sur un serveur Exchange à l'aide des cmdlets [Set-ThrottlingPolicy](http://technet.microsoft.com/fr-FR/library/dd298094.aspx) et [Set-ThrottlingPolicyAssociation](http://technet.microsoft.com/fr-FR/library/ff459231.aspx). Vous pouvez créer et supprimer des stratégies de limitation autres que celles par défaut en utilisant les cmdlets [New-ThrottlingPolicy](http://technet.microsoft.com/fr-FR/library/dd351045.aspx) et [Remove-ThrottlingPolicy](http://technet.microsoft.com/fr-FR/library/dd351178.aspx) . 
  
> [!TIP]
> Nous vous recommandons de concevoir vos applications de sorte qu'elles adhèrent à la stratégie de limitation par défaut. Apportez des modifications aux stratégies de limitation uniquement si la conception de votre application cliente ne peut pas s'ajuster à la stratégie par défaut. N'oubliez pas que moins les stratégies de limitation sont restrictives, plus elles risquent d'avoir une incidence négative sur la fiabilité du service. 

<a name="bk_ThrottlingConsiderations"> </a>

## <a name="throttling-considerations-for-applications-that-use-ews-impersonation"></a>Observations à propos de la limitation pour les applications qui utilisent l’emprunt d’identité EWS


L'[emprunt d'identité](impersonation-and-ews-in-exchange.md) est une méthode d'autorisation qui permet à un seul compte d'accéder à de nombreux comptes. Lorsqu'un compte de service emprunte l'identité d'utilisateurs, il agit en tant qu'utilisateur et assume donc les droits qui sont affectés à ces utilisateurs. Les fichiers journaux enregistrent l'accès en tant qu'utilisateur dont l'identité a été empruntée. Les administrateurs utilisent le contrôle d'accès en fonction du rôle (RBAC) pour configurer l'emprunt d'identité via l'environnement de ligne de commande Exchange Management Shell. 
  
Lorsque l'emprunt d'identité est utilisé, les budgets de tous les seuils de limitation s'appliquent différemment selon la version d'Exchange. Le budget est calculé en fonction du compte qui est emprunté ou du compte de service. Si votre application est multithread et effectue des demandes simultanées sur plusieurs boîtes aux lettres, vous devez envisager la façon dont le seuil de limitation affecte les performances de l'application. En règle générale, vous devez avoir connaissance des seuils suivants sur les comptes de service lorsque vous créez une application de service qui utilise l'emprunt d'identité pour accéder à toutes les boîtes aux lettres : 
  
- Lorsque vous utilisez l'emprunt d'identité, le compte de service a un budget distinct pour les paramètres de stratégie suivants :
    
  - **EWSMaxConcurrency**
    
  - **EWSPercentTimeInAD**
    
  - **EWSPercentTimeInCAS**
    
  - **EWSPercentTimeInMailboxRPC**
    
  - **EWSMaxSubscriptions**
    
  - **EWSFastSearchTimeoutInSeconds**
    
  - **EWSFindCountLimit**
    
- Le budget **EWSMaxConcurrency** est partagé entre le compte de service et le compte dont l'identité est empruntée pour toutes les connexions de versions d'Exchange antérieures au correctif cumulatif 4 (RU4) pour Exchange 2010 Service Pack 2 (SP2). À compter d'Exchange 2010 SP2 RU4 (y compris Exchange Online), l'accès au compte de service utilise un budget distinct du budget **EWSMaxConcurrency** de l'utilisateur. Pour plus d'informations sur la mise à jour de la stratégie de limitation de la connexion simultanée Exchange pour EWS, reportez-vous à [Description du correctif cumulatif 4 pour Exchange Server 2010 Service Pack 2](http://support.microsoft.com/kb/2706690).
    
    Dans les versions d'Exchange à compter d'Exchange 2010 (y compris Exchange Online), les notifications de diffusion en continu ont un budget **EWSMaxConcurrency** supplémentaire cloné à partir de toutes les autres connexions clientes EWS. Les connexions de notification de diffusion en continu sont prises en compte en fonction d'un budget distinct par rapport à toutes les autres opérations EWS. Le budget de simultanéité maximale des notifications en continu est constitué en réalité de deux budgets différents : l'un est réservé à tous les comptes de service et l'autre est réservé au compte dont l'identité est empruntée. Dans Exchange Online et les versions d'Exchange à compter d'Exchange 2013, les notifications de diffusion en continu utilisent la limite [HangingConnectionLimit](ews-throttling-in-exchange.md#bk_ThrottlingNotifications) pour restreindre le nombre de connexions. 
    
    Par exemple, supposons que la valeur de **EWSMaxConcurrency** est égale à cinq. Un utilisateur peut alors disposer de cinq connexions ouvertes de notification d'extraction, tandis qu'un compte de service peut disposer de cinq connexions simultanées de notification d'extraction sur la boîte aux lettres de l'utilisateur en même temps que ce dernier. 
    
- Le tableau suivant identifie la façon dont les budgets de limitation **EWSMaxSubscriptions** sont calculés entre le compte de service et le compte auquel emprunter l'identité. 
    
   **Tableau 2 : Gestion du budget EWSMaxSubscriptions**

   |**Version d’Exchange**|**Gestion du budget de limitation EWSMaxSubscriptions**|
   |:-----|:-----|
   |Exchange Online  <br/> |Facturé en fonction de la boîte aux lettres cible.  <br/> |
   |Exchange 2013  <br/> |Facturé en fonction de la boîte aux lettres cible.  <br/> |
   |Exchange 2010 SP3  <br/> |Facturé en fonction de la boîte aux lettres cible.  <br/> |
   |Exchange 2010 SP2  <br/> |Facturé en fonction du compte d'appel. À compter d'Exchange 2010 SP2 RU4, le budget est facturé en fonction de la boîte aux lettres cible.  <br/> |
   |Exchange 2010 SP1  <br/> |Facturé en fonction du compte d'appel.  <br/> |
   |Exchange 2010  <br/> |Facturé en fonction du compte d'appel.  <br/> |
   
- Étant donné que le budget de limitation **EWSMaxSubscriptions** est facturé en fonction du compte dont l'identité est empruntée, il n'existe aucune limite relative au nombre de boîtes aux lettres auxquelles un compte de service peut s'abonner et à partir desquelles il peut recevoir des notifications de diffusion en continu, tant que l'emprunt d'identité est en cours. Pour le compte dont l'identité est empruntée, vous ne pouvez pas disposer de plus de  _n_ demandes simultanées par boîte aux lettres cible, où  _n_ correspond à la valeur de **EWSMaxSubscriptions**. Si vous n'utilisez pas l'emprunt d'identité, le même compte de service ne peut pas disposer de plus de  _n_ demandes simultanées en tout. Par conséquent, en utilisant l’emprunt d’identité avec un compte de service, vous augmentez de manière exponentielle le nombre de boîtes aux lettres que vous pouvez activer. Pour plus d'informations, voir[Maintenir l'affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md).
    
- Les paramètres de stratégie **EWSPercentTimeInMailboxRPC**, **EWSPercentTimeInCAS** et **EWSPercentTimeInAD** font référence à des actions effectuées par un thread unique. Lorsqu'une application effectue plusieurs opérations simultanément, vous devez tenir compte de l'effet cumulé de ces opérations sur le budget de ressources de l'utilisateur. 
    
## <a name="throttling-implications-for-ews-batch-requests"></a>Implications de la limitation pour les demandes de lot EWS
<a name="bk_ThrottlingBatch"> </a>

EWS permet de traiter en lots plusieurs demandes d'éléments dans une seule demande exécutée par le serveur d'accès au client. Cela permet d'améliorer l'efficacité et les performances. Lorsqu'un serveur Exchange exécute une demande par lot, il vérifie le budget de l'utilisateur après l'exécution de chaque élément contenu dans le lot. Si l'application dépasse le budget, le traitement de l'élément suivant dans le lot est retardé jusqu'à ce que le budget soit rechargé pour cet utilisateur. Pour vous assurer que les applications qui utilisent des opérations par lot ont été exécutées correctement, limitez le nombre de demandes d'élément pouvant être incluses dans un lot et divisez les lots volumineux en plusieurs petits lots afin d'augmenter la fiabilité des résultats. L'effet d'une opération par lot sur des seuils de limitation spécifiques varie selon le type de la demande, la taille des éléments à traiter (par exemple, dans les opérations **UploadItems** ou **ExportItems** ) et le contenu de la boîte aux lettres. Les stratégies de limitation affectent les opérations en lots en ralentissant le traitement de la demande. Par conséquent, l'appelant doit attendre plus longtemps avant d'obtenir la réponse et, sachant que les services EWS limitent à une minute la durée d'exécution d'une demande de lot, il se peut que l'appel expire. 
  
Pour déterminer la taille de lot optimale pour une application, effectuez un test unitaire avec plusieurs ensembles de valeurs d'entrée pour vous assurer que l'application ne rencontre aucune erreur dans un environnement de production. 
  
## <a name="throttling-policy-parameters-that-affect-ews-search-operations"></a>Paramètres de stratégie de limitation qui affectent les opérations de recherche EWS
<a name="bk_ThrottlingSearch"> </a>

Les [opérations de recherche dans EWS](search-and-ews-in-exchange.md) peuvent consommer beaucoup de temps et de ressources, en fonction de la manière dont la recherche est exécutée et du type d'informations requises. Pour contrôler l'utilisation des ressources lors des recherches, deux paramètres de stratégie sont utiles : **EWSFastSearchTimeoutInSeconds** et **EWSFindCountLimit**. 
  
Le paramètre de stratégie **EWSFastSearchTimeoutInSeconds** spécifie la durée, en secondes, d'exécution des recherches rapides EWS (également appelées recherche d'indexation de contenu) avant expiration. Une recherche rapide est effectuée à l'aide d'une chaîne de requête AQS (syntaxe de requête avancée) dans une [FindItem Operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).
  
Vous pouvez effectuer une recherche dans un dossier de boîte aux lettres Exchange des deux manières suivantes :
  
- En effectuant une recherche dans la banque d'informations Exchange, qui effectue une analyse séquentielle de tous les messages dans la zone de recherche cible.
    
- En utilisant le service de recherche Exchange (indexation de contenu).
    
Ces deux types de recherches peuvent entraîner des délais d'attente. Si possible, utilisez le service de recherche Exchange, car ces recherches sont souvent ciblées par rapport aux index de la boîte aux lettres et utilisent des requêtes AQS. L'exemple suivant indique comment effectuer une recherche AQS dans la boîte de réception en utilisant EWS et le service de recherche Exchange.
  
```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiitems = service.FindItems(WellKnownFolderName.Inbox, "subject:football", iv);
```

Si vous ne pouvez pas utiliser une recherche AQS, évitez d'utiliser des filtres de recherche trop complexes. Essayez également d'éviter de créer des filtres de recherche reposant sur des valeurs calculées si la requête implique des propriétés MAPI étendues. La recherche ASQ est une nouveauté d'Exchange 2010.
  
> [!NOTE]
> La première fois que vous exécutez une requête de recherche complexe dans la banque d'informations Exchange, celle-ci est très lente et risque d'expirer. Par la suite, la requête répond plus rapidement. Pour plus d'informations sur les processus du serveur principal Exchange qui se produisent lors des requêtes de recherche dans la banque d'informations Exchange, consultez la rubrique [Impact sur les performances des nombres élevés d'éléments et des affichages restreints](http://technet.microsoft.com/fr-FR/library/cc535025%28EXCHG.80%29.aspx) sur TechNet. L'utilisation d'un **SearchFilter** crée une restriction dynamique qui est utile pour des requêtes semblables à l'avenir, mais ces restrictions étant dynamiques par nature, elles ne sont ni permanentes ni fiables, et sont supprimées au bout de trois jours maximum. 
  
Le paramètre de stratégie **EWSFindCountLimit** indique le nombre maximal d'éléments provenant des résultats d'une opération **FindItem** ou **FindFolder** pouvant exister simultanément en mémoire sur un serveur d'accès au client pour un utilisateur. Chaque élément ou dossier traité par EWS dans une demande **FindItem** ou **FindFolder** est pris en compte en fonction du budget spécifié dans l'élément **EWSFindCountLimit**. Lorsque la réponse est renvoyée au demandeur, les frais relatifs au nombre de recherches pour l'appel en cours sont publiés. La réponse renvoyée à un demandeur par le serveur lorsque le budget est dépassé dépend de la valeur de l'élément **RequestServerVersion** et de la spécification ou non d'une pagination par le demandeur. Lorsque la valeur de l'élément **RequestServerVersion** indique Exchange 2010 ou une version antérieure d'Exchange, le serveur envoie une réponse d'échec avec le code d'erreur **ErrorServerBusy**. Si la valeur de l'élément **RequestServerVersion** indique une version d'Exchange à partir d'Exchange 2010 SP1 ou d'Exchange Online et si le client utilise la pagination, EWS peut renvoyer un ensemble de résultats partiel plutôt qu'une erreur. Votre application doit s'attendre à ce qu'EWS ne renvoie pas tous les éléments. Si la valeur de l'élément **IncludesLastItemInRange** est False, l'application doit effectuer une autre demande **FindItem** ou **FindFolder** avec le nouveau décalage, jusqu'à ce que l'élément **IncludesLastItemInRange** renvoie la valeur True. 
  
Lorsque vous utilisez une opération **FindItem** ou **FindFolder**, il est important d'utiliser la pagination. L'API managée EWS impose l'utilisation de la pagination, mais si vous utilisez d'autres méthodes, comme les objets proxy EWS ou SOAP brut, vous devez définir la pagination de manière explicite. L'exemple suivant montre comment utiliser la pagination dans l'API managée EWS. 
  
```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiFindItemResults = service.FindItems(WellKnownFolderName.Inbox, iv);
```

> [!NOTE]
> La stratégie par défaut dans Exchange limite la taille de page à 1 000 éléments. La définition d'une taille de page sur une valeur supérieure à celle-ci n'a aucun effet pratique. 
  
Les applications doivent également tenir compte du fait que la valeur du paramètre de limitation  _EWSFindCountLimit_ peut entraîner le renvoi d'un ensemble de résultats partiel pour les applications qui effectuent des demandes simultanées. L'exemple suivant montre comment utiliser la propriété **MoreAvailable** dans l'API managée EWS pour vous assurer que tous les résultats sont inclus dans une demande. 
  
```cs
ItemView iv = new ItemView(1000);
service.TraceEnabled = false;
FindItemsResults<Item> fiResults = null;
Do 
{
    fiResults = service.FindItems(WellKnownFolderName.Inbox, iv);
    PropertySet itItemPropSet = new PropertySet(BasePropertySet.IdOnly) { EmailMessageSchema.Body };
    //Process Items in Result Set
    iv.Offset += fiResults.Items.Count;
}
while (fiResults.MoreAvailable == true);
```

## <a name="throttling-policies-and-concurrency"></a>Stratégies de limitation et simultanéité
<a name="bk_ThrottlingConcurrency"> </a>

La simultanéité fait référence au nombre de connexions provenant d'un utilisateur spécifique. Une connexion est maintenue de la réception d'une demande à l'envoi d'une réponse au demandeur. Si les utilisateurs essaient d'effectuer plus de demandes simultanées qu'autorisé par leur stratégie, la nouvelle tentative de connexion échoue. Toutefois, les connexions existantes restent valides. Les stratégies de limitation peuvent affecter la simultanéité de nombreuses façons différentes.
  
Le paramètre de stratégie de limitation **EWSMaxConcurrency** définit le nombre de connexions simultanées dont un utilisateur spécifique peut disposer sur un serveur Exchange. Pour déterminer le nombre maximal de connexions simultanées à autoriser, prenez en compte les connexions utilisées par les clients Outlook. Outlook 2007 et Outlook 2010 utilisent EWS pour accéder aux informations relatives à la disponibilité et à l'absence du bureau (OOF). Outlook 2011 sur Mac utilise EWS pour toutes les fonctionnalités d'accès au client. En fonction du nombre de clients Outlook qui se connectent activement à la boîte aux lettres d'un utilisateur, le nombre de connexions simultanées disponibles par utilisateur peut être limité. En outre, si votre application doit se connecter simultanément à plusieurs boîtes aux lettres lors de l'utilisation d'un contexte de sécurité unique, il est important de prendre en compte la valeur de la stratégie **EWSMaxConcurrency**. Pour plus d'informations sur l'utilisation d'un contexte de sécurité unique avec des connexions simultanées, consultez la section [Considérations relatives à la limitation pour les applications qui utilisent l'emprunt d'identité EWS](#bk_ThrottlingConsiderations) plus haut dans cet article. 
  
Les applications qui se connectent simultanément à plusieurs boîtes aux lettres doivent pouvoir effectuer le suivi de l'utilisation des ressources côté client. Les opérations EWS reposant sur le principe de demande/réponse, vous pouvez vérifier que vos applications fonctionnent bien en dessous du seuil **EWSMaxConcurrency** via le suivi du nombre de connexions existantes entre le début d'une demande et la réception de la réponse, en vous assurant qu'un maximum de dix demandes ouvertes sont effectuées simultanément. 
  
Le paramètre de stratégie **EWSFindCountLimit** indique la taille maximale des résultats qu'une opération **FindItem** ou **FindFolder** peut utiliser en même temps sur un serveur d'accès au client pour un utilisateur. Si une application (ou potentiellement plusieurs applications) effectue deux demandes **FindItem** EWS simultanées qui renvoient 100 éléments chacune pour un utilisateur spécifique, les frais **EWSFindCountLimit** par rapport au budget de cet utilisateur spécifique sont de 200. Lorsque la première requête est renvoyée, le budget passe à 100 et lorsque la deuxième requête est renvoyée, le budget passe à zéro. Si la même application effectue deux demandes simultanées pour 1 000 éléments, la valeur de budget est de 2 000 éléments, ce qui dépasse la valeur de **EWSFindCountLimit**. Si le budget de l'utilisateur pour les éléments devient inférieur à zéro, la demande suivante entraîne une erreur jusqu'à ce que le budget soit rechargé. 

<a name="bk_ThrottlingNotifications"> </a>
  
## <a name="throttling-considerations-for-ews-notification-applications"></a>Observations à propos de la limitation pour les applications de notification EWS


Si vous créez des applications EWS qui utilisent des notifications Push, d'extraction ou de diffusion en continu, vous devez tenir compte des implications des stratégies de limitation **EWSMaxSubscriptions** et **EWSMaxConcurrency**, ainsi que de la limite **HangingConnectionLimit**. 
  
Le paramètre de stratégie **EWSMaxSubscriptions** indique le nombre maximal d'abonnements actifs par émission de données, par extraction et par diffusion en continu dont peut disposer simultanément un utilisateur sur un serveur d'accès au client spécifique. Selon les versions d'Exchange, les valeurs par défaut pour ce paramètre varient. Un utilisateur peut s'abonner à tous les dossiers d'une boîte aux lettres à l'aide de la propriété **SubscribeToAllFolders**. Cela correspond à un seul abonnement par rapport au budget **EWSMaxSubscriptions**. Les utilisateurs peuvent s'abonner à des dossiers individuels, auquel cas chaque abonnement à un dossier est comptabilisé dans le budget **EWSMaxSubscriptions**, jusqu'à la limite définie par la valeur du paramètre **EWSMaxSubscriptions** (par exemple, les utilisateurs peuvent s'abonner à 20 dossiers de calendrier dans différentes boîtes aux lettres si le paramètre **EWSMaxSubscriptions** est défini sur 20). 
  
Pour plus d'informations sur l'emprunt d'identité et le paramètre **EWSMaxSubscriptions**, consultez la section [Considérations relatives à la limitation pour les applications qui utilisent l'emprunt d'identité EWS](#bk_ThrottlingConsiderations) plus haut dans cet article. 
  
Le paramètre de stratégie **EWSMaxConcurrency** peut également représenter un problème pour les notifications EWS, par exemple : 
  
- Quand EWS incrémente le nombre de connexions pour le titulaire de l'abonnement alors que la notification est générée par un abonnement par émission de données.
    
- Quand une application est conçue de manière à écouter les boîtes aux lettres de plusieurs utilisateurs et que les utilisateurs reçoivent des notifications simultanées pour une instance d'un message qui est envoyé à une liste de distribution.
    
S'il s'agit d'une application de notifications multithread qui effectue des demandes de connexion simultanées afin d'obtenir plus d'informations sur un message spécifique reçu par un compte d'utilisateur, la limite de stratégie **EWSMaxConcurrency** peut être dépassée. Pour parer cette éventualité, pensez à surveiller les connexions simultanées de votre application (y compris celles pouvant être utilisées par le serveur) et à implémenter la mise en file d'attente des demandes sur le client. 
  
Le paramètre **HangingConnectionLimit** est valable uniquement pour les notifications de diffusion en continu. Cette limite est définie dans le fichier web.config, ce qui signifie qu'un administrateur Exchange peut définir cette valeur sur un serveur Exchange local, mais que les boîtes aux lettres Exchange Online doivent utiliser la valeur par défaut de cette limite, qui est de 3 pour Exchange Online et Exchange 2013. Pour en savoir plus, consultez la rubrique relative aux [Les valeurs de limitation ai-je besoin de prendre en considération ?](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).
  
## <a name="throttling-policy-and-application-performance"></a>Stratégie de limitation et performances d'application
<a name="bk_PercentTimeIn"> </a>

Les trois paramètres suivants de la stratégie de limitation **PercentTimeIn** affectent la durée qu'une application EWS peut consommer sur un serveur d'accès au client : 
  
- **EWSPercentTimeInAD**
    
- **EWSPercentTimeInCAS**
    
- **EWSPercentTimeInMailboxRPC**
    
Les valeurs indiquées dans les paramètres de stratégie **PercentTimeIn** indiquent le temps alloué à un thread pour effectuer une demande. Par exemple, en supposant que la valeur de **EWSPercentTimeInCAS** soit 90, si un processus effectue deux demandes simultanées qui ont besoin de 54 secondes chacune pour exécuter le code sur le serveur d'accès au client, le processus utilise 108 secondes dans une fenêtre de 60 secondes. Cela correspond à une valeur du paramètre **EWSPercentTimeInCAS** de 180 %. 
  
> [!NOTE]
> La valeur du paramètre **EWSPercentTimeInCAS** correspond à un sur-ensemble superposé des valeurs des paramètres **EWSPercentTimeInAD** et **EWSPercentTimeInMailboxRPC**. Cela signifie que la dépense de temps de traitement dans le serveur d'accès au client est toujours supérieure à la dépense de temps dans **EWSPercentTimeInAD** et **EWSPercentTimeInMailboxRPC**. En effet, pour que le composant Exchange puisse effectuer un appel RPC ou Active Directory, il doit déjà être en train d'exécuter le code de serveur d'accès au client. En outre, les dépenses de temps de traitement pour **EWSPercentTimeInCAS** ne sont pas interrompues lors de l'émission d'appels LDAP ou RPC. Bien que la demande puisse être en attente d'une réponse des services de domaine Active Directory (AD DS) ou de la banque d'informations Exchange de manière synchrone, le processus continue à consommer un thread sur le serveur et le thread doit donc continuer à être facturé pour cette utilisation. 
  
La quantité de temps processeur qu'une application utilise dans une période de 60 secondes peut dépasser ces seuils de limitation. Par conséquent, il est important de prendre en compte le volume et le type de demandes émises. Par exemple, si des opérations **ResolveNames** sont effectuées simultanément par lot important, la valeur du paramètre de stratégie **EWSPercentTimeInAD** peut être dépassée. Les valeurs de stratégie contenues dans la stratégie de limitation par défaut sont conçues pour permettre à la plupart des applications EWS de fonctionner sans problème. Toutefois, lorsque des applications multithread de volume élevé émettent un grand nombre de demandes sur un serveur d'accès au client spécifique, cela peut générer des problèmes. Pour éviter cela, envisagez de limiter la taille des lots à exécuter sur le serveur. 
  
## <a name="throttling-policies-and-applications-that-send-a-large-volume-of-email"></a>Stratégies de limitation et applications qui envoient une quantité élevée de messages électroniques
<a name="bk_RateLimits"> </a>

Les stratégies de limitation par défaut incluent trois paramètres de stratégie de limitation du débit pouvant affecter les applications qui utilisent EWS pour envoyer un volume élevé de messages ou pour envoyer des messages par lot important sur une courte période de temps. 
  
> [!NOTE]
> En général, il n'est pas recommandé d'utiliser EWS pour envoyer des messages électroniques en nombre. Utilisez un hôte SMTP, spécialisé dans les services de courrier en nombre pour envoyer fréquemment des messages électroniques volumineux en nombre. 
  
Le paramètre de stratégie **MessageRateLimit** indique le nombre de messages pouvant être envoyés par minute par tout client Exchange, y compris EWS. Par défaut, cette stratégie est définie sur 30 messages par minute. Pour les utilisateurs ordinaires, cette quantité est généralement suffisante. Toutefois, les applications qui envoient des lots importants de messages électroniques, par exemple dans le cadre d'un programme de facturation, peuvent rencontrer des problèmes. Lorsque la limite définie pour cette stratégie est dépassée, la remise des messages est retardée pour la boîte aux lettres. Plus précisément, les messages s'affichent plus longtemps dans le dossier Boîte d'envoi ou Brouillons lorsqu'un utilisateur ou une application envoie un nombre de messages plus élevé que la valeur spécifiée par le paramètre **MessageRateLimit**. Pensez-y lorsque vous développez un système de suivi pour la remise des messages, notamment si votre application utilise une boîte aux lettres à laquelle les utilisateurs se connectent via Outlook. Lorsque des éléments différés sont stockés dans le dossier Boîte d'envoi ou Brouillons, les utilisateurs peuvent l'interpréter comme une erreur. 
  
Le paramètre de stratégie **RecipientRateLimit** indique la limite relative au nombre de destinataires auxquels un utilisateur peut adresser des messages sur une période de 24 heures. Par exemple, si cette valeur est définie sur 500, cela signifie qu'un seul compte de boîte aux lettres Exchange peut envoyer des messages à un maximum de 500 destinataires par jour. Cette limite s'applique aux messages envoyés à des destinataires tant internes qu'externes à l'organisation. Cette limite par défaut risque d'entraîner des problèmes pour certaines applications métier qui réalisent des exécutions de facturation de fin de mois et qui doivent envoyer des messages à plus de destinataires que le nombre défini. Pour éviter cette limitation, vous pouvez utiliser des services externes permettant le traitement par lot de messages ou des solutions locales distinctes de relais de messagerie sortant. 
  
Le paramètre de stratégie **ForwardeeLimit** indique le nombre maximal de destinataires auxquels les messages peuvent être transférés ou vers lesquels ils peuvent être redirigés à l'aide de règles de boîte de réception. Ce paramètre ne limite pas le nombre de messages pouvant être transférés ou redirigés vers les destinataires. 
  
## <a name="errors-generated-when-throttling-limits-are-exceeded"></a>Erreurs générées lorsque les seuils de limitation sont dépassés
<a name="bk_ThrottlingErrors"> </a>

Lorsque les stratégies de limitation sont dépassées, EWS génère l'une des erreurs répertoriées dans le tableau suivant.
  
**Tableau 3 : Erreurs de seuil de limitation**

|**Erreur**|**Paramètre de stratégie de limitation**|**Description**|
|:-----|:-----|:-----|
|ErrorExceededConnectionCount  <br/> |**EWSMaxConcurrency** <br/> |Indique que le nombre de demandes simultanées sur le serveur dépasse la limite autorisée par la stratégie de l'utilisateur.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |**EWSMaxSubscriptions** <br/> |Indique que le nombre maximal d'abonnements défini par une stratégie de limitation d'un utilisateur a été dépassé.  <br/> |
|ErrorExceededFindCountLimit  <br/> |**EWSFindCountLimit** <br/> |Indique qu'un appel d'opération de recherche a dépassé le nombre total d'éléments pouvant être renvoyés.  <br/> |
|ErrorServerBusy  <br/> |**EWSPercentTimeInMailboxRPC**         **EWSPercentTimeInCAS**         **EWSPercentTimeInAD** <br/> |Survient lorsque le serveur est occupé. La valeur de BackOffMilliseconds renvoyée avec les erreurs ErrorServerBusy indique au client la durée d'attente nécessaire avant de soumettre à nouveau la demande qui est à l'origine de la réponse qui a renvoyé ce code d'erreur.  <br/> |
   
Le tableau suivant répertorie les codes d'état HTTP renvoyés par les erreurs de limitation.
  
**Tableau 4 : Codes d'état HTTP renvoyés par les erreurs de limitation**

|**Code d'état HTTP**|**Description**|
|:-----|:-----|
|HTTP 503  <br/> |Indique que les demandes EWS sont mises en file d'attente avec IIS. Le client doit retarder l'envoi de demandes supplémentaires à une date ultérieure.  <br/> |
|HTTP 500  <br/> |Indique une erreur de serveur interne avec le code d'erreur ErrorServerBusy. Cela indique que le client doit retarder l'envoi de demandes supplémentaires à une date ultérieure. La réponse peut contenir une indication d'interruption appelée BackOffMilliseconds. Le cas échéant, la valeur de BackOffMilliseconds doit être utilisée comme durée nécessaire avant que le client ne soumette à nouveau une demande.  <br/> |
|HTTP 200  <br/> |Contient une réponse d'erreur basée sur le schéma EWS avec le code d'erreur ErrorInternalServerError. Le code d'erreur ErrorServerBusy interne peut être présent. Cela indique que le client doit retarder l'envoi de demandes supplémentaires à une date ultérieure.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Gestion de la charge de travail Exchange](http://technet.microsoft.com/fr-FR/library/jj150503.aspx)
- [Cmdlet New-ThrottlingPolicy](http://technet.microsoft.com/fr-FR/library/dd351045.aspx)
- [Présentation des stratégies de limitation du client](http://technet.microsoft.com/fr-FR/library/dd297964.aspx)
- [Classe ThrottlingPolicy](http://msdn.microsoft.com/fr-FR/library/ff342496%28v=EXCHG.140%29.aspx)
- [Stratégies de limitation et limite EWSFindCountLimit](http://blogs.msdn.com/b/exchangedev/archive/2010/03/12/throttling-policies-and-the-ewsfindcountlimit.aspx)
- [Captures instantanées du budget dans les journaux IIS](http://blogs.msdn.com/b/exchangedev/archive/2010/03/10/budget-snapshots-in-the-iis-logs.aspx)
- [Effets de la limitation sur votre déploiement dans Exchange 2010 SP1](http://msexchangeteam.com/archive/2010/08/27/456040.aspx)
- [Associations de stratégies de limitation dans Exchange 2010 SP1](http://msexchangeteam.com/archive/2010/08/02/455707.aspx)
- [Stratégies de limitation et CPUStartPercent](http://blogs.msdn.com/b/exchangedev/archive/2010/03/11/throttling-policies-and-cpustartpercent.aspx)
- [Emprunt d'identité et EWS dans Exchange](impersonation-and-ews-in-exchange.md)
    

