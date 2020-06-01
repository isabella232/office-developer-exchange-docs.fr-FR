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
description: L’élément DeletedOccurrences contient un tableau d’occurrences supprimées d’un élément de calendrier périodique.
ms.openlocfilehash: be39ff95b5529481a36b7549e638818a20e01283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463705"
---
# <a name="deletedoccurrences"></a><span data-ttu-id="c69ec-103">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="c69ec-103">DeletedOccurrences</span></span>

<span data-ttu-id="c69ec-104">L’élément **DeletedOccurrences** contient un tableau d’occurrences supprimées d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="c69ec-104">The **DeletedOccurrences** element contains an array of deleted occurrences of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrences>
   <DeletedOccurrence/>
</DeletedOccurrences>
```

 <span data-ttu-id="c69ec-105">**NonEmptyArrayOfDeletedOccurrencesType**</span><span class="sxs-lookup"><span data-stu-id="c69ec-105">**NonEmptyArrayOfDeletedOccurrencesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c69ec-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c69ec-106">Attributes and elements</span></span>

<span data-ttu-id="c69ec-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c69ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c69ec-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c69ec-108">Attributes</span></span>

<span data-ttu-id="c69ec-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c69ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c69ec-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c69ec-110">Child elements</span></span>

|<span data-ttu-id="c69ec-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c69ec-111">**Element**</span></span>|<span data-ttu-id="c69ec-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c69ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c69ec-113">DeletedOccurrence</span><span class="sxs-lookup"><span data-stu-id="c69ec-113">DeletedOccurrence</span></span>](deletedoccurrence.md) <br/> |<span data-ttu-id="c69ec-114">Représente une occurrence supprimée d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="c69ec-114">Represents a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c69ec-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c69ec-115">Parent elements</span></span>

|<span data-ttu-id="c69ec-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c69ec-116">**Element**</span></span>|<span data-ttu-id="c69ec-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c69ec-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c69ec-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c69ec-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c69ec-119">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="c69ec-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c69ec-120">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="c69ec-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c69ec-121">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c69ec-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c69ec-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="c69ec-122">Remarks</span></span>

<span data-ttu-id="c69ec-123">Cet élément est valide si la valeur de texte RecurringMaster est utilisée pour l’élément [CalendarItemType](calendaritemtype.md) .</span><span class="sxs-lookup"><span data-stu-id="c69ec-123">This element is valid if the RecurringMaster text value is used for the [CalendarItemType](calendaritemtype.md) element.</span></span> 
  
<span data-ttu-id="c69ec-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c69ec-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c69ec-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c69ec-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c69ec-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c69ec-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c69ec-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c69ec-127">Schema name</span></span>  <br/> |<span data-ttu-id="c69ec-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c69ec-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="c69ec-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c69ec-129">Validation file</span></span>  <br/> |<span data-ttu-id="c69ec-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c69ec-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c69ec-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c69ec-131">Can be empty</span></span>  <br/> |<span data-ttu-id="c69ec-132">False</span><span class="sxs-lookup"><span data-stu-id="c69ec-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c69ec-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c69ec-133">See also</span></span>

- [<span data-ttu-id="c69ec-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c69ec-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="c69ec-135">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="c69ec-135">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

