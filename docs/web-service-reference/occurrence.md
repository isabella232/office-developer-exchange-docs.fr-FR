---
title: Occurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: d292b99c-b896-40b7-be5d-2cb314c9481f
description: L’élément Occurrence représente une seule occurrence de modification d’un élément de calendrier périodique.
ms.openlocfilehash: 5a40faa9b885a235d30e7f41830d1eefe2ed23c3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828653"
---
# <a name="occurrence"></a><span data-ttu-id="8bcc7-103">Occurrence</span><span class="sxs-lookup"><span data-stu-id="8bcc7-103">Occurrence</span></span>

<span data-ttu-id="8bcc7-104">L’élément **Occurrence** représente une seule occurrence de modification d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="8bcc7-104">The **Occurrence** element represents a single modified occurrence of a recurring calendar item.</span></span> 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

<span data-ttu-id="8bcc7-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="8bcc7-105">**OccurrenceInfoType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8bcc7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8bcc7-106">Attributes and elements</span></span>

<span data-ttu-id="8bcc7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8bcc7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8bcc7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8bcc7-108">Attributes</span></span>

<span data-ttu-id="8bcc7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8bcc7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8bcc7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8bcc7-110">Child elements</span></span>

|<span data-ttu-id="8bcc7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8bcc7-111">**Element**</span></span>|<span data-ttu-id="8bcc7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8bcc7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8bcc7-113">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="8bcc7-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="8bcc7-114">Contient la clé unique identificateur et modification d’une occurrence de modification d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="8bcc7-114">Contains the unique identifier and change key of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8bcc7-115">Début</span><span class="sxs-lookup"><span data-stu-id="8bcc7-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="8bcc7-116">Représente l’heure de début d’une occurrence de modification d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="8bcc7-116">Represents the start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8bcc7-117">Fin</span><span class="sxs-lookup"><span data-stu-id="8bcc7-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8bcc7-118">Représente l’heure de fin d’une occurrence de modification d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="8bcc7-118">Represents the end time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8bcc7-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="8bcc7-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="8bcc7-120">Représente l’heure de début d’origine d’une occurrence de modification d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="8bcc7-120">Represents the original start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8bcc7-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8bcc7-121">Parent elements</span></span>

|<span data-ttu-id="8bcc7-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8bcc7-122">**Element**</span></span>|<span data-ttu-id="8bcc7-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="8bcc7-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8bcc7-124">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="8bcc7-124">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="8bcc7-125">Contient une collection d’occurrences d’élément calendrier périodiques qui ont été modifiés afin qu’ils soient différents de celui de l’élément maître de périodicité.</span><span class="sxs-lookup"><span data-stu-id="8bcc7-125">Contains a collection of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8bcc7-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="8bcc7-126">Remarks</span></span>

<span data-ttu-id="8bcc7-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8bcc7-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8bcc7-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8bcc7-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8bcc7-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8bcc7-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8bcc7-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8bcc7-130">Schema name</span></span>  <br/> |<span data-ttu-id="8bcc7-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8bcc7-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="8bcc7-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8bcc7-132">Validation file</span></span>  <br/> |<span data-ttu-id="8bcc7-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8bcc7-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8bcc7-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8bcc7-134">Can be empty</span></span>  <br/> |<span data-ttu-id="8bcc7-135">False</span><span class="sxs-lookup"><span data-stu-id="8bcc7-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8bcc7-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8bcc7-136">See also</span></span>

- [<span data-ttu-id="8bcc7-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8bcc7-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

