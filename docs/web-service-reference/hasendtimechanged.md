---
title: HasEndTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0eb444d-8e2e-478b-b785-2b9787ffb226
description: L’élément HasEndTimeChanged Spécifie si l’heure de fin d’une réunion a été modifiée.
ms.openlocfilehash: 046bb302d6f7052c6f1757ce393583b305311e2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827805"
---
# <a name="hasendtimechanged"></a><span data-ttu-id="74e02-103">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="74e02-103">HasEndTimeChanged</span></span>

<span data-ttu-id="74e02-104">L’élément **HasEndTimeChanged** Spécifie si l’heure de fin d’une réunion a été modifiée.</span><span class="sxs-lookup"><span data-stu-id="74e02-104">The **HasEndTimeChanged** element specifies whether the end time for a meeting has changed.</span></span> 
  
```XML
<HasEndTimeChanged>true | false</HasEndTimeChanged>
```

 <span data-ttu-id="74e02-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="74e02-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74e02-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="74e02-106">Attributes and elements</span></span>

<span data-ttu-id="74e02-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="74e02-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74e02-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="74e02-108">Attributes</span></span>

<span data-ttu-id="74e02-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="74e02-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74e02-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="74e02-110">Child elements</span></span>

<span data-ttu-id="74e02-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="74e02-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="74e02-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="74e02-112">Parent elements</span></span>

|<span data-ttu-id="74e02-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="74e02-113">**Element**</span></span>|<span data-ttu-id="74e02-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="74e02-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74e02-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="74e02-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="74e02-116">Spécifie ce qui a changé entre deux versions d’une réunion message de demande.</span><span class="sxs-lookup"><span data-stu-id="74e02-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74e02-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="74e02-117">Text value</span></span>

<span data-ttu-id="74e02-118">Une valeur de texte de **la valeur true** pour l’élément **HasEndTimeChanged** indique que l’heure de fin d’une réunion a été modifiée.</span><span class="sxs-lookup"><span data-stu-id="74e02-118">A text value of **true** for the **HasEndTimeChanged** element indicates that the end time of a meeting has changed.</span></span> <span data-ttu-id="74e02-119">La valeur **false** indique que l’heure de fin d’une réunion n’a pas changé.</span><span class="sxs-lookup"><span data-stu-id="74e02-119">A value of **false** indicates that the end time of a meeting has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="74e02-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="74e02-120">Remarks</span></span>

<span data-ttu-id="74e02-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="74e02-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="74e02-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="74e02-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74e02-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="74e02-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74e02-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="74e02-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="74e02-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="74e02-125">Schema Name</span></span>  <br/> |<span data-ttu-id="74e02-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="74e02-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="74e02-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="74e02-127">Validation File</span></span>  <br/> |<span data-ttu-id="74e02-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="74e02-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="74e02-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="74e02-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="74e02-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="74e02-130">See also</span></span>



- [<span data-ttu-id="74e02-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="74e02-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

