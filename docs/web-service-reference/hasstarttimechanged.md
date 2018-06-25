---
title: HasStartTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04a6968d-7fb5-47ee-b66e-dc99c35dbb63
description: L’élément HasStartTimeChanged Spécifie si l’heure de début d’une réunion a été modifiée.
ms.openlocfilehash: 2096084f4ec8848a63d10e0e80fdc7a37e473cd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827809"
---
# <a name="hasstarttimechanged"></a><span data-ttu-id="c84b1-103">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="c84b1-103">HasStartTimeChanged</span></span>

<span data-ttu-id="c84b1-104">L’élément **HasStartTimeChanged** Spécifie si l’heure de début d’une réunion a été modifiée.</span><span class="sxs-lookup"><span data-stu-id="c84b1-104">The **HasStartTimeChanged** element specifies whether the start time for a meeting has changed.</span></span> 
  
```XML
<HasStartTimeChanged> true | false </HasStartTimeChanged>
```

 <span data-ttu-id="c84b1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c84b1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c84b1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c84b1-106">Attributes and elements</span></span>

<span data-ttu-id="c84b1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c84b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c84b1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c84b1-108">Attributes</span></span>

<span data-ttu-id="c84b1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c84b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c84b1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c84b1-110">Child elements</span></span>

<span data-ttu-id="c84b1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c84b1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c84b1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c84b1-112">Parent elements</span></span>

|<span data-ttu-id="c84b1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c84b1-113">**Element**</span></span>|<span data-ttu-id="c84b1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="c84b1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c84b1-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="c84b1-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="c84b1-116">Spécifie ce qui a changé entre deux versions d’une réunion message de demande.</span><span class="sxs-lookup"><span data-stu-id="c84b1-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c84b1-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c84b1-117">Text value</span></span>

<span data-ttu-id="c84b1-118">Une valeur de texte de **la valeur true** pour l’élément **HasStartTimeChanged** indique que l’heure de début d’une réunion a été modifiée.</span><span class="sxs-lookup"><span data-stu-id="c84b1-118">A text value of **true** for the **HasStartTimeChanged** element indicates that the start time for a meeting has changed.</span></span> <span data-ttu-id="c84b1-119">La valeur **false** indique que l’heure de début n’a pas changé.</span><span class="sxs-lookup"><span data-stu-id="c84b1-119">A value of **false** indicates that the start time has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c84b1-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="c84b1-120">Remarks</span></span>

<span data-ttu-id="c84b1-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c84b1-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c84b1-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c84b1-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c84b1-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c84b1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c84b1-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c84b1-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c84b1-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c84b1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c84b1-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="c84b1-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="c84b1-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="c84b1-127">Validation File</span></span>  <br/> |<span data-ttu-id="c84b1-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="c84b1-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c84b1-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c84b1-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c84b1-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c84b1-130">See also</span></span>



- [<span data-ttu-id="c84b1-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c84b1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

