---
title: Reminder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54dd748a-23a5-4ea2-88f2-b74c68a3c48f
description: L’élément Reminder spécifie un rappel pour une tâche ou un élément de calendrier.
ms.openlocfilehash: 71e54d920a169b8060d22bb7d7d294208c344c2e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457486"
---
# <a name="reminder"></a><span data-ttu-id="78d44-103">Reminder</span><span class="sxs-lookup"><span data-stu-id="78d44-103">Reminder</span></span>

<span data-ttu-id="78d44-104">L’élément **Reminder** spécifie un rappel pour une tâche ou un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="78d44-104">The **Reminder** element specifies a reminder for a task or a calendar item.</span></span> 
  
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

 <span data-ttu-id="78d44-105">**ReminderType**</span><span class="sxs-lookup"><span data-stu-id="78d44-105">**ReminderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78d44-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="78d44-106">Attributes and elements</span></span>

<span data-ttu-id="78d44-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="78d44-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78d44-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="78d44-108">Attributes</span></span>

<span data-ttu-id="78d44-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="78d44-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78d44-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="78d44-110">Child elements</span></span>

<span data-ttu-id="78d44-111">[Objet](subject.md)  |  [Emplacement](location.md)  |  [ReminderTime](remindertime.md)  |  [StartDate](startdate.md)  |  [EndDate (ReminderType)](enddate-remindertype.md)  |  [ItemId](itemid.md)  |  [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md)  |  [ReminderGroup](remindergroup.md)  |  [UID](uid.md)</span><span class="sxs-lookup"><span data-stu-id="78d44-111">[Subject](subject.md) | [Location](location.md) | [ReminderTime](remindertime.md) | [StartDate](startdate.md) | [EndDate (ReminderType)](enddate-remindertype.md) | [ItemId](itemid.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md) | [ReminderGroup](remindergroup.md) | [UID](uid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="78d44-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="78d44-112">Parent elements</span></span>

[<span data-ttu-id="78d44-113">Reminders</span><span class="sxs-lookup"><span data-stu-id="78d44-113">Reminders</span></span>](reminders.md)
  
## <a name="remarks"></a><span data-ttu-id="78d44-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="78d44-114">Remarks</span></span>

<span data-ttu-id="78d44-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="78d44-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="78d44-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="78d44-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78d44-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="78d44-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78d44-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="78d44-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78d44-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="78d44-119">Schema Name</span></span>  <br/> |<span data-ttu-id="78d44-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="78d44-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="78d44-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="78d44-121">Validation File</span></span>  <br/> |<span data-ttu-id="78d44-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="78d44-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="78d44-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="78d44-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="78d44-124">False</span><span class="sxs-lookup"><span data-stu-id="78d44-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78d44-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="78d44-125">See also</span></span>



[<span data-ttu-id="78d44-126">Reminders</span><span class="sxs-lookup"><span data-stu-id="78d44-126">Reminders</span></span>](reminders.md)


- [<span data-ttu-id="78d44-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="78d44-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

