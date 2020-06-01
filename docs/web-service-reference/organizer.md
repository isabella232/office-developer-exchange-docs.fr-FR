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
description: L’élément organisateur représente l’organisateur d’une réunion.
ms.openlocfilehash: c1188c9b3a894e86a08b8869045c3647e394f506
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462415"
---
# <a name="organizer"></a><span data-ttu-id="41c17-103">Organisateur</span><span class="sxs-lookup"><span data-stu-id="41c17-103">Organizer</span></span>

<span data-ttu-id="41c17-104">L’élément **organisateur** représente l’organisateur d’une réunion.</span><span class="sxs-lookup"><span data-stu-id="41c17-104">The **Organizer** element represents the organizer of a meeting.</span></span> 
  
```xml
<Organizer>
   <Mailbox/>
</Organizer>
```

<span data-ttu-id="41c17-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="41c17-105">**SingleRecipientType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="41c17-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="41c17-106">Attributes and elements</span></span>

<span data-ttu-id="41c17-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="41c17-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41c17-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="41c17-108">Attributes</span></span>

<span data-ttu-id="41c17-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="41c17-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41c17-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="41c17-110">Child elements</span></span>

|<span data-ttu-id="41c17-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="41c17-111">**Element**</span></span>|<span data-ttu-id="41c17-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="41c17-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41c17-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="41c17-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="41c17-114">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="41c17-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="41c17-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="41c17-115">Parent elements</span></span>

|<span data-ttu-id="41c17-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="41c17-116">**Element**</span></span>|<span data-ttu-id="41c17-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="41c17-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41c17-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="41c17-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="41c17-119">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="41c17-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="41c17-120">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="41c17-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="41c17-121">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="41c17-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="41c17-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="41c17-122">Remarks</span></span>

<span data-ttu-id="41c17-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="41c17-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41c17-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="41c17-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41c17-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="41c17-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41c17-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="41c17-126">Schema name</span></span>  <br/> |<span data-ttu-id="41c17-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="41c17-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="41c17-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="41c17-128">Validation file</span></span>  <br/> |<span data-ttu-id="41c17-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="41c17-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="41c17-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="41c17-130">Can be empty</span></span>  <br/> |<span data-ttu-id="41c17-131">False</span><span class="sxs-lookup"><span data-stu-id="41c17-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41c17-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="41c17-132">See also</span></span>

- [<span data-ttu-id="41c17-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="41c17-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

