---
title: ReminderMessageData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04dd4987-baaf-4ebe-ae58-ad962c2f8fa1
description: L’élément ReminderMessageData spécifie les données dans un message de rappel.
ms.openlocfilehash: a1d01dd24030b047bd8ad025f3e1cebed0da8e29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829067"
---
# <a name="remindermessagedata"></a><span data-ttu-id="260fc-103">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="260fc-103">ReminderMessageData</span></span>

<span data-ttu-id="260fc-104">L’élément **ReminderMessageData** spécifie les données dans un message de rappel.</span><span class="sxs-lookup"><span data-stu-id="260fc-104">The **ReminderMessageData** element specifies the data in a reminder message.</span></span> 
  
```XML
<ReminderMessageData>
   <ReminderText></ReminderText>
   <Location></Location>
   <StartTime></StartTime>
   <EndTime></EndTime>
   <AssociatedCalendarItemId></AssociatedCalendarItemId>
</ReminderMessageData>

```

 <span data-ttu-id="260fc-105">**ReminderMessageDataType**</span><span class="sxs-lookup"><span data-stu-id="260fc-105">**ReminderMessageDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="260fc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="260fc-106">Attributes and elements</span></span>

<span data-ttu-id="260fc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="260fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="260fc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="260fc-108">Attributes</span></span>

<span data-ttu-id="260fc-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="260fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="260fc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="260fc-110">Child elements</span></span>

<span data-ttu-id="260fc-111">[ReminderText](remindertext.md) | [emplacement](location.md) | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span><span class="sxs-lookup"><span data-stu-id="260fc-111">[ReminderText](remindertext.md) | [Location](location.md) | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="260fc-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="260fc-112">Parent elements</span></span>

[<span data-ttu-id="260fc-113">Message</span><span class="sxs-lookup"><span data-stu-id="260fc-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="260fc-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="260fc-114">Remarks</span></span>

<span data-ttu-id="260fc-115">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="260fc-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="260fc-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="260fc-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="260fc-117">Versions d’Exchange commençant par le numéro de version 15.00.0913.09 peuvent inclure l’élément **AssociatedCalendarItemId** comme un élément enfant de l’élément **ReminderMessageData** .</span><span class="sxs-lookup"><span data-stu-id="260fc-117">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="260fc-118">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="260fc-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="260fc-119">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="260fc-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="260fc-120">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="260fc-120">Schema Name</span></span>  <br/> |<span data-ttu-id="260fc-121">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="260fc-121">Types schema</span></span>  <br/> |
|<span data-ttu-id="260fc-122">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="260fc-122">Validation File</span></span>  <br/> |<span data-ttu-id="260fc-123">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="260fc-123">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="260fc-124">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="260fc-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="260fc-125">True</span><span class="sxs-lookup"><span data-stu-id="260fc-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="260fc-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="260fc-126">See also</span></span>



[<span data-ttu-id="260fc-127">Message</span><span class="sxs-lookup"><span data-stu-id="260fc-127">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="260fc-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="260fc-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

