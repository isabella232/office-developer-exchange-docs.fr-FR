---
title: DeleteFromFolderStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3aba59a0-f12a-48b5-842b-11cf4530dd51
description: L’élément DeleteFromFolderStateDefinition spécifie l’État lorsqu’un élément est supprimé d’un dossier.
ms.openlocfilehash: 0ea8c61a6839790869781d5d87ca81772b2e38d6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455722"
---
# <a name="deletefromfolderstatedefinition"></a><span data-ttu-id="f7c60-103">DeleteFromFolderStateDefinition</span><span class="sxs-lookup"><span data-stu-id="f7c60-103">DeleteFromFolderStateDefinition</span></span>

<span data-ttu-id="f7c60-104">L’élément **DeleteFromFolderStateDefinition** spécifie l’État lorsqu’un élément est supprimé d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="f7c60-104">The **DeleteFromFolderStateDefinition** element specifies the state when an item is deleted from a folder.</span></span> 
  
```XML
<DeleteFromFolderStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeleteFromFolderStateDefinition>
```

 <span data-ttu-id="f7c60-105">**DeleteFromFolderStateDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="f7c60-105">**DeleteFromFolderStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7c60-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f7c60-106">Attributes and elements</span></span>

<span data-ttu-id="f7c60-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f7c60-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7c60-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f7c60-108">Attributes</span></span>

<span data-ttu-id="f7c60-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f7c60-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7c60-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f7c60-110">Child elements</span></span>

|<span data-ttu-id="f7c60-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7c60-111">**Element**</span></span>|<span data-ttu-id="f7c60-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7c60-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7c60-113">Occurrence (transition de fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="f7c60-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="f7c60-114">Spécifie la date de l’occurrence d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="f7c60-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f7c60-115">IsOccurrencePresent</span><span class="sxs-lookup"><span data-stu-id="f7c60-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="f7c60-116">Spécifie une valeur de type Boolean qui indique si une occurrence de l’élément de calendrier est présente.</span><span class="sxs-lookup"><span data-stu-id="f7c60-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7c60-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f7c60-117">Parent elements</span></span>

|<span data-ttu-id="f7c60-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7c60-118">**Element**</span></span>|<span data-ttu-id="f7c60-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7c60-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7c60-120">StateDefinition</span><span class="sxs-lookup"><span data-stu-id="f7c60-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="f7c60-121">Spécifie une définition d’État.</span><span class="sxs-lookup"><span data-stu-id="f7c60-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f7c60-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="f7c60-122">Remarks</span></span>

<span data-ttu-id="f7c60-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f7c60-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f7c60-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7c60-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7c60-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f7c60-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7c60-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f7c60-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7c60-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f7c60-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f7c60-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="f7c60-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="f7c60-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="f7c60-129">Validation File</span></span>  <br/> |<span data-ttu-id="f7c60-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="f7c60-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7c60-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f7c60-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f7c60-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f7c60-132">See also</span></span>

- [<span data-ttu-id="f7c60-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f7c60-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

