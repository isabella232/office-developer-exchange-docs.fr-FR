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
ms.openlocfilehash: f2632062cd02581c426f7dbfa2a33d53e5594d72
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458550"
---
# <a name="remindermessagedata"></a><span data-ttu-id="25db2-103">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="25db2-103">ReminderMessageData</span></span>

<span data-ttu-id="25db2-104">L’élément **ReminderMessageData** spécifie les données dans un message de rappel.</span><span class="sxs-lookup"><span data-stu-id="25db2-104">The **ReminderMessageData** element specifies the data in a reminder message.</span></span> 
  
```XML
<ReminderMessageData>
   <ReminderText></ReminderText>
   <Location></Location>
   <StartTime></StartTime>
   <EndTime></EndTime>
   <AssociatedCalendarItemId></AssociatedCalendarItemId>
</ReminderMessageData>

```

 <span data-ttu-id="25db2-105">**ReminderMessageDataType**</span><span class="sxs-lookup"><span data-stu-id="25db2-105">**ReminderMessageDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25db2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="25db2-106">Attributes and elements</span></span>

<span data-ttu-id="25db2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="25db2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25db2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="25db2-108">Attributes</span></span>

<span data-ttu-id="25db2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="25db2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25db2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="25db2-110">Child elements</span></span>

<span data-ttu-id="25db2-111">[ReminderText](remindertext.md)  |  [Emplacement](location.md)  |  [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md)  |  [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md)  |  [AssociatedCalendarItemId](associatedcalendaritemid.md)</span><span class="sxs-lookup"><span data-stu-id="25db2-111">[ReminderText](remindertext.md) | [Location](location.md) | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25db2-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="25db2-112">Parent elements</span></span>

[<span data-ttu-id="25db2-113">Message</span><span class="sxs-lookup"><span data-stu-id="25db2-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="25db2-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="25db2-114">Remarks</span></span>

<span data-ttu-id="25db2-115">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="25db2-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="25db2-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="25db2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="25db2-117">Les versions d’Exchange commençant par le numéro de Build 15.00.0913.09 peuvent inclure l’élément **AssociatedCalendarItemId** en tant qu’élément enfant de l’élément **ReminderMessageData** .</span><span class="sxs-lookup"><span data-stu-id="25db2-117">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="25db2-118">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="25db2-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25db2-119">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="25db2-119">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25db2-120">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="25db2-120">Schema Name</span></span>  <br/> |<span data-ttu-id="25db2-121">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="25db2-121">Types schema</span></span>  <br/> |
|<span data-ttu-id="25db2-122">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="25db2-122">Validation File</span></span>  <br/> |<span data-ttu-id="25db2-123">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="25db2-123">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25db2-124">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="25db2-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="25db2-125">True</span><span class="sxs-lookup"><span data-stu-id="25db2-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25db2-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="25db2-126">See also</span></span>



[<span data-ttu-id="25db2-127">Message</span><span class="sxs-lookup"><span data-stu-id="25db2-127">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="25db2-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="25db2-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

