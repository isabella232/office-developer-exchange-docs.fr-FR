---
title: DeletedOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedOccurrences
api_type:
- schema
ms.assetid: 736fb305-9528-4be8-ad37-65d7556edbf2
description: L’élément DeletedOccurrences contient un tableau d’occurrences supprimés d’un élément de calendrier périodique.
ms.openlocfilehash: 269c1176913cd642f93987462286dd1fee3a7339
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755856"
---
# <a name="deletedoccurrences"></a><span data-ttu-id="c4d6c-103">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="c4d6c-103">DeletedOccurrences</span></span>

<span data-ttu-id="c4d6c-104">L’élément **DeletedOccurrences** contient un tableau d’occurrences supprimés d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="c4d6c-104">The **DeletedOccurrences** element contains an array of deleted occurrences of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrences>
   <DeletedOccurrence/>
</DeletedOccurrences>
```

 <span data-ttu-id="c4d6c-105">**NonEmptyArrayOfDeletedOccurrencesType**</span><span class="sxs-lookup"><span data-stu-id="c4d6c-105">**NonEmptyArrayOfDeletedOccurrencesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4d6c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c4d6c-106">Attributes and elements</span></span>

<span data-ttu-id="c4d6c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c4d6c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4d6c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c4d6c-108">Attributes</span></span>

<span data-ttu-id="c4d6c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c4d6c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4d6c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c4d6c-110">Child elements</span></span>

|<span data-ttu-id="c4d6c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c4d6c-111">**Element**</span></span>|<span data-ttu-id="c4d6c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c4d6c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4d6c-113">DeletedOccurrence</span><span class="sxs-lookup"><span data-stu-id="c4d6c-113">DeletedOccurrence</span></span>](deletedoccurrence.md) <br/> |<span data-ttu-id="c4d6c-114">Représente une occurrence d’un élément de calendrier périodique supprimée.</span><span class="sxs-lookup"><span data-stu-id="c4d6c-114">Represents a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c4d6c-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c4d6c-115">Parent elements</span></span>

|<span data-ttu-id="c4d6c-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c4d6c-116">**Element**</span></span>|<span data-ttu-id="c4d6c-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c4d6c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4d6c-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c4d6c-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c4d6c-119">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4d6c-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c4d6c-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c4d6c-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c4d6c-121">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4d6c-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c4d6c-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="c4d6c-122">Remarks</span></span>

<span data-ttu-id="c4d6c-123">Cet élément n’est valide que si la valeur de texte RecurringMaster est utilisée pour l’élément [CalendarItemType](calendaritemtype.md) .</span><span class="sxs-lookup"><span data-stu-id="c4d6c-123">This element is valid if the RecurringMaster text value is used for the [CalendarItemType](calendaritemtype.md) element.</span></span> 
  
<span data-ttu-id="c4d6c-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c4d6c-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4d6c-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c4d6c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4d6c-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c4d6c-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c4d6c-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c4d6c-127">Schema name</span></span>  <br/> |<span data-ttu-id="c4d6c-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c4d6c-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="c4d6c-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c4d6c-129">Validation file</span></span>  <br/> |<span data-ttu-id="c4d6c-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c4d6c-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c4d6c-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c4d6c-131">Can be empty</span></span>  <br/> |<span data-ttu-id="c4d6c-132">False</span><span class="sxs-lookup"><span data-stu-id="c4d6c-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4d6c-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c4d6c-133">See also</span></span>

- [<span data-ttu-id="c4d6c-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c4d6c-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="c4d6c-135">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="c4d6c-135">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

