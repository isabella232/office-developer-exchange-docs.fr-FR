---
title: surveillance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- monitoring
api_type:
- schema
ms.assetid: 350d7b46-9260-41a7-8613-3cb8cc1b29a5
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: 5614ac2c6428da9b6845769a9335486d3ded5754
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455827"
---
# <a name="monitoring"></a><span data-ttu-id="e9299-103">surveillance</span><span class="sxs-lookup"><span data-stu-id="e9299-103">monitoring</span></span>
  
<span data-ttu-id="e9299-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="e9299-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="e9299-105">L’élément **Monitoring** contient des informations de configuration qui définissent comment et quand le service de transport frontal ou le service de transport surveille les agents installés.</span><span class="sxs-lookup"><span data-stu-id="e9299-105">The **monitoring** element contains configuration information that defines how and when the Front End transport service or the Transport service monitors agents that are installed.</span></span> 
  
- [<span data-ttu-id="e9299-106">configuration</span><span class="sxs-lookup"><span data-stu-id="e9299-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="e9299-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="e9299-107">mexRuntime</span></span>](mexruntime.md)  
- [<span data-ttu-id="e9299-108">surveillance</span><span class="sxs-lookup"><span data-stu-id="e9299-108">monitoring</span></span>](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

<span data-ttu-id="e9299-109">**monitoringType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="e9299-109">**monitoringType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e9299-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e9299-110">Attributes and elements</span></span>

<span data-ttu-id="e9299-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e9299-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9299-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="e9299-112">Attributes</span></span>

<span data-ttu-id="e9299-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e9299-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9299-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e9299-114">Child elements</span></span>

|<span data-ttu-id="e9299-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e9299-115">**Element**</span></span>|<span data-ttu-id="e9299-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9299-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9299-117">agentExecution</span><span class="sxs-lookup"><span data-stu-id="e9299-117">agentExecution</span></span>](agentexecution.md) <br/> |<span data-ttu-id="e9299-118">Définit le temps, en millisecondes, au-delà duquel le serveur d’accès au client ou de boîtes aux lettres doit attendre qu’un agent renvoie à partir d’un événement avant d’écrire dans le journal des événements.</span><span class="sxs-lookup"><span data-stu-id="e9299-118">Defines the time, in milliseconds, for the Client Access or the Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span>  <br/> |
|[<span data-ttu-id="e9299-119">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="e9299-119">messageSnapshot</span></span>](messagesnapshot.md) <br/> |<span data-ttu-id="e9299-120">Contient un attribut qui indique si la fonctionnalité de suivi de pipeline est activée pour le serveur d’accès au client ou de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e9299-120">Contains an attribute that specifies whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9299-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e9299-121">Parent elements</span></span>

|<span data-ttu-id="e9299-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e9299-122">**Element**</span></span>|<span data-ttu-id="e9299-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9299-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9299-124">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="e9299-124">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="e9299-125">Contient des éléments qui définissent les informations de configuration des informations de configuration et de surveillance de l’agent pour les agents SMTP et de routage installés.</span><span class="sxs-lookup"><span data-stu-id="e9299-125">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="e9299-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e9299-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9299-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e9299-127">Namespace</span></span>  <br/> |<span data-ttu-id="e9299-128">Ce fichier ne définit pas d’espace de noms.</span><span class="sxs-lookup"><span data-stu-id="e9299-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="e9299-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e9299-129">Schema Name</span></span>  <br/> |<span data-ttu-id="e9299-130">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="e9299-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="e9299-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e9299-131">Validation File</span></span>  <br/> |<span data-ttu-id="e9299-132">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="e9299-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="e9299-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e9299-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9299-134">Faux.</span><span class="sxs-lookup"><span data-stu-id="e9299-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9299-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e9299-135">See also</span></span>

- [<span data-ttu-id="e9299-136">Éléments du fichier de configuration des agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e9299-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

