---
title: HasStartTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04a6968d-7fb5-47ee-b66e-dc99c35dbb63
description: L’élément HasStartTimeChanged spécifie si l’heure de début d’une réunion a changé.
ms.openlocfilehash: 1355917005d956d05064bfc095055fb72aa16c57
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462744"
---
# <a name="hasstarttimechanged"></a><span data-ttu-id="49214-103">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="49214-103">HasStartTimeChanged</span></span>

<span data-ttu-id="49214-104">L’élément **HasStartTimeChanged** spécifie si l’heure de début d’une réunion a changé.</span><span class="sxs-lookup"><span data-stu-id="49214-104">The **HasStartTimeChanged** element specifies whether the start time for a meeting has changed.</span></span> 
  
```XML
<HasStartTimeChanged> true | false </HasStartTimeChanged>
```

 <span data-ttu-id="49214-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="49214-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49214-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="49214-106">Attributes and elements</span></span>

<span data-ttu-id="49214-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="49214-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49214-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="49214-108">Attributes</span></span>

<span data-ttu-id="49214-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="49214-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49214-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="49214-110">Child elements</span></span>

<span data-ttu-id="49214-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="49214-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="49214-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="49214-112">Parent elements</span></span>

|<span data-ttu-id="49214-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="49214-113">**Element**</span></span>|<span data-ttu-id="49214-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="49214-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49214-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="49214-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="49214-116">Spécifie les modifications apportées entre deux versions d’un message de demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="49214-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="49214-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="49214-117">Text value</span></span>

<span data-ttu-id="49214-118">Une valeur de texte de **true** pour l’élément **HasStartTimeChanged** indique que l’heure de début d’une réunion a changé.</span><span class="sxs-lookup"><span data-stu-id="49214-118">A text value of **true** for the **HasStartTimeChanged** element indicates that the start time for a meeting has changed.</span></span> <span data-ttu-id="49214-119">La valeur **false** indique que l’heure de début n’a pas changé.</span><span class="sxs-lookup"><span data-stu-id="49214-119">A value of **false** indicates that the start time has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="49214-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="49214-120">Remarks</span></span>

<span data-ttu-id="49214-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="49214-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="49214-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="49214-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49214-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="49214-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49214-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="49214-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49214-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="49214-125">Schema Name</span></span>  <br/> |<span data-ttu-id="49214-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="49214-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="49214-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="49214-127">Validation File</span></span>  <br/> |<span data-ttu-id="49214-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="49214-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="49214-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="49214-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="49214-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="49214-130">See also</span></span>



- [<span data-ttu-id="49214-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="49214-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

