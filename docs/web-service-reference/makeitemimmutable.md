---
title: MakeItemImmutable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: L’élément MakeItemImmutable spécifie une valeur de type Boolean qui indique si un élément doit être effectué en lecture seule.
ms.openlocfilehash: 63c05fd3572c7b4ab93fe098d9165a117849ef02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828337"
---
# <a name="makeitemimmutable"></a><span data-ttu-id="efb37-103">MakeItemImmutable</span><span class="sxs-lookup"><span data-stu-id="efb37-103">MakeItemImmutable</span></span>

<span data-ttu-id="efb37-104">L’élément **MakeItemImmutable** spécifie une valeur de type Boolean qui indique si un élément doit être effectué en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="efb37-104">The **MakeItemImmutable** element specifies a Boolean value that indicates whether an item should be made read-only.</span></span> 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 <span data-ttu-id="efb37-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="efb37-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="efb37-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="efb37-106">Attributes and elements</span></span>

<span data-ttu-id="efb37-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="efb37-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="efb37-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="efb37-108">Attributes</span></span>

<span data-ttu-id="efb37-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="efb37-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="efb37-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="efb37-110">Child elements</span></span>

<span data-ttu-id="efb37-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="efb37-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="efb37-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="efb37-112">Parent elements</span></span>

[<span data-ttu-id="efb37-113">UpdateItemInRecoverableItems</span><span class="sxs-lookup"><span data-stu-id="efb37-113">UpdateItemInRecoverableItems</span></span>](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a><span data-ttu-id="efb37-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="efb37-114">Text value</span></span>

<span data-ttu-id="efb37-115">Une valeur de texte de **la valeur true** pour l’élément **MakeItemImmutable** indique que l’élément doit être mis en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="efb37-115">A text value of **true** for the **MakeItemImmutable** element indicates that the item should be made read-only.</span></span> <span data-ttu-id="efb37-116">La valeur **false** indique que l’élément autorise l’accès en lecture-écriture.</span><span class="sxs-lookup"><span data-stu-id="efb37-116">A value of **false** indicates that the item allows read-write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="efb37-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="efb37-117">Remarks</span></span>

<span data-ttu-id="efb37-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="efb37-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="efb37-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="efb37-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="efb37-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="efb37-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="efb37-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="efb37-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="efb37-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="efb37-122">Schema name</span></span>  <br/> |<span data-ttu-id="efb37-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="efb37-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="efb37-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="efb37-124">Validation file</span></span>  <br/> |<span data-ttu-id="efb37-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="efb37-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="efb37-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="efb37-126">Can be empty</span></span>  <br/> ||
   

