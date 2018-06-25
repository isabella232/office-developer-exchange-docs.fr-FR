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
ms.openlocfilehash: 1b5484467def0bf3d22ba0707357977d5ed461ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755139"
---
# <a name="monitoring"></a><span data-ttu-id="44b1d-103">surveillance</span><span class="sxs-lookup"><span data-stu-id="44b1d-103">monitoring</span></span>
  
<span data-ttu-id="44b1d-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="44b1d-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="44b1d-105">L’élément de **surveillance** contient des informations de configuration qui définit comment et quand le service de transport frontal ou le service de Transport analyse les agents qui sont installés.</span><span class="sxs-lookup"><span data-stu-id="44b1d-105">The **monitoring** element contains configuration information that defines how and when the Front End transport service or the Transport service monitors agents that are installed.</span></span> 
  
- [<span data-ttu-id="44b1d-106">configuration</span><span class="sxs-lookup"><span data-stu-id="44b1d-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="44b1d-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="44b1d-107">mexRuntime</span></span>](mexruntime.md)  
- [<span data-ttu-id="44b1d-108">surveillance</span><span class="sxs-lookup"><span data-stu-id="44b1d-108">monitoring</span></span>](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

<span data-ttu-id="44b1d-109">**monitoringType (type complexe)**</span><span class="sxs-lookup"><span data-stu-id="44b1d-109">**monitoringType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="44b1d-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="44b1d-110">Attributes and elements</span></span>

<span data-ttu-id="44b1d-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="44b1d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44b1d-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="44b1d-112">Attributes</span></span>

<span data-ttu-id="44b1d-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="44b1d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44b1d-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="44b1d-114">Child elements</span></span>

|<span data-ttu-id="44b1d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="44b1d-115">**Element**</span></span>|<span data-ttu-id="44b1d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="44b1d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44b1d-117">agentExecution</span><span class="sxs-lookup"><span data-stu-id="44b1d-117">agentExecution</span></span>](agentexecution.md) <br/> |<span data-ttu-id="44b1d-118">Définit la durée, en millisecondes, pour l’accès au Client ou le serveur de boîtes aux lettres d’attente d’un agent renvoyer à partir d’un événement avant de les écrire dans le journal des événements.</span><span class="sxs-lookup"><span data-stu-id="44b1d-118">Defines the time, in milliseconds, for the Client Access or the Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span>  <br/> |
|[<span data-ttu-id="44b1d-119">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="44b1d-119">messageSnapshot</span></span>](messagesnapshot.md) <br/> |<span data-ttu-id="44b1d-120">Contient un attribut qui spécifie si la fonctionnalité de suivi du pipeline est activée pour l’accès au Client ou le serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="44b1d-120">Contains an attribute that specifies whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="44b1d-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="44b1d-121">Parent elements</span></span>

|<span data-ttu-id="44b1d-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="44b1d-122">**Element**</span></span>|<span data-ttu-id="44b1d-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="44b1d-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44b1d-124">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="44b1d-124">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="44b1d-125">Contient des éléments qui définissent les informations de configuration pour l’agent de surveillance et les informations de configuration pour SMTP et les agents de routage qui sont installés.</span><span class="sxs-lookup"><span data-stu-id="44b1d-125">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="44b1d-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="44b1d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44b1d-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="44b1d-127">Namespace</span></span>  <br/> |<span data-ttu-id="44b1d-128">Ce fichier ne définit pas un espace de noms.</span><span class="sxs-lookup"><span data-stu-id="44b1d-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="44b1d-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="44b1d-129">Schema Name</span></span>  <br/> |<span data-ttu-id="44b1d-130">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="44b1d-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="44b1d-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="44b1d-131">Validation File</span></span>  <br/> |<span data-ttu-id="44b1d-132">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="44b1d-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="44b1d-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="44b1d-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="44b1d-134">Faux</span><span class="sxs-lookup"><span data-stu-id="44b1d-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44b1d-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="44b1d-135">See also</span></span>

- [<span data-ttu-id="44b1d-136">Éléments du fichier de configuration agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="44b1d-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

