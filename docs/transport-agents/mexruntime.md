---
title: mexRuntime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: f192965a8375eb46d1ca5b46d3b768a3299c284d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461834"
---
# <a name="mexruntime"></a><span data-ttu-id="6be09-103">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="6be09-103">mexRuntime</span></span>
  
<span data-ttu-id="6be09-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="6be09-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="6be09-105">L’élément **mexRuntime** contient des éléments qui définissent les informations de configuration des informations de configuration et de surveillance de l’agent pour les agents SMTP et de routage installés.</span><span class="sxs-lookup"><span data-stu-id="6be09-105">The **mexRuntime** element contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span> 
  
- [<span data-ttu-id="6be09-106">configuration</span><span class="sxs-lookup"><span data-stu-id="6be09-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="6be09-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="6be09-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

<span data-ttu-id="6be09-108">**mexRuntimeType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="6be09-108">**mexRuntimeType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6be09-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6be09-109">Attributes and elements</span></span>

<span data-ttu-id="6be09-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6be09-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6be09-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="6be09-111">Attributes</span></span>

<span data-ttu-id="6be09-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6be09-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6be09-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6be09-113">Child elements</span></span>

|<span data-ttu-id="6be09-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6be09-114">**Element**</span></span>|<span data-ttu-id="6be09-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="6be09-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6be09-116">surveillance</span><span class="sxs-lookup"><span data-stu-id="6be09-116">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="6be09-117">Contient des informations de configuration qui définissent comment et quand le transport surveille les agents installés.</span><span class="sxs-lookup"><span data-stu-id="6be09-117">Contains configuration information that defines how and when transport monitors agents that are installed.</span></span>  <br/> |
|[<span data-ttu-id="6be09-118">agentList</span><span class="sxs-lookup"><span data-stu-id="6be09-118">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="6be09-119">Contient un élément [agent](agent.md) pour chaque agent installé.</span><span class="sxs-lookup"><span data-stu-id="6be09-119">Contains an [agent](agent.md) element for each agent that is installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6be09-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6be09-120">Parent elements</span></span>

|<span data-ttu-id="6be09-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6be09-121">**Element**</span></span>|<span data-ttu-id="6be09-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="6be09-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6be09-123">configuration</span><span class="sxs-lookup"><span data-stu-id="6be09-123">configuration</span></span>](configuration.md) <br/> |<span data-ttu-id="6be09-124">Élément racine du fichier de configuration des agents.</span><span class="sxs-lookup"><span data-stu-id="6be09-124">The root element for the agents configuration file.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="6be09-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6be09-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6be09-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6be09-126">Namespace</span></span>  <br/> |<span data-ttu-id="6be09-127">Ce fichier ne définit pas d’espace de noms.</span><span class="sxs-lookup"><span data-stu-id="6be09-127">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="6be09-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6be09-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6be09-129">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="6be09-129">Not available.</span></span>  <br/> |
|<span data-ttu-id="6be09-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6be09-130">Validation File</span></span>  <br/> |<span data-ttu-id="6be09-131">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="6be09-131">Not available.</span></span>  <br/> |
|<span data-ttu-id="6be09-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6be09-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="6be09-133">Faux.</span><span class="sxs-lookup"><span data-stu-id="6be09-133">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6be09-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6be09-134">See also</span></span>

- [<span data-ttu-id="6be09-135">Éléments du fichier de configuration des agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6be09-135">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

