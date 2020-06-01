---
title: AssociatedCalendarItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssociatedCalendarItemId
api_type:
- schema
ms.assetid: 5b29898c-ea59-4e6a-914c-c011ec754032
description: L’élément AssociatedCalendarItemId représente l’élément de calendrier qui est associé à un MeetingMessage, propriété meetingrequest, MeetingResponse, MeetingCancellation ou ReminderMessageData.
ms.openlocfilehash: 816372c38243ba0fe5a7606c264dd1c5107350f2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460882"
---
# <a name="associatedcalendaritemid"></a><span data-ttu-id="2f036-103">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="2f036-103">AssociatedCalendarItemId</span></span>

<span data-ttu-id="2f036-104">L' **élément AssociatedCalendarItemId** représente l’élément de calendrier qui est associé à un [MeetingMessage](meetingmessage.md), [propriété meetingrequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md)ou [ReminderMessageData](remindermessagedata.md).</span><span class="sxs-lookup"><span data-stu-id="2f036-104">The **AssociatedCalendarItemId** element represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md), [MeetingRequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md), or [ReminderMessageData](remindermessagedata.md).</span></span>
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="2f036-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="2f036-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f036-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2f036-106">Attributes and elements</span></span>

<span data-ttu-id="2f036-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2f036-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f036-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2f036-108">Attributes</span></span>

|<span data-ttu-id="2f036-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="2f036-109">**Attribute**</span></span>|<span data-ttu-id="2f036-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="2f036-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2f036-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="2f036-111">**Id**</span></span> <br/> |<span data-ttu-id="2f036-112">Identifie l’élément de calendrier qui est associé à la réunion.</span><span class="sxs-lookup"><span data-stu-id="2f036-112">Identifies the calendar item that is associated with meeting.</span></span>  <br/> |
|<span data-ttu-id="2f036-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="2f036-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="2f036-114">Identifie une version spécifique de l’élément de calendrier associé à une réunion.</span><span class="sxs-lookup"><span data-stu-id="2f036-114">Identifies a specific version of the calendar item that is associated with a meeting.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2f036-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2f036-115">Child elements</span></span>

<span data-ttu-id="2f036-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2f036-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2f036-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2f036-117">Parent elements</span></span>

<span data-ttu-id="2f036-118">[MeetingMessage](meetingmessage.md)  |  [Propriété meetingrequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [ReminderMessageData](remindermessagedata.md)</span><span class="sxs-lookup"><span data-stu-id="2f036-118">[MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [ReminderMessageData](remindermessagedata.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2f036-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="2f036-119">Remarks</span></span>

<span data-ttu-id="2f036-120">Les versions d’Exchange commençant par le numéro de Build 15.00.0913.09 peuvent inclure l’élément **AssociatedCalendarItemId** en tant qu’élément enfant de l’élément **ReminderMessageData** .</span><span class="sxs-lookup"><span data-stu-id="2f036-120">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
<span data-ttu-id="2f036-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f036-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f036-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2f036-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f036-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2f036-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2f036-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2f036-124">Schema Name</span></span>  <br/> |<span data-ttu-id="2f036-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2f036-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="2f036-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2f036-126">Validation File</span></span>  <br/> |<span data-ttu-id="2f036-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2f036-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2f036-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2f036-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="2f036-129">False</span><span class="sxs-lookup"><span data-stu-id="2f036-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f036-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2f036-130">See also</span></span>

- [<span data-ttu-id="2f036-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2f036-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

