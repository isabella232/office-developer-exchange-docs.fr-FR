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
ms.openlocfilehash: 7dd9d48356932c82dbc048a85b9f02437c6366de
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755111"
---
# <a name="agentlist"></a><span data-ttu-id="65ddd-103">agentList</span><span class="sxs-lookup"><span data-stu-id="65ddd-103">agentList</span></span>
  
<span data-ttu-id="65ddd-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="65ddd-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="65ddd-105">L’élément **agentList** contient un élément de [l’agent](agent.md) pour chaque agent installé.</span><span class="sxs-lookup"><span data-stu-id="65ddd-105">The **agentList** element contains an [agent](agent.md) element for each installed agent.</span></span> 
  
- [<span data-ttu-id="65ddd-106">configuration</span><span class="sxs-lookup"><span data-stu-id="65ddd-106">configuration</span></span>](configuration.md)
- [<span data-ttu-id="65ddd-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="65ddd-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="65ddd-108">agentList</span><span class="sxs-lookup"><span data-stu-id="65ddd-108">agentList</span></span>](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

<span data-ttu-id="65ddd-109">**agentListType (type complexe)**</span><span class="sxs-lookup"><span data-stu-id="65ddd-109">**agentListType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="65ddd-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="65ddd-110">Attributes and elements</span></span>

<span data-ttu-id="65ddd-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="65ddd-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65ddd-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="65ddd-112">Attributes</span></span>

<span data-ttu-id="65ddd-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="65ddd-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65ddd-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="65ddd-114">Child elements</span></span>

|<span data-ttu-id="65ddd-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65ddd-115">**Element**</span></span>|<span data-ttu-id="65ddd-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="65ddd-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65ddd-117">agent</span><span class="sxs-lookup"><span data-stu-id="65ddd-117">agent</span></span>](agent.md) <br/> |<span data-ttu-id="65ddd-118">Contient des informations de configuration sur un agent installé.</span><span class="sxs-lookup"><span data-stu-id="65ddd-118">Contains configuration information about an installed agent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65ddd-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="65ddd-119">Parent elements</span></span>

|<span data-ttu-id="65ddd-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65ddd-120">**Element**</span></span>|<span data-ttu-id="65ddd-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="65ddd-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65ddd-122">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="65ddd-122">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="65ddd-123">Contient des éléments qui définissent les informations de configuration pour l’agent de surveillance et les informations de configuration sur les agents installés.</span><span class="sxs-lookup"><span data-stu-id="65ddd-123">Contains elements that define configuration information for agent monitoring and configuration information about installed agents.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="65ddd-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="65ddd-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65ddd-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="65ddd-125">Namespace</span></span>  <br/> |<span data-ttu-id="65ddd-126">Ce fichier ne définit pas un espace de noms.</span><span class="sxs-lookup"><span data-stu-id="65ddd-126">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="65ddd-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="65ddd-127">Schema Name</span></span>  <br/> |<span data-ttu-id="65ddd-128">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="65ddd-128">Not available.</span></span>  <br/> |
|<span data-ttu-id="65ddd-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="65ddd-129">Validation File</span></span>  <br/> |<span data-ttu-id="65ddd-130">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="65ddd-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="65ddd-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="65ddd-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="65ddd-132">Faux</span><span class="sxs-lookup"><span data-stu-id="65ddd-132">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65ddd-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65ddd-133">See also</span></span>

- [<span data-ttu-id="65ddd-134">Éléments du fichier de configuration agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="65ddd-134">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

