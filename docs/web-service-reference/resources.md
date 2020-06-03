---
title: Ressources
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Resources
api_type:
- schema
ms.assetid: a2133cf2-7c62-4f1c-b3aa-75f14d30dd74
description: L’élément Resources représente une ressource planifiée pour une réunion.
ms.openlocfilehash: 67b4ed93a67a48945845887aa2d08b5bfe0102d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455589"
---
# <a name="resources"></a><span data-ttu-id="1e96c-103">Ressources</span><span class="sxs-lookup"><span data-stu-id="1e96c-103">Resources</span></span>

<span data-ttu-id="1e96c-104">L’élément **Resources** représente une ressource planifiée pour une réunion.</span><span class="sxs-lookup"><span data-stu-id="1e96c-104">The **Resources** element represents a scheduled resource for a meeting.</span></span> 
  
```xml
<Resources>
   <Attendee/>
</Resources>
```

 <span data-ttu-id="1e96c-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="1e96c-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e96c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1e96c-106">Attributes and elements</span></span>

<span data-ttu-id="1e96c-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1e96c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e96c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1e96c-108">Attributes</span></span>

<span data-ttu-id="1e96c-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1e96c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e96c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1e96c-110">Child elements</span></span>

|<span data-ttu-id="1e96c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1e96c-111">**Element**</span></span>|<span data-ttu-id="1e96c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e96c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e96c-113">Participant</span><span class="sxs-lookup"><span data-stu-id="1e96c-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="1e96c-114">Représente les participants et les ressources d’une réunion.</span><span class="sxs-lookup"><span data-stu-id="1e96c-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1e96c-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1e96c-115">Parent elements</span></span>

|<span data-ttu-id="1e96c-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1e96c-116">**Element**</span></span>|<span data-ttu-id="1e96c-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e96c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e96c-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="1e96c-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="1e96c-119">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e96c-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="1e96c-120">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="1e96c-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="1e96c-121">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e96c-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1e96c-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="1e96c-122">Remarks</span></span>

<span data-ttu-id="1e96c-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1e96c-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e96c-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1e96c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e96c-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1e96c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1e96c-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1e96c-126">Schema name</span></span>  <br/> |<span data-ttu-id="1e96c-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1e96c-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="1e96c-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1e96c-128">Validation file</span></span>  <br/> |<span data-ttu-id="1e96c-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1e96c-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1e96c-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1e96c-130">Can be empty</span></span>  <br/> |<span data-ttu-id="1e96c-131">False</span><span class="sxs-lookup"><span data-stu-id="1e96c-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e96c-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1e96c-132">See also</span></span>



- [<span data-ttu-id="1e96c-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1e96c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

