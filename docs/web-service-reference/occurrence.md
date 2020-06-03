---
title: Réunions
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
description: L’élément occurrence représente une occurrence modifiée unique d’un élément de calendrier périodique.
ms.openlocfilehash: c3a6bcce23f0bb1125dbd2a5bb86e9b20039a4e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466317"
---
# <a name="occurrence"></a><span data-ttu-id="71f47-103">Réunions</span><span class="sxs-lookup"><span data-stu-id="71f47-103">Occurrence</span></span>

<span data-ttu-id="71f47-104">L’élément **occurrence** représente une occurrence modifiée unique d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="71f47-104">The **Occurrence** element represents a single modified occurrence of a recurring calendar item.</span></span> 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

<span data-ttu-id="71f47-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="71f47-105">**OccurrenceInfoType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="71f47-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="71f47-106">Attributes and elements</span></span>

<span data-ttu-id="71f47-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="71f47-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71f47-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="71f47-108">Attributes</span></span>

<span data-ttu-id="71f47-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="71f47-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71f47-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="71f47-110">Child elements</span></span>

|<span data-ttu-id="71f47-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="71f47-111">**Element**</span></span>|<span data-ttu-id="71f47-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="71f47-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71f47-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="71f47-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="71f47-114">Contient l’identificateur unique et la clé de modification d’une occurrence modifiée d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="71f47-114">Contains the unique identifier and change key of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="71f47-115">Démarrage</span><span class="sxs-lookup"><span data-stu-id="71f47-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="71f47-116">Représente l’heure de début d’une occurrence modifiée d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="71f47-116">Represents the start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="71f47-117">Fin</span><span class="sxs-lookup"><span data-stu-id="71f47-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="71f47-118">Représente l’heure de fin d’une occurrence modifiée d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="71f47-118">Represents the end time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="71f47-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="71f47-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="71f47-120">Représente l’heure de début d’origine d’une occurrence modifiée d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="71f47-120">Represents the original start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71f47-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="71f47-121">Parent elements</span></span>

|<span data-ttu-id="71f47-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="71f47-122">**Element**</span></span>|<span data-ttu-id="71f47-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="71f47-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71f47-124">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="71f47-124">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="71f47-125">Contient une collection d’occurrences de calendrier périodiques qui ont été modifiées afin qu’elles soient différentes de l’élément de masque de récurrence.</span><span class="sxs-lookup"><span data-stu-id="71f47-125">Contains a collection of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="71f47-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="71f47-126">Remarks</span></span>

<span data-ttu-id="71f47-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="71f47-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71f47-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="71f47-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71f47-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="71f47-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71f47-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="71f47-130">Schema name</span></span>  <br/> |<span data-ttu-id="71f47-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="71f47-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="71f47-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="71f47-132">Validation file</span></span>  <br/> |<span data-ttu-id="71f47-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="71f47-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71f47-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="71f47-134">Can be empty</span></span>  <br/> |<span data-ttu-id="71f47-135">False</span><span class="sxs-lookup"><span data-stu-id="71f47-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71f47-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="71f47-136">See also</span></span>

- [<span data-ttu-id="71f47-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="71f47-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

