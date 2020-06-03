---
title: IsExternalMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5cc83174-e684-42c8-b72a-f82d3de3bb2f
description: L’élément IsExternalMailbox indique si la boîte aux lettres est externe à l’organisation.
ms.openlocfilehash: 9be702b05e89857913023a8ec34b78ea4c309274
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455288"
---
# <a name="isexternalmailbox"></a><span data-ttu-id="77a89-103">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="77a89-103">IsExternalMailbox</span></span>

<span data-ttu-id="77a89-104">L’élément **IsExternalMailbox** indique si la boîte aux lettres est externe à l’organisation.</span><span class="sxs-lookup"><span data-stu-id="77a89-104">The **IsExternalMailbox** element indicates whether the mailbox is external to the organization.</span></span> 
  
```XML
<IsExternalMailbox>true | false</IsExternalMailbox>
```

 <span data-ttu-id="77a89-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="77a89-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77a89-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="77a89-106">Attributes and elements</span></span>

<span data-ttu-id="77a89-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="77a89-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77a89-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="77a89-108">Attributes</span></span>

<span data-ttu-id="77a89-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="77a89-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77a89-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="77a89-110">Child elements</span></span>

<span data-ttu-id="77a89-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="77a89-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="77a89-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="77a89-112">Parent elements</span></span>

[<span data-ttu-id="77a89-113">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="77a89-113">SearchableMailbox</span></span>](searchablemailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="77a89-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="77a89-114">Text value</span></span>

<span data-ttu-id="77a89-115">Une valeur de texte de **true** pour l’élément **IsExternalMailbox** indique que la boîte aux lettres se trouve dans une organisation externe.</span><span class="sxs-lookup"><span data-stu-id="77a89-115">A text value of **true** for the **IsExternalMailbox** element indicates that the mailbox is in an external organization.</span></span> <span data-ttu-id="77a89-116">La valeur **false** indique que la boîte aux lettres se trouve dans l’organisation.</span><span class="sxs-lookup"><span data-stu-id="77a89-116">A value of **false** indicates that the mailbox is in the organization.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="77a89-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="77a89-117">Remarks</span></span>

<span data-ttu-id="77a89-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="77a89-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="77a89-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="77a89-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77a89-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="77a89-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77a89-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="77a89-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="77a89-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="77a89-122">Schema name</span></span>  <br/> |<span data-ttu-id="77a89-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="77a89-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="77a89-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="77a89-124">Validation file</span></span>  <br/> |<span data-ttu-id="77a89-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="77a89-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="77a89-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="77a89-126">Can be empty</span></span>  <br/> |<span data-ttu-id="77a89-127">False</span><span class="sxs-lookup"><span data-stu-id="77a89-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77a89-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="77a89-128">See also</span></span>



- [<span data-ttu-id="77a89-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="77a89-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

