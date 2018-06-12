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
description: L’élément DeletedOccurrence représente une occurrence d’un élément de calendrier périodique supprimée.
ms.openlocfilehash: f12a2ba20f87f7803e492d8422b68c8ecdf9d797
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755852"
---
# <a name="deletedoccurrence"></a><span data-ttu-id="b6dcb-103">DeletedOccurrence</span><span class="sxs-lookup"><span data-stu-id="b6dcb-103">DeletedOccurrence</span></span>

<span data-ttu-id="b6dcb-104">L’élément **DeletedOccurrence** représente une occurrence d’un élément de calendrier périodique supprimée.</span><span class="sxs-lookup"><span data-stu-id="b6dcb-104">The **DeletedOccurrence** element represents a deleted occurrence of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrence>
   <Start/>
</DeletedOccurrence>
```

 <span data-ttu-id="b6dcb-105">**DeletedOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="b6dcb-105">**DeletedOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6dcb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b6dcb-106">Attributes and elements</span></span>

<span data-ttu-id="b6dcb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b6dcb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6dcb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b6dcb-108">Attributes</span></span>

<span data-ttu-id="b6dcb-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b6dcb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6dcb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b6dcb-110">Child elements</span></span>

|<span data-ttu-id="b6dcb-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b6dcb-111">**Element**</span></span>|<span data-ttu-id="b6dcb-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b6dcb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6dcb-113">Début</span><span class="sxs-lookup"><span data-stu-id="b6dcb-113">Start</span></span>](start.md) <br/> |<span data-ttu-id="b6dcb-114">Représente l’heure de début d’une occurrence d’un élément de calendrier périodique supprimée.</span><span class="sxs-lookup"><span data-stu-id="b6dcb-114">Represents the start time of a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b6dcb-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b6dcb-115">Parent elements</span></span>

|<span data-ttu-id="b6dcb-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b6dcb-116">**Element**</span></span>|<span data-ttu-id="b6dcb-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b6dcb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6dcb-118">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="b6dcb-118">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="b6dcb-119">Contient un tableau d’occurrences supprimés d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="b6dcb-119">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b6dcb-120">Note</span><span class="sxs-lookup"><span data-stu-id="b6dcb-120">Remarks</span></span>

<span data-ttu-id="b6dcb-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b6dcb-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6dcb-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b6dcb-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6dcb-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b6dcb-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6dcb-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b6dcb-124">Schema name</span></span>  <br/> |<span data-ttu-id="b6dcb-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b6dcb-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="b6dcb-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b6dcb-126">Validation file</span></span>  <br/> |<span data-ttu-id="b6dcb-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b6dcb-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6dcb-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b6dcb-128">Can be empty</span></span>  <br/> |<span data-ttu-id="b6dcb-129">False</span><span class="sxs-lookup"><span data-stu-id="b6dcb-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6dcb-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b6dcb-130">See also</span></span>

- [<span data-ttu-id="b6dcb-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b6dcb-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="b6dcb-132">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b6dcb-132">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

