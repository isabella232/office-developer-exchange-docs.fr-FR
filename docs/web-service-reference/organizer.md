---
title: Organisateur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Organizer
api_type:
- schema
ms.assetid: 63892b57-3805-4d60-b9f7-20552a69c241
description: L’élément de bibliothèque multimédia représente l’organisateur d’une réunion.
ms.openlocfilehash: b723578a1b52cd5f6e9bd869a15430453adfa291
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828662"
---
# <a name="organizer"></a><span data-ttu-id="3501e-103">Organisateur</span><span class="sxs-lookup"><span data-stu-id="3501e-103">Organizer</span></span>

<span data-ttu-id="3501e-104">L’élément de **bibliothèque multimédia** représente l’organisateur d’une réunion.</span><span class="sxs-lookup"><span data-stu-id="3501e-104">The **Organizer** element represents the organizer of a meeting.</span></span> 
  
```xml
<Organizer>
   <Mailbox/>
</Organizer>
```

<span data-ttu-id="3501e-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="3501e-105">**SingleRecipientType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3501e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3501e-106">Attributes and elements</span></span>

<span data-ttu-id="3501e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3501e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3501e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3501e-108">Attributes</span></span>

<span data-ttu-id="3501e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3501e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3501e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3501e-110">Child elements</span></span>

|<span data-ttu-id="3501e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3501e-111">**Element**</span></span>|<span data-ttu-id="3501e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3501e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3501e-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="3501e-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="3501e-114">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3501e-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3501e-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3501e-115">Parent elements</span></span>

|<span data-ttu-id="3501e-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3501e-116">**Element**</span></span>|<span data-ttu-id="3501e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="3501e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3501e-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="3501e-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3501e-119">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="3501e-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3501e-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3501e-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3501e-121">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3501e-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3501e-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="3501e-122">Remarks</span></span>

<span data-ttu-id="3501e-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3501e-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3501e-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3501e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3501e-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3501e-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3501e-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3501e-126">Schema name</span></span>  <br/> |<span data-ttu-id="3501e-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3501e-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="3501e-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3501e-128">Validation file</span></span>  <br/> |<span data-ttu-id="3501e-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3501e-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3501e-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3501e-130">Can be empty</span></span>  <br/> |<span data-ttu-id="3501e-131">False</span><span class="sxs-lookup"><span data-stu-id="3501e-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3501e-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3501e-132">See also</span></span>

- [<span data-ttu-id="3501e-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3501e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

