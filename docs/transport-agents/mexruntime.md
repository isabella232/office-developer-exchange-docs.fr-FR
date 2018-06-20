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
ms.openlocfilehash: 4a34eedfc16d64cbfa67003ed23cf6eba2bb4bad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755143"
---
# <a name="mexruntime"></a><span data-ttu-id="08f1b-103">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="08f1b-103">mexRuntime</span></span>
  
<span data-ttu-id="08f1b-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="08f1b-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="08f1b-105">L’élément **mexRuntime** contienne les éléments qui définissent les informations de configuration pour l’agent de surveillance et les informations de configuration pour SMTP et les agents de routage qui sont installés.</span><span class="sxs-lookup"><span data-stu-id="08f1b-105">The **mexRuntime** element contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span> 
  
- [<span data-ttu-id="08f1b-106">configuration</span><span class="sxs-lookup"><span data-stu-id="08f1b-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="08f1b-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="08f1b-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

<span data-ttu-id="08f1b-108">**mexRuntimeType (type complexe)**</span><span class="sxs-lookup"><span data-stu-id="08f1b-108">**mexRuntimeType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="08f1b-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="08f1b-109">Attributes and elements</span></span>

<span data-ttu-id="08f1b-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="08f1b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08f1b-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="08f1b-111">Attributes</span></span>

<span data-ttu-id="08f1b-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08f1b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08f1b-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="08f1b-113">Child elements</span></span>

|<span data-ttu-id="08f1b-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="08f1b-114">**Element**</span></span>|<span data-ttu-id="08f1b-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="08f1b-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08f1b-116">surveillance</span><span class="sxs-lookup"><span data-stu-id="08f1b-116">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="08f1b-117">Contient des informations de configuration qui définit comment et quand transport analyse les agents qui sont installés.</span><span class="sxs-lookup"><span data-stu-id="08f1b-117">Contains configuration information that defines how and when transport monitors agents that are installed.</span></span>  <br/> |
|[<span data-ttu-id="08f1b-118">agentList</span><span class="sxs-lookup"><span data-stu-id="08f1b-118">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="08f1b-119">Contient un élément de [l’agent](agent.md) pour chaque agent qui est installé.</span><span class="sxs-lookup"><span data-stu-id="08f1b-119">Contains an [agent](agent.md) element for each agent that is installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08f1b-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="08f1b-120">Parent elements</span></span>

|<span data-ttu-id="08f1b-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="08f1b-121">**Element**</span></span>|<span data-ttu-id="08f1b-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="08f1b-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08f1b-123">configuration</span><span class="sxs-lookup"><span data-stu-id="08f1b-123">configuration</span></span>](configuration.md) <br/> |<span data-ttu-id="08f1b-124">L’élément racine du fichier de configuration des agents.</span><span class="sxs-lookup"><span data-stu-id="08f1b-124">The root element for the agents configuration file.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="08f1b-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="08f1b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08f1b-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="08f1b-126">Namespace</span></span>  <br/> |<span data-ttu-id="08f1b-127">Ce fichier ne définit pas un espace de noms.</span><span class="sxs-lookup"><span data-stu-id="08f1b-127">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="08f1b-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="08f1b-128">Schema Name</span></span>  <br/> |<span data-ttu-id="08f1b-129">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="08f1b-129">Not available.</span></span>  <br/> |
|<span data-ttu-id="08f1b-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="08f1b-130">Validation File</span></span>  <br/> |<span data-ttu-id="08f1b-131">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="08f1b-131">Not available.</span></span>  <br/> |
|<span data-ttu-id="08f1b-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="08f1b-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="08f1b-133">Faux</span><span class="sxs-lookup"><span data-stu-id="08f1b-133">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08f1b-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="08f1b-134">See also</span></span>

- [<span data-ttu-id="08f1b-135">Éléments du fichier de configuration agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="08f1b-135">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

