---
title: Limitation EWS dans Exchange
manager: sethgros
ms.date: 05/10/2019
ms.audience: Developer
ms.assetid: b4fff4c9-c625-4d2a-9d14-bb28a5da5baf
description: Découvrez les stratégies de limitation qui affectent EWS lorsque vous utilisez Exchange.
localization_priority: Priority
ms.openlocfilehash: 27db12c01180abbaf92b5b9a09a072212b6012ec
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012551"
---
# <a name="ews-throttling-in-exchange"></a>Limitation EWS dans Exchange

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez les stratégies de limitation qui affectent EWS lorsque vous utilisez Exchange.

**Auteurs :** Glen Scales ; Michael Mainer, Microsoft Corporation

The article provides information about EWS throttling in Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with Exchange 2010. Throttling in Exchange helps to ensure server reliability and uptime by limiting the amount of server resources that a single user or application can consume. Throttling is a reactive response to overuse of system resources that may affect service reliability and functionality. Exchange constantly monitors the health of critical infrastructure resources, such as mailbox databases. When high load factors are detected that degrade the performance of these resources, EWS connections are throttled proportionally based on the amount that each caller has contributed to this high load condition. The result is that a user may be within their throttling limit and still experience slowdowns until the health of the resource is back to operational levels.

Each client access protocol in Exchange, including EWS, has a throttling policy. When you design applications that use EWS, it is important to account for throttling policies, to help ensure application reliability and the health of your Exchange server. This article identifies the different throttling policies and service limits for EWS, whether you are targeting Exchange Online or versions of Exchange on-premises starting with Exchange Server 2010. As applicable, this article also identifies differences in throttling policies in different versions of Exchange.

> [!IMPORTANT]
> Default throttling policy, access to throttling policy, and throttling policy configuration differs between Exchange Online and Exchange on-premises. Specific throttling setting values are only accurate for a specific version of Exchange. Because setting values vary across versions, and because Exchange administrators can change the default throttling policies for on-premises deployments, this article does not provide the default setting values. It is more important for you to be aware of the considerations for designing an application that functions within throttling limits and reacts appropriately to throttling scenarios.

Si vous êtes un développeur d'applications, vous devez factoriser la limitation dans la conception de votre application. Selon les versions d'Exchange, les valeurs par défaut des paramètres de limitation EWS varient. Les applications clientes et de service qui sont conçues pour accéder à différentes versions d'Exchange doivent prendre en compte ces paramètres, qu'il s'agisse de valeurs par défaut, de valeurs personnalisées définies par un administrateur Exchange ou, comme pour Exchange Online, de la valeur définie par défaut non détectable. Étant donné que les valeurs du paramètre de limitation ne peuvent pas être détectées par un programme, les spécifications de conception de votre client doivent inclure un plan permettant à l'application de s'adapter à différents seuils de limitation potentiels. Lorsque vous concevez des applications à threads multiples qui accèdent à un grand nombre de boîtes aux lettres ou lorsque de nombreux clients accèdent à la même boîte aux lettres, tenez compte des limites de simultanéité auxquelles la stratégie par défaut s’applique à Exchange.

## <a name="throttling-policies-that-affect-ews"></a>Stratégies de limitation affectant EWS

Les stratégies de limitation d'Exchange affectent non seulement EWS, mais également toutes les connexions clientes au serveur Exchange, y compris les protocoles utilisés par Office Outlook, Outlook Web App et Exchange ActiveSync.

The **CPUStartPercent** throttling policy can affect EWS performance when you are running Exchange 2010. When the average CPU utilization of Exchange processes running on the Client Access server — including, but not limited to, the EWS process — exceeds the value specified by this policy, inbound requests will be delayed to reduce CPU utilization. You cannot change the value of this policy, but knowing about it can help you troubleshoot performance issues. The sampling logic the Client Access server performs for this value is an average over a 10 second rolling window. This allows the process to respond appropriately to quick spikes in CPU utilization. When this threshold is exceeded, inbound connections to EWS are delayed. This delay is capped at 500 milliseconds (msecs) at a theoretical 100% CPU usage per EWS request. If a batch EWS request to get 100 items is passed, the server will check the CPU usage 100 times (once per item) for a maximum delay of 50 seconds. The delay time is linearly proportional to CPU usage. At **CPUStartPercent**, the delay is 0 (a thread yield) and it increases linearly up to 500 msec at 100% CPU usage. Because throttling policies apply to all Exchange users, it's unlikely that CPU usage would exceed the **CPUStartPercent** limit on an Exchange Client Access server, because individual users or applications cannot gain enough CPU utilization to affect server operation.

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
|**EwsMaxBurst** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Defines the amount of time that an EWS user can consume an elevated amount of resources before being throttled. This is measured in milliseconds. This value is set separately for each component.  <br/> |
|**EwsRechargeRate** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Définit la fréquence à laquelle le budget d'un utilisateur EWS est rechargé (budgétisation) pendant la période de budget.  <br/> |
|**EWSMaxSubscriptions** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Defines the maximum number of active push, pull, and streaming notification subscriptions that a user can have on a specific Client Access server at one time. This is budgeted differently for different Exchange versions.  <br/> |
|**EWSFastSearchTimeoutInSeconds** <br/> |Exchange 2010  <br/> |Définit la durée en secondes des recherches rapides effectuées avec la recherche Exchange dans EWS avant leur délai d'expiration. Les recherches rapides sont effectuées à l'aide d'une chaîne de requête AQS (syntaxe de requête avancée) dans une [FindItem Operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).      <br/> |
|**EWSFindCountLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Defines the maximum number of items from a [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) or [FindFolder operation](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) that can exist in memory on the Client Access server at one time for one user. The default value for this property is 1000. The [fallback value](https://technet.microsoft.com/library/dd297964%28v=exchg.141%29.aspx#fallback)for this value is 1000.  <br/> In Exchange Online and on-premises versions of Exchange starting with Exchange 2013, this throttling policy cannot be queried or configured by a cmdlet. In Exchange Online and on-premises versions of Exchange starting with Exchange 2013, the EWSFindCountLimit for [AQS search](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md) and any Exchange search with a restriction is 250 results. An Exchange search without a restriction will return up to 1000 results.  <br/> |
|**EWSPercentTimeInAD** <br/> |Exchange 2010  <br/> |Définit le pourcentage de temps par minute où un utilisateur spécifique peut exécuter des demandes Active Directory.  <br/> |
|**EWSPercentTimeInCAS** <br/> |Exchange 2010  <br/> |Définit le pourcentage de temps par minute où un utilisateur spécifique peut exécuter le code de serveur d'accès au client.  <br/> |
|**EWSPercentTimeInMailboxRPC** <br/> |Exchange 2010  <br/> |Définit le pourcentage de temps par minute où un utilisateur spécifique peut exécuter des demandes RPC de boîte aux lettres.  <br/> |
|**EWSMaxConcurrency** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Defines the number of concurrent open connections that a specific user can have against an Exchange server that is using EWS at one time. The default value for Exchange 2010 is 10. The default value for Exchange 2013 and Exchange Online is 27.  <br/> This policy applies to all operations except for streaming notifications. Streaming notifications use the **HangingConnectionLimit** to indicate the number of open streaming event connections that are available. For more information, see [What throttling values do I need to take into consideration?](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).  <br/> |
|**MessageRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Définit le nombre de messages pouvant être envoyés par minute.  <br/> |
|**RecipientRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Définit le nombre maximal de destinataires auxquels un utilisateur peut adresser des messages sur une période de 24 heures.  <br/> |
|**ForwardeeLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Définit le nombre maximal de destinataires pour les actions de transfert/redirection de la boîte de réception sur une période de 24 heures.  <br/> |
|**ConcurrentSyncCalls** <br/> |Exchange 2019  <br/> Exchange 2016  <br/> Exchange Online  <br/> |Définit la limite du nombre d’appels de synchronisation simultanés (Opérationsyncfolderhierarchy, SyncFolderItems) pour un utilisateur. <br/> |

> [!CAUTION]
> Do not set throttling polices to **null**. This will set the policy to equal unlimited, which indicates that a throttling policy isn't set.

## <a name="displaying-the-policies-that-apply-to-exchange-mailboxes"></a>Affichage des stratégies qui s'appliquent aux boîtes aux lettres Exchange

Exchange on-premises provides Exchange Management Shell cmdlets that you can use to set and get throttling policy. Exchange Online does not provide access to the throttling policy cmdlets.

Vous pouvez utiliser les cmdlets suivantes pour afficher les stratégies de limitation pour un déploiement Exchange Server local :

- **Get-ThrottlingPolicy**: permet d'obtenir les paramètres de limitation des clients pour une ou plusieurs stratégies de limitation. Pour plus d’informations, consultez la rubrique [Get-ThrottlingPolicy](https://technet.microsoft.com/library/dd351264.aspx) sur TechNet.

- **Get-ThrottlingPolicyAssociation** — Enables you to view the relationship between an object and its associated throttling policies. The object can be a user with a mailbox, a user without a mailbox, or a contact. For more information, see [Get-ThrottlingPolicyAssociation](https://technet.microsoft.com/library/ff459241.aspx) on TechNet.

Utilisez la commande suivante pour afficher la stratégie de limitation par défaut pour Exchange 2010.

**Get-ThrottlingPolicy | Where-Object {$_.IsDefault -eq "True"} | format-list**

Utilisez la commande suivante pour afficher la stratégie de limitation globale pour Exchange 2013 (ce qui correspond à la stratégie de limitation par défaut dans Exchange 2010).

**Get-ThrottlingPolicy | Where-Object {$_.ThrottlingPolicyScope -eq "Global"} | format-list**

Use the following command to show the throttling policy associated with a user in Exchange 2010 or Exchange 2013. Replace the user name john@contoso.com with the user name of the target user for whom you want to get throttling policy information.

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
> [!REMARQUE] Lorsque la propriété **ThrottlingPolicyId** est vide, la stratégie par défaut s'applique à la boîte aux lettres.

Vous pouvez définir une stratégie de limitation sur un serveur Exchange à l'aide des cmdlets [Set-ThrottlingPolicy](https://technet.microsoft.com/library/dd298094.aspx) et [Set-ThrottlingPolicyAssociation](https://technet.microsoft.com/library/ff459231.aspx). Vous pouvez créer et supprimer des stratégies de limitation non définies par défaut à l’aide des cmdlets [New-ThrottlingPolicy](https://technet.microsoft.com/library/dd351045.aspx) et [Remove-ThrottlingPolicy](https://technet.microsoft.com/library/dd351178.aspx) .

> [!TIP]
> We recommend that you design your applications to adhere to the default throttling policy. Only make changes to default throttling policies if your client application design cannot accommodate the default policy. Be aware that less restrictive throttling policies can negatively affect service reliability.

## <a name="throttling-considerations-for-applications-that-use-ews-impersonation"></a>Observations à propos de la limitation pour les applications qui utilisent l’emprunt d’identité EWS

[Impersonation](impersonation-and-ews-in-exchange.md) is an authorization method that enables a single account to access many accounts. When a service account impersonates users, it acts as the users and therefore assumes the rights that are assigned to those users. Log files record the access as the impersonated user. Administrators use role-based access control (RBAC) to configure impersonation via the Exchange Management Shell.

Lorsque l'emprunt d'identité est utilisé, les budgets de tous les seuils de limitation s'appliquent différemment selon la version d'Exchange. Le budget est calculé en fonction du compte qui est emprunté ou du compte de service. Si votre application est multi-thread et effectue des demandes simultanées sur plusieurs boîtes aux lettres, vous devez tenir compte de la façon dont le seuil de limitation affecte les performances de votre application. En règle générale, vous devez avoir connaissance des seuils suivants sur les comptes de service lorsque vous créez une application de service qui utilise l'emprunt d'identité pour accéder à toutes les boîtes aux lettres :

- Lorsque vous utilisez l'emprunt d'identité, le compte de service a un budget distinct pour les paramètres de stratégie suivants :

  - **EWSMaxConcurrency**

  - **EWSPercentTimeInAD**

  - **EWSPercentTimeInCAS**

  - **EWSPercentTimeInMailboxRPC**

  - **EWSMaxSubscriptions**

  - **EWSFastSearchTimeoutInSeconds**

  - **EWSFindCountLimit**

- The **EWSMaxConcurrency** budget is shared for the service account and the account being impersonated for all connections to versions of Exchange earlier than Exchange 2010 Service Pack 2 (SP2) Update Rollup 4 (RU4). Starting with Exchange 2010 SP2 RU4, and including Exchange Online, the service account access uses a separate budget from the user **EWSMaxConcurrency** budget. For more information about the update to the Exchange concurrent connection throttling policy for EWS, see [Description of Update Rollup 4 for Exchange Server 2010 Service Pack 2](https://support.microsoft.com/kb/2706690).

    EWS streaming notifications in versions of Exchange starting with Exchange 2010, and including Exchange Online, have an additional cloned **EWSMaxConcurrency** budget from all other EWS client connections. Streaming notification connections are counted against a separate budget than all other EWS operations. The streaming notification maximum concurrency budget is actually two different budgets: one budget is for all service accounts, and one budget is for the account being impersonated. Streaming notifications in Exchange Online and versions of Exchange starting with Exchange 2013 use the [HangingConnectionLimit](#throttling-considerations-for-ews-notification-applications) to limit the number of connections.

    For example, let's assume that **EWSMaxConcurrency** is equal to five. A user can have five open pull notification connections, while an service account can have five concurrent pull notification connections against the user's mailbox at the same time as the user.

- Le tableau suivant identifie la façon dont les budgets de limitation **EWSMaxSubscriptions** sont calculés entre le compte de service et le compte auquel emprunter l'identité.

   **Tableau 2 : Gestion du budget EWSMaxSubscriptions**

   |**Version d'Exchange**|**Gestion du budget de limitation EWSMaxSubscriptions**|
   |:-----|:-----|
   |Exchange Online  <br/> |Facturé en fonction de la boîte aux lettres cible.  <br/> |
   |Exchange 2013  <br/> |Facturé en fonction de la boîte aux lettres cible.  <br/> |
   |Exchange 2010 SP3  <br/> |Facturé en fonction de la boîte aux lettres cible.  <br/> |
   |Exchange 2010 SP2  <br/> |Charged against the calling account. Starting with Exchange 2010 SP2 RU4, the budget is charged against the target mailbox.  <br/> |
   |Exchange 2010 SP1  <br/> |Facturé en fonction du compte d’appel.  <br/> |
   |Exchange 2010  <br/> |Facturé en fonction du compte d'appel.  <br/> |

- Étant donné que le budget de limitation **EWSMaxSubscriptions** est facturé en fonction du compte dont l'identité est empruntée, il n'existe aucune limite relative au nombre de boîtes aux lettres auxquelles un compte de service peut s'abonner et à partir desquelles il peut recevoir des notifications de diffusion en continu, tant que l'emprunt d'identité est en cours. Pour le compte dont l'identité est empruntée, vous ne pouvez pas disposer de plus de  _n_ demandes simultanées par boîte aux lettres cible, où  _n_ correspond à la valeur de **EWSMaxSubscriptions**. Si vous n'utilisez pas l'emprunt d'identité, le même compte de service ne peut pas disposer de plus de  _n_ demandes simultanées en tout. Par conséquent, en utilisant l’emprunt d’identité avec un compte de service, vous augmentez de manière exponentielle le nombre de boîtes aux lettres que vous pouvez activer. Pour plus d'informations, voir[Maintenir l'affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md).

- The **EWSPercentTimeInMailboxRPC**, **EWSPercentTimeInCAS**, and **EWSPercentTimeInAD** policy parameters refer to actions performed by a single thread. When an application performs multiple concurrent operations, you should account for the cumulative effect of these operations on the user resource budget.

## <a name="throttling-implications-for-ews-batch-requests"></a>Implications de la limitation pour les demandes de lot EWS

EWS enables you to batch multiple item requests into a single request that is executed by the Client Access server. This allows for greater efficiency and performance. When an Exchange server executes a batched request, it checks the user's budget after the execution of each item within the batch. If the application is over budget, the processing of the next item in the batch is delayed until the budget for that user has recharged. To ensure that applications that use batch operations run successfully, limit the number of item requests that can be included in a single batch, and divide large batches across multiple smaller batches to increase the reliability of the results. The effect that a batch operation has on particular throttling thresholds depends on the type of the request, the size of the items to be processed (for example in **UploadItems** or **ExportItems** operations) and the mailbox content. Throttling policies affect batch operations by causing the request to take longer to process. The caller will therefore have to wait longer for the response, and, because EWS limits the execution time of a batch request to one minute, the call could time out.

Pour déterminer la taille de lot optimale pour une application, effectuez un test unitaire avec plusieurs ensembles de valeurs d'entrée pour vous assurer que l'application ne rencontre aucune erreur dans un environnement de production.

## <a name="throttling-policy-parameters-that-affect-ews-search-operations"></a>Paramètres de stratégie de limitation qui affectent les opérations de recherche EWS

[Search operations in EWS](search-and-ews-in-exchange.md) can require large amounts of time and resources, depending on how the search is run and what information is requested. To control resource usage during searches, two policy parameters take effect: **EWSFastSearchTimeoutInSeconds** and **EWSFindCountLimit**.

Le paramètre de stratégie **EWSFastSearchTimeoutInSeconds** spécifie la durée, en secondes, d'exécution des recherches rapides EWS (également appelées recherche d'indexation de contenu) avant expiration. Une recherche rapide est effectuée à l'aide d'une chaîne de requête AQS (syntaxe de requête avancée) dans une [FindItem Operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).

Vous pouvez effectuer une recherche dans un dossier de boîte aux lettres Exchange des deux manières suivantes :

- En effectuant une recherche dans la banque d'informations Exchange, qui effectue une analyse séquentielle de tous les messages dans la zone de recherche cible.

- En utilisant le service de recherche Exchange (indexation de contenu).

Both of these types of searches can result in timeouts. When possible, use the Exchange Search service because these searches are often targeted against mailbox indexes and use AQS queries. The following example shows how to perform an AQS search of the Inbox by using EWS and the Exchange Search service.

```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiitems = service.FindItems(WellKnownFolderName.Inbox, "subject:football", iv);
```

If you can't use an AQS search, avoid using overly complex search filters. Also try to avoid creating search filters based on computed values if the query involves extended MAPI properties. AQS search was introduced in Exchange 2010.

> [!NOTE]
> The first time you run a complex Exchange store search query, it runs very slowly and may time out. After that, the query will respond more quickly. For more information about the backend Exchange server processes that occur during Exchange store search queries, see [Understanding the Performance Impact of High Item Counts and Restricted Views](https://technet.microsoft.com/library/cc535025%28EXCHG.80%29.aspx) on TechNet. Using a **SearchFilter** creates a dynamic restriction that helps similar queries in the future, but because these restrictions are dynamic in nature, they are not permanent or reliable, and are deleted after a maximum of three days.

The **EWSFindCountLimit** policy parameter specifies the maximum number of items from the results of a **FindItem** or **FindFolder** operation that can exist in memory on a Client Access server at the same time for one user. Every item or folder that EWS processes in a **FindItem** or **FindFolder** request is counted against the budget specified in the **EWSFindCountLimit** element. When the response is sent back to the requester, the find count charge for the current call is released. The response the server returns to a requester when the budget is exceeded is based on the **RequestServerVersion** element value and whether the requester specified paging. When the value of the **RequestServerVersion** element indicates Exchange 2010 or an earlier version of Exchange, the server sends a failure response with error code **ErrorServerBusy**. If the value of the **RequestServerVersion** element indicates a version of Exchange starting with Exchange 2010 SP1 or Exchange Online, and the client is using paging, EWS may return a partial result set instead of an error. Your application should expect that EWS might not return all items. If the value of the **IncludesLastItemInRange** element is false, the application should make another **FindItem** or **FindFolder** request with the new offset and continue until the **IncludesLastItemInRange** element returns true.

When you use a **FindItem** or **FindFolder** operation, it is important to use paging. The EWS Managed API enforces the use of paging, but if you are using other methods, such as EWS proxy objects or raw SOAP, you need to explicitly set paging. The following example shows how to use paging in the EWS Managed API.

```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiFindItemResults = service.FindItems(WellKnownFolderName.Inbox, iv);
```

> [!NOTE]
> The default policy in Exchange limits the page size to 1000 items. Setting the page size to a value that is greater than this number has no practical effect.

Applications should also account for the fact that the  _EWSFindCountLimit_ throttling parameter value may result in a partial result set being returned for applications that make concurrent requests. The following example shows how to use the **MoreAvailable** property in the EWS Managed API to ensure that all results are included in a query.

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

Concurrency refers to the number of connections from a specific user. A connection is held from the moment a request is received until a response is sent to the requester. If users try to make more concurrent requests than their policy allows, the new connection attempt fails. However, the existing connections remain valid. Throttling policies can affect concurrency in a number of different ways.

The **EWSMaxConcurrency** throttling policy parameter sets the number of concurrent connections that a specific user can have against an Exchange server at one time. To determine the maximum number of concurrent connections to allow, consider the connections that Outlook clients will use. Outlook 2007 and Outlook 2010 use EWS to access availability and Out of Office (OOF) information. Mac Outlook 2011 uses EWS for all client access functionality. Depending on the number of Outlook clients that are actively connecting to a user's mailbox, the number of concurrent connections available for a user might be limited. Also, if your application has to connect to multiple mailboxes simultaneously while using a single security context, it is important to take the value of the **EWSMaxConcurrency** policy into account. For more information about using a single security context with concurrent connections, see [Throttling considerations for applications that use EWS impersonation](#throttling-considerations-for-applications-that-use-ews-impersonation) earlier in this article.

Applications that concurrently connect to multiple mailboxes have to be able to track resource usage on the client side. Because EWS operations are request/response-based, you can ensure that your applications function well within the **EWSMaxConcurrency** threshold by tracking the number of connections that occur between the start of a request and when the response is received and ensuring that no more than ten open requests occur concurrently.

The **EWSFindCountLimit** policy parameter specifies the maximum result size a **FindItem** or **FindFolder** operation can use on a Client Access server at the same time for one user. If an application (or potentially multiple applications) makes two concurrent EWS **FindItem** requests that return 100 items each for a specific user, the **EWSFindCountLimit** charge against that specific user's budget will be 200. When the first request returns, the budget drops to 100, and when the second request returns, the budget drops to zero. If the same application were to make two simultaneous requests for 1000 items, the budget value would be 2000 items, which exceeds the **EWSFindCountLimit** value. If the user's budget for items drops below zero, the next request results in an error until the user's budget recharges to one or more.

## <a name="throttling-considerations-for-ews-notification-applications"></a>Observations à propos de la limitation pour les applications de notification EWS

Si vous créez des applications EWS qui utilisent des notifications Push, d'extraction ou de diffusion en continu, vous devez tenir compte des implications des stratégies de limitation **EWSMaxSubscriptions** et **EWSMaxConcurrency**, ainsi que de la limite **HangingConnectionLimit**.

The **EWSMaxSubscriptions** policy parameter specifies the maximum number of active push, pull, and streaming subscriptions that a user can have on a specific Client Access server at the same time. Different versions of Exchange have different default values for this parameter. A user can subscribe to all folders in a mailbox by using the **SubscribeToAllFolders** property - this uses a single subscription against the **EWSMaxSubscriptions** budget. Users can subscribe to individual folders, with each folder subscription counting towards the **EWSMaxSubscriptions** budget, up to the limit set by the value of the **EWSMaxSubscriptions** parameter (for example, users can subscribe to 20 calendar folders in different mailboxes if **EWSMaxSubscriptions** is set to 20).

Pour plus d'informations sur l'emprunt d'identité et le paramètre **EWSMaxSubscriptions**, consultez la section [Considérations relatives à la limitation pour les applications qui utilisent l'emprunt d'identité EWS](#throttling-considerations-for-applications-that-use-ews-impersonation) plus haut dans cet article.

Le paramètre de stratégie **EWSMaxConcurrency** peut également représenter un problème pour les notifications EWS, par exemple :

- Quand EWS incrémente le nombre de connexions pour le titulaire de l'abonnement alors que la notification est générée par un abonnement par émission de données.

- Quand une application est conçue de manière à écouter les boîtes aux lettres de plusieurs utilisateurs et que les utilisateurs reçoivent des notifications simultanées pour une instance d'un message qui est envoyé à une liste de distribution.

Si l’application de notification est multi-thread et effectue des demandes de connexion simultanées pour obtenir plus d’informations sur un message particulier reçu par un compte d’utilisateur, la limite de stratégie **EWSMaxConcurrency** peut être dépassée. Pour parer cette éventualité, pensez à surveiller les connexions simultanées de votre application (y compris celles pouvant être utilisées par le serveur) et à implémenter la mise en file d'attente des demandes sur le client.

Le paramètre **HangingConnectionLimit** est valable uniquement pour les notifications de diffusion en continu. Cette limite est définie dans le fichier web.config, ce qui signifie qu’un administrateur Exchange peut définir cette valeur sur un serveur Exchange local, mais les boîtes aux lettres Exchange Online doivent utiliser la valeur par défaut pour cette limite, 10 pour Exchange Online, Exchange 2019, Exchange 2016 et 3 pour Exchange 2013. Pour en savoir plus, consultez la rubrique relative aux [valeurs de limitation à prendre en compte](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).

## <a name="throttling-policy-and-application-performance"></a>Stratégie de limitation et performances d'application

Les trois paramètres suivants de la stratégie de limitation **PercentTimeIn** affectent la durée qu'une application EWS peut consommer sur un serveur d'accès au client :

- **EWSPercentTimeInAD**

- **EWSPercentTimeInCAS**

- **EWSPercentTimeInMailboxRPC**

The values specified in the **PercentTimeIn** policy parameters indicate the amount of time that one thread making one request is allocated. For example, assuming a **EWSPercentTimeInCAS** value of 90, if a process makes two concurrent requests that spend 54 seconds each running code on the Client Access server, the process uses 108 seconds in a 60 second window. This represents an **EWSPercentTimeInCAS** parameter value of 180 percent.

> [!NOTE]
> The **EWSPercentTimeInCAS** parameter value is an overlapping superset of the **EWSPercentTimeInAD** and **EWSPercentTimeInMailboxRPC** parameter values. This means that the expenditure in Client Access server processing time will always be larger than the expenditures in **EWSPercentTimeInAD** and **EWSPercentTimeInMailboxRPC**. This is because for the Exchange component to make an Active Directory or RPC call, it must already be running Client Access server code. In addition, the expenditure in processing time for **EWSPercentTimeInCAS** doesn't stop while LDAP or RPC calls are being made. Although the request might be synchronously waiting for a response from Active Directory Domain Services (AD DS) or the Exchange store, the process is still consuming a thread on the server, and therefore the thread should continue to be charged for that usage.

Le temps processeur qu’une application peut prendre pendant une période de 60 seconde peut dépasser ces limites de limitation ; par conséquent, il est important de prendre en compte le volume et le type de demandes effectuées. Par exemple, un lot important d’opérations **ResolveNames** effectuées simultanément peut dépasser la valeur du paramètre de stratégie **EWSPercentTimeInAD** . Les valeurs de stratégie contenues dans la stratégie de limitation par défaut sont conçues pour permettre à la plupart des applications EWS de fonctionner sans problème ; Toutefois, lorsque des applications à volumes élevés à plusieurs threads placent un grand nombre de demandes sur un serveur d’accès au client particulier, cela peut créer des problèmes. Pour éviter cela, envisagez de limiter la taille des lots qui vont s’exécuter sur le serveur.

## <a name="throttling-policies-and-applications-that-send-a-large-volume-of-email"></a>Stratégies de limitation et applications qui envoient une quantité élevée de messages électroniques

Les stratégies de limitation par défaut incluent trois paramètres de stratégie de limitation du débit pouvant affecter les applications qui utilisent EWS pour envoyer un volume élevé de messages ou pour envoyer des messages par lot important sur une courte période de temps.

> [!NOTE]
> In general, we recommend that you do not use EWS to send bulk email. Use an SMTP host that specializes in bulk mail services to submit frequent large bulk email messages.

The **MessageRateLimit** policy parameter specifies the number of messages per minute that can be submitted by any Exchange client, including EWS. By default, this policy is set to 30 messages per minute. For ordinary users, this is generally sufficient. However, applications that send large batches of email messages, for example as part of an invoicing program, can run into problems. When this policy limit is exceeded, message delivery for the mailbox is delayed. Specifically, messages will appear in the Outbox or Drafts folder for longer periods of time when a user or application submits a larger number of messages than the value specified by the **MessageRateLimit** parameter. Be sure to consider this when you are developing a delivery tracking system, especially if your application uses a mailbox that users connect to via Outlook. When deferred items are stored in the Outbox or drafts folder, users might interpret that as an error.

The **RecipientRateLimit** policy parameter specifies the limit on the number of recipients that a user can address in a 24-hour period. For example, if this value is set to 500, it means that a single Exchange mailbox account can send messages to no more than 500 recipients each day. This limit applies to messages to recipients that are inside and outside the organization. This default limit might cause problems for some line-of-business applications that do end-of-month invoice runs and need to send messages to more than this number of recipients. You can use external services that enable batch processing of messages or separate on-premises outbound relay solutions to work around this limitation.

The **ForwardeeLimit** policy parameter specifies the maximum number of recipients that messages can be forwarded or redirected to by means of Inbox rules. This parameter doesn't limit the number of messages that can be forwarded or redirected to the recipients.

## <a name="errors-generated-when-throttling-limits-are-exceeded"></a>Erreurs générées lorsque les seuils de limitation sont dépassés

Lorsque les stratégies de limitation sont dépassées, EWS génère l'une des erreurs répertoriées dans le tableau suivant.

**Tableau 3 : Erreurs de seuil de limitation**

|**Erreur**|**Paramètre de stratégie de limitation**|**Description**|
|:-----|:-----|:-----|
|ErrorExceededConnectionCount  <br/> |**EWSMaxConcurrency** <br/> |Indique que le nombre de demandes simultanées sur le serveur dépasse la limite autorisée par la stratégie de l'utilisateur.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |**EWSMaxSubscriptions** <br/> |Indique que le nombre maximal d'abonnements défini par une stratégie de limitation d'un utilisateur a été dépassé.  <br/> |
|ErrorExceededFindCountLimit  <br/> |**EWSFindCountLimit** <br/> |Indique qu'un appel d'opération de recherche a dépassé le nombre total d'éléments pouvant être renvoyés.  <br/> |
|ErrorServerBusy  <br/> |**EWSPercentTimeInMailboxRPC**         **EWSPercentTimeInCAS**         **EWSPercentTimeInAD** <br/> |Occurs when the server is busy. The BackOffMilliseconds value returned with ErrorServerBusy errors indicates to the client the amount of time it should wait until it should resubmit the request that caused the response that returned this error code.  <br/> |

Le tableau suivant répertorie les codes d'état HTTP renvoyés par les erreurs de limitation.

**Tableau 4 : Codes d'état HTTP renvoyés par les erreurs de limitation**

|**Code d'état HTTP**|**Description**|
|:-----|:-----|
|HTTP 503  <br/> |Indicates that EWS requests are queuing with IIS. The client should delay sending additional requests until a later time.  <br/> |
|HTTP 500  <br/> |Indicates an internal server error with the ErrorServerBusy error code. This indicates that the client should delay sending additional requests until a later time. The response may contain a back off hint called BackOffMilliseconds. If present, the value of BackOffMilliseconds should be used as the duration until the client resubmits a request.  <br/> |
|HTTP 200  <br/> |Contains an EWS schema-based error response with an ErrorInternalServerError error code. An inner ErrorServerBusy error code may be present. This indicates that the client should delay sending additional requests until a later time.  <br/> |

## <a name="see-also"></a>Voir aussi

- [Gestion de la charge de travail Exchange](https://technet.microsoft.com/library/jj150503.aspx)
- [Cmdlet New-ThrottlingPolicy](https://technet.microsoft.com/library/dd351045.aspx)
- [Présentation des stratégies de limitation du client](https://technet.microsoft.com/library/dd297964.aspx)
- [Classe ThrottlingPolicy](https://msdn.microsoft.com/library/ff342496%28v=EXCHG.140%29.aspx)
- [Stratégies de limitation et limite EWSFindCountLimit](https://blogs.msdn.com/b/exchangedev/archive/2010/03/12/throttling-policies-and-the-ewsfindcountlimit.aspx)
- [Captures instantanées du budget dans les journaux IIS](https://blogs.msdn.com/b/exchangedev/archive/2010/03/10/budget-snapshots-in-the-iis-logs.aspx)

- [Effets de la limitation sur votre déploiement dans Exchange 2010 SP1](http://msexchangeteam.com/archive/2010/08/27/456040.aspx)
- [Associations de stratégies de limitation dans Exchange 2010 SP1](http://msexchangeteam.com/archive/2010/08/02/455707.aspx)
- [Stratégies de limitation et CPUStartPercent](https://blogs.msdn.com/b/exchangedev/archive/2010/03/11/throttling-policies-and-cpustartpercent.aspx)
- [Emprunt d'identité et EWS dans Exchange](impersonation-and-ews-in-exchange.md)
