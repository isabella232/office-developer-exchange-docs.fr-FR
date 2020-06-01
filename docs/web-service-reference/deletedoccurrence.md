---
title: DeletedOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedOccurrence
api_type:
- schema
ms.assetid: ff24ea15-0cd7-407d-a378-73ec16451870
description: L’élément DeletedOccurrence représente une occurrence supprimée d’un élément de calendrier périodique.
ms.openlocfilehash: 814a81934786963ae5e7ea3a40406834c27b64ce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457836"
---
# <a name="deletedoccurrence"></a><span data-ttu-id="badc3-103">DeletedOccurrence</span><span class="sxs-lookup"><span data-stu-id="badc3-103">DeletedOccurrence</span></span>

<span data-ttu-id="badc3-104">L’élément **DeletedOccurrence** représente une occurrence supprimée d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="badc3-104">The **DeletedOccurrence** element represents a deleted occurrence of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrence>
   <Start/>
</DeletedOccurrence>
```

 <span data-ttu-id="badc3-105">**DeletedOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="badc3-105">**DeletedOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="badc3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="badc3-106">Attributes and elements</span></span>

<span data-ttu-id="badc3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="badc3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="badc3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="badc3-108">Attributes</span></span>

<span data-ttu-id="badc3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="badc3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="badc3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="badc3-110">Child elements</span></span>

|<span data-ttu-id="badc3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="badc3-111">**Element**</span></span>|<span data-ttu-id="badc3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="badc3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="badc3-113">Start</span><span class="sxs-lookup"><span data-stu-id="badc3-113">Start</span></span>](start.md) <br/> |<span data-ttu-id="badc3-114">Représente l’heure de début d’une occurrence supprimée d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="badc3-114">Represents the start time of a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="badc3-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="badc3-115">Parent elements</span></span>

|<span data-ttu-id="badc3-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="badc3-116">**Element**</span></span>|<span data-ttu-id="badc3-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="badc3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="badc3-118">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="badc3-118">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="badc3-119">Contient un tableau d’occurrences supprimées d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="badc3-119">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="badc3-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="badc3-120">Remarks</span></span>

<span data-ttu-id="badc3-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="badc3-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="badc3-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="badc3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="badc3-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="badc3-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="badc3-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="badc3-124">Schema name</span></span>  <br/> |<span data-ttu-id="badc3-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="badc3-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="badc3-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="badc3-126">Validation file</span></span>  <br/> |<span data-ttu-id="badc3-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="badc3-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="badc3-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="badc3-128">Can be empty</span></span>  <br/> |<span data-ttu-id="badc3-129">False</span><span class="sxs-lookup"><span data-stu-id="badc3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="badc3-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="badc3-130">See also</span></span>

- [<span data-ttu-id="badc3-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="badc3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="badc3-132">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="badc3-132">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

