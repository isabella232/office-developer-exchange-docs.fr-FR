---
title: configuration
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
ms.openlocfilehash: 342e52e879534b6a130d286d358138c6095e4563
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755113"
---
# <a name="configuration"></a><span data-ttu-id="f3307-103">configuration</span><span class="sxs-lookup"><span data-stu-id="f3307-103">configuration</span></span>
  
<span data-ttu-id="f3307-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="f3307-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="f3307-105">L’élément de **configuration** est l’élément racine du fichier de configuration des agents.</span><span class="sxs-lookup"><span data-stu-id="f3307-105">The **configuration** element is the root element for the agents configuration file.</span></span> 
  
- [<span data-ttu-id="f3307-106">configuration</span><span class="sxs-lookup"><span data-stu-id="f3307-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="f3307-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="f3307-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<configuration>
      <mexRuntime/>
</configuration>
```

<span data-ttu-id="f3307-108">**configurationType (type complexe)**</span><span class="sxs-lookup"><span data-stu-id="f3307-108">**configurationType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f3307-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f3307-109">Attributes and elements</span></span>

<span data-ttu-id="f3307-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f3307-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3307-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="f3307-111">Attributes</span></span>

<span data-ttu-id="f3307-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f3307-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3307-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f3307-113">Child elements</span></span>

|<span data-ttu-id="f3307-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f3307-114">**Element**</span></span>|<span data-ttu-id="f3307-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="f3307-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3307-116">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="f3307-116">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="f3307-117">Contient des éléments qui définissent les informations de configuration pour l’agent de surveillance et les informations de configuration pour SMTP et les agents de routage qui sont installés.</span><span class="sxs-lookup"><span data-stu-id="f3307-117">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3307-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f3307-118">Parent elements</span></span>

<span data-ttu-id="f3307-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f3307-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3307-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f3307-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3307-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f3307-121">Namespace</span></span>  <br/> |<span data-ttu-id="f3307-122">Ce fichier ne définit pas un espace de noms.</span><span class="sxs-lookup"><span data-stu-id="f3307-122">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="f3307-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f3307-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f3307-124">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="f3307-124">Not available.</span></span>  <br/> |
|<span data-ttu-id="f3307-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f3307-125">Validation File</span></span>  <br/> |<span data-ttu-id="f3307-126">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="f3307-126">Not available.</span></span>  <br/> |
|<span data-ttu-id="f3307-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f3307-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3307-128">Faux</span><span class="sxs-lookup"><span data-stu-id="f3307-128">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3307-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f3307-129">See also</span></span>

- [<span data-ttu-id="f3307-130">Éléments du fichier de configuration agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f3307-130">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

