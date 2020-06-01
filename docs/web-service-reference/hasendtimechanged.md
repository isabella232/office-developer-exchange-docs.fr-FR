---
title: HasEndTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0eb444d-8e2e-478b-b785-2b9787ffb226
description: L’élément HasEndTimeChanged spécifie si l’heure de fin d’une réunion a changé.
ms.openlocfilehash: 15ad52c7b7581cce5ca96ba5ff4e8a1c130a02cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461785"
---
# <a name="hasendtimechanged"></a><span data-ttu-id="79dd5-103">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="79dd5-103">HasEndTimeChanged</span></span>

<span data-ttu-id="79dd5-104">L’élément **HasEndTimeChanged** spécifie si l’heure de fin d’une réunion a changé.</span><span class="sxs-lookup"><span data-stu-id="79dd5-104">The **HasEndTimeChanged** element specifies whether the end time for a meeting has changed.</span></span> 
  
```XML
<HasEndTimeChanged>true | false</HasEndTimeChanged>
```

 <span data-ttu-id="79dd5-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="79dd5-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79dd5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="79dd5-106">Attributes and elements</span></span>

<span data-ttu-id="79dd5-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="79dd5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79dd5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="79dd5-108">Attributes</span></span>

<span data-ttu-id="79dd5-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="79dd5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79dd5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="79dd5-110">Child elements</span></span>

<span data-ttu-id="79dd5-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79dd5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79dd5-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="79dd5-112">Parent elements</span></span>

|<span data-ttu-id="79dd5-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="79dd5-113">**Element**</span></span>|<span data-ttu-id="79dd5-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="79dd5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79dd5-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="79dd5-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="79dd5-116">Spécifie les modifications apportées entre deux versions d’un message de demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="79dd5-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79dd5-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="79dd5-117">Text value</span></span>

<span data-ttu-id="79dd5-118">Une valeur de texte de **true** pour l’élément **HasEndTimeChanged** indique que l’heure de fin d’une réunion a changé.</span><span class="sxs-lookup"><span data-stu-id="79dd5-118">A text value of **true** for the **HasEndTimeChanged** element indicates that the end time of a meeting has changed.</span></span> <span data-ttu-id="79dd5-119">La valeur **false** indique que l’heure de fin d’une réunion n’a pas été modifiée.</span><span class="sxs-lookup"><span data-stu-id="79dd5-119">A value of **false** indicates that the end time of a meeting has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="79dd5-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="79dd5-120">Remarks</span></span>

<span data-ttu-id="79dd5-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="79dd5-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="79dd5-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="79dd5-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79dd5-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="79dd5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79dd5-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="79dd5-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79dd5-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="79dd5-125">Schema Name</span></span>  <br/> |<span data-ttu-id="79dd5-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="79dd5-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="79dd5-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="79dd5-127">Validation File</span></span>  <br/> |<span data-ttu-id="79dd5-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="79dd5-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="79dd5-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="79dd5-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="79dd5-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79dd5-130">See also</span></span>



- [<span data-ttu-id="79dd5-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="79dd5-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

