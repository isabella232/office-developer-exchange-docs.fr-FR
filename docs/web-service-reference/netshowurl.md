---
title: NetShowUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NetShowUrl
api_type:
- schema
ms.assetid: a5d48fc1-b141-422c-bcb0-05d0f9ba90dd
description: L’élément NetShowUrl spécifie l’URL d’une réunion Microsoft NetShow online.
ms.openlocfilehash: 66e288a5e66eecf404698135cc3257085b852034
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466331"
---
# <a name="netshowurl"></a><span data-ttu-id="43305-103">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="43305-103">NetShowUrl</span></span>

<span data-ttu-id="43305-104">L’élément **NetShowUrl** spécifie l’URL d’une réunion Microsoft NetShow online.</span><span class="sxs-lookup"><span data-stu-id="43305-104">The **NetShowUrl** element specifies the URL for a Microsoft NetShow online meeting.</span></span> 
  
```xml
<NetShowUrl/>
```

 <span data-ttu-id="43305-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="43305-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43305-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="43305-106">Attributes and elements</span></span>

<span data-ttu-id="43305-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="43305-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43305-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="43305-108">Attributes</span></span>

<span data-ttu-id="43305-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="43305-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43305-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="43305-110">Child elements</span></span>

<span data-ttu-id="43305-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="43305-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="43305-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="43305-112">Parent elements</span></span>

|<span data-ttu-id="43305-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="43305-113">**Element**</span></span>|<span data-ttu-id="43305-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="43305-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43305-115">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="43305-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="43305-116">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="43305-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="43305-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="43305-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="43305-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="43305-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="43305-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="43305-119">Text value</span></span>

<span data-ttu-id="43305-120">Une valeur de texte qui représente une URL est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="43305-120">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="43305-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="43305-121">Remarks</span></span>

<span data-ttu-id="43305-122">Cette propriété NetShowUrl est accessible en lecture pour l’élément de calendrier de l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="43305-122">This NetShowUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="43305-123">Elle est en lecture seule pour les demandes de réunion et pour les participants.</span><span class="sxs-lookup"><span data-stu-id="43305-123">It is read-only for meeting requests and for attendees.</span></span>
  
<span data-ttu-id="43305-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="43305-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43305-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="43305-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43305-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="43305-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="43305-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="43305-127">Schema name</span></span>  <br/> |<span data-ttu-id="43305-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="43305-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="43305-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="43305-129">Validation file</span></span>  <br/> |<span data-ttu-id="43305-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="43305-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="43305-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="43305-131">Can be empty</span></span>  <br/> |<span data-ttu-id="43305-132">False</span><span class="sxs-lookup"><span data-stu-id="43305-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="43305-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="43305-133">See also</span></span>



- [<span data-ttu-id="43305-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="43305-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

