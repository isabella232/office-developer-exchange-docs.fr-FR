---
title: Rappel
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54dd748a-23a5-4ea2-88f2-b74c68a3c48f
description: L’élément de rappel spécifie un rappel pour une tâche ou un élément de calendrier.
ms.openlocfilehash: cfa1160bd25f5045a3da5a98f081c9dcb3debe7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829056"
---
# <a name="reminder"></a><span data-ttu-id="a29b1-103">Rappel</span><span class="sxs-lookup"><span data-stu-id="a29b1-103">Reminder</span></span>

<span data-ttu-id="a29b1-104">L’élément de **rappel** spécifie un rappel pour une tâche ou un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="a29b1-104">The **Reminder** element specifies a reminder for a task or a calendar item.</span></span> 
  
```XML
<Reminder>
   <Subject></Subject>
   <Location></Location>
   <ReminderTime></ReminderTime>
   <StartDate></StartDate>
   <EndDate></EndDate>
   <ItemId></ItemId>
   <RecurringMasterItemId></RecurringMasterItemId>
   <ReminderGroup></ReminderGroup>
   <UID></UID>
</Reminder>

```

 <span data-ttu-id="a29b1-105">**ReminderType**</span><span class="sxs-lookup"><span data-stu-id="a29b1-105">**ReminderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a29b1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a29b1-106">Attributes and elements</span></span>

<span data-ttu-id="a29b1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a29b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a29b1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a29b1-108">Attributes</span></span>

<span data-ttu-id="a29b1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a29b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a29b1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a29b1-110">Child elements</span></span>

<span data-ttu-id="a29b1-111">[Objet](subject.md) | [emplacement](location.md) | [ReminderTime](remindertime.md) | [StartDate](startdate.md) | [EndDate (ReminderType)](enddate-remindertype.md) | [ItemId](itemid.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md)  |  [ReminderGroup](remindergroup.md) | [UID](uid.md)</span><span class="sxs-lookup"><span data-stu-id="a29b1-111">[Subject](subject.md) | [Location](location.md) | [ReminderTime](remindertime.md) | [StartDate](startdate.md) | [EndDate (ReminderType)](enddate-remindertype.md) | [ItemId](itemid.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md) | [ReminderGroup](remindergroup.md) | [UID](uid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a29b1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a29b1-112">Parent elements</span></span>

[<span data-ttu-id="a29b1-113">Rappels</span><span class="sxs-lookup"><span data-stu-id="a29b1-113">Reminders</span></span>](reminders.md)
  
## <a name="remarks"></a><span data-ttu-id="a29b1-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="a29b1-114">Remarks</span></span>

<span data-ttu-id="a29b1-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a29b1-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a29b1-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a29b1-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a29b1-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a29b1-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a29b1-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a29b1-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a29b1-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a29b1-119">Schema Name</span></span>  <br/> |<span data-ttu-id="a29b1-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a29b1-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="a29b1-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a29b1-121">Validation File</span></span>  <br/> |<span data-ttu-id="a29b1-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a29b1-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a29b1-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a29b1-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="a29b1-124">False</span><span class="sxs-lookup"><span data-stu-id="a29b1-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a29b1-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a29b1-125">See also</span></span>



[<span data-ttu-id="a29b1-126">Rappels</span><span class="sxs-lookup"><span data-stu-id="a29b1-126">Reminders</span></span>](reminders.md)


- [<span data-ttu-id="a29b1-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a29b1-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

