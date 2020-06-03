---
title: Configuration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- configuration
api_type:
- schema
ms.assetid: 6fc04e4d-657a-4999-9431-186ccb7832b5
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: b886851b9a0c17d58428f49281d664930d0e4070
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461561"
---
# <a name="configuration"></a><span data-ttu-id="4b7c3-103">Configuration</span><span class="sxs-lookup"><span data-stu-id="4b7c3-103">configuration</span></span>
  
<span data-ttu-id="4b7c3-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="4b7c3-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="4b7c3-105">L’élément **configuration** est l’élément racine du fichier de configuration des agents.</span><span class="sxs-lookup"><span data-stu-id="4b7c3-105">The **configuration** element is the root element for the agents configuration file.</span></span> 
  
- [<span data-ttu-id="4b7c3-106">configuration</span><span class="sxs-lookup"><span data-stu-id="4b7c3-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="4b7c3-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="4b7c3-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<configuration>
      <mexRuntime/>
</configuration>
```

<span data-ttu-id="4b7c3-108">**configurationType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="4b7c3-108">**configurationType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4b7c3-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4b7c3-109">Attributes and elements</span></span>

<span data-ttu-id="4b7c3-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4b7c3-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b7c3-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="4b7c3-111">Attributes</span></span>

<span data-ttu-id="4b7c3-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4b7c3-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b7c3-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4b7c3-113">Child elements</span></span>

|<span data-ttu-id="4b7c3-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b7c3-114">**Element**</span></span>|<span data-ttu-id="4b7c3-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b7c3-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b7c3-116">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="4b7c3-116">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="4b7c3-117">Contient des éléments qui définissent les informations de configuration des informations de configuration et de surveillance de l’agent pour les agents SMTP et de routage installés.</span><span class="sxs-lookup"><span data-stu-id="4b7c3-117">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b7c3-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4b7c3-118">Parent elements</span></span>

<span data-ttu-id="4b7c3-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4b7c3-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b7c3-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4b7c3-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b7c3-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4b7c3-121">Namespace</span></span>  <br/> |<span data-ttu-id="4b7c3-122">Ce fichier ne définit pas d’espace de noms.</span><span class="sxs-lookup"><span data-stu-id="4b7c3-122">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="4b7c3-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4b7c3-123">Schema Name</span></span>  <br/> |<span data-ttu-id="4b7c3-124">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="4b7c3-124">Not available.</span></span>  <br/> |
|<span data-ttu-id="4b7c3-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4b7c3-125">Validation File</span></span>  <br/> |<span data-ttu-id="4b7c3-126">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="4b7c3-126">Not available.</span></span>  <br/> |
|<span data-ttu-id="4b7c3-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4b7c3-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b7c3-128">Faux.</span><span class="sxs-lookup"><span data-stu-id="4b7c3-128">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b7c3-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4b7c3-129">See also</span></span>

- [<span data-ttu-id="4b7c3-130">Éléments du fichier de configuration des agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4b7c3-130">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

