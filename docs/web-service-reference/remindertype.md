---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: L’élément ReminderType Spécifie le type de rappels à renvoyer.
ms.openlocfilehash: 11739d2068a1009b2840b2169e86b113151cbfa9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829077"
---
# <a name="remindertype"></a><span data-ttu-id="1b054-103">ReminderType</span><span class="sxs-lookup"><span data-stu-id="1b054-103">ReminderType</span></span>

<span data-ttu-id="1b054-104">L’élément **ReminderType** Spécifie le type de rappels à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="1b054-104">The **ReminderType** element specifies the type of reminders to return.</span></span> 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 <span data-ttu-id="1b054-105">**string**</span><span class="sxs-lookup"><span data-stu-id="1b054-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b054-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1b054-106">Attributes and elements</span></span>

<span data-ttu-id="1b054-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1b054-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b054-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1b054-108">Attributes</span></span>

<span data-ttu-id="1b054-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1b054-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b054-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1b054-110">Child elements</span></span>

<span data-ttu-id="1b054-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1b054-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1b054-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1b054-112">Parent elements</span></span>

[<span data-ttu-id="1b054-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="1b054-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="1b054-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1b054-114">Text value</span></span>

<span data-ttu-id="1b054-115">La valeur de texte de l’élément **ReminderType** est le type de rappels à renvoyer, **tous les**, **actuel**ou **ancien**.</span><span class="sxs-lookup"><span data-stu-id="1b054-115">The text value of the **ReminderType** element is the type of reminders to return, either **All**, **Current**, or **Old**.</span></span> <span data-ttu-id="1b054-116">**All** est la valeur recommandée pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="1b054-116">**All** is the recommended value for this element.</span></span> <span data-ttu-id="1b054-117">Pour plus d’informations sur la relation entre l’élément **ReminderType** et les éléments [BeginTime](begintime.md) et [EndTime](endtime-remindermessagedatatype.md) , voir [opération GetReminders](getreminders-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1b054-117">For more information about the relationship between the **ReminderType** element and the [BeginTime](begintime.md) and [EndTime](endtime-remindermessagedatatype.md) elements, see [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1b054-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="1b054-118">Remarks</span></span>

<span data-ttu-id="1b054-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1b054-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1b054-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b054-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b054-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1b054-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b054-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1b054-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1b054-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1b054-123">Schema Name</span></span>  <br/> |<span data-ttu-id="1b054-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1b054-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1b054-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1b054-125">Validation File</span></span>  <br/> |<span data-ttu-id="1b054-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1b054-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b054-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1b054-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b054-128">False</span><span class="sxs-lookup"><span data-stu-id="1b054-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b054-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1b054-129">See also</span></span>



[<span data-ttu-id="1b054-130">GetReminders</span><span class="sxs-lookup"><span data-stu-id="1b054-130">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="1b054-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1b054-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

