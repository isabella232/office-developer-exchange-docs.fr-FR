---
title: agentList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentList
api_type:
- schema
ms.assetid: e877b7ef-e303-4270-964d-8d116ff2a865
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: 99e4e24c3bca77c7e7d5f2c59bb21cee1317fed2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44446391"
---
# <a name="agentlist"></a><span data-ttu-id="56506-103">agentList</span><span class="sxs-lookup"><span data-stu-id="56506-103">agentList</span></span>
  
<span data-ttu-id="56506-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="56506-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="56506-105">L’élément **agentList** contient un élément [agent](agent.md) pour chaque agent installé.</span><span class="sxs-lookup"><span data-stu-id="56506-105">The **agentList** element contains an [agent](agent.md) element for each installed agent.</span></span> 
  
- [<span data-ttu-id="56506-106">configuration</span><span class="sxs-lookup"><span data-stu-id="56506-106">configuration</span></span>](configuration.md)
- [<span data-ttu-id="56506-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="56506-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="56506-108">agentList</span><span class="sxs-lookup"><span data-stu-id="56506-108">agentList</span></span>](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

<span data-ttu-id="56506-109">**agentListType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="56506-109">**agentListType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="56506-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="56506-110">Attributes and elements</span></span>

<span data-ttu-id="56506-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="56506-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56506-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="56506-112">Attributes</span></span>

<span data-ttu-id="56506-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="56506-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56506-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="56506-114">Child elements</span></span>

|<span data-ttu-id="56506-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="56506-115">**Element**</span></span>|<span data-ttu-id="56506-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="56506-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56506-117">agent</span><span class="sxs-lookup"><span data-stu-id="56506-117">agent</span></span>](agent.md) <br/> |<span data-ttu-id="56506-118">Contient des informations de configuration sur un agent installé.</span><span class="sxs-lookup"><span data-stu-id="56506-118">Contains configuration information about an installed agent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="56506-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="56506-119">Parent elements</span></span>

|<span data-ttu-id="56506-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="56506-120">**Element**</span></span>|<span data-ttu-id="56506-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="56506-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56506-122">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="56506-122">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="56506-123">Contient des éléments qui définissent les informations de configuration des informations de configuration et de surveillance de l’agent sur les agents installés.</span><span class="sxs-lookup"><span data-stu-id="56506-123">Contains elements that define configuration information for agent monitoring and configuration information about installed agents.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="56506-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="56506-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56506-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="56506-125">Namespace</span></span>  <br/> |<span data-ttu-id="56506-126">Ce fichier ne définit pas d’espace de noms.</span><span class="sxs-lookup"><span data-stu-id="56506-126">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="56506-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="56506-127">Schema Name</span></span>  <br/> |<span data-ttu-id="56506-128">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="56506-128">Not available.</span></span>  <br/> |
|<span data-ttu-id="56506-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="56506-129">Validation File</span></span>  <br/> |<span data-ttu-id="56506-130">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="56506-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="56506-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="56506-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="56506-132">Faux.</span><span class="sxs-lookup"><span data-stu-id="56506-132">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56506-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="56506-133">See also</span></span>

- [<span data-ttu-id="56506-134">Éléments du fichier de configuration des agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="56506-134">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

