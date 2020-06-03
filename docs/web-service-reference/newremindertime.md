---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: L’élément NewReminderTime spécifie une nouvelle heure pour un rappel.
ms.openlocfilehash: a10f7e481b474501f33dba4c09060766568952b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465953"
---
# <a name="newremindertime"></a><span data-ttu-id="57794-103">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="57794-103">NewReminderTime</span></span>

<span data-ttu-id="57794-104">L’élément **NewReminderTime** spécifie une nouvelle heure pour un rappel.</span><span class="sxs-lookup"><span data-stu-id="57794-104">The **NewReminderTime** element specifies a new time for a reminder.</span></span> 
  
```XML
<NewReminderTime/>
```

 <span data-ttu-id="57794-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="57794-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57794-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="57794-106">Attributes and elements</span></span>

<span data-ttu-id="57794-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="57794-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57794-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="57794-108">Attributes</span></span>

<span data-ttu-id="57794-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="57794-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57794-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="57794-110">Child elements</span></span>

<span data-ttu-id="57794-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="57794-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57794-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="57794-112">Parent elements</span></span>

[<span data-ttu-id="57794-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="57794-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="57794-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="57794-114">Text value</span></span>

<span data-ttu-id="57794-115">La valeur de texte de l’élément **NewReminderTime** est une nouvelle heure pour le rappel.</span><span class="sxs-lookup"><span data-stu-id="57794-115">The text value of the **NewReminderTime** element is a new time for the reminder.</span></span> <span data-ttu-id="57794-116">L’élément **NewReminderTime** est utilisé lorsque l’élément [ActionType](actiontype-reminderactiontype.md) est défini sur **SNOOZE**, afin de retarder le rappel.</span><span class="sxs-lookup"><span data-stu-id="57794-116">The **NewReminderTime** element is used when the [ActionType](actiontype-reminderactiontype.md) element is set to **Snooze**, in order to delay the reminder.</span></span> <span data-ttu-id="57794-117">La valeur de **NewReminderTime** doit être supérieure à la [ReminderTime](remindertime.md) renvoyée par l' [opération GetReminders](getreminders-operation.md).</span><span class="sxs-lookup"><span data-stu-id="57794-117">The value of the **NewReminderTime** must be greater than the [ReminderTime](remindertime.md) returned by the [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57794-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="57794-118">Remarks</span></span>

<span data-ttu-id="57794-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="57794-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="57794-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="57794-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57794-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="57794-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57794-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="57794-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57794-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="57794-123">Schema Name</span></span>  <br/> |<span data-ttu-id="57794-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="57794-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="57794-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="57794-125">Validation File</span></span>  <br/> |<span data-ttu-id="57794-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="57794-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57794-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="57794-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="57794-128">False</span><span class="sxs-lookup"><span data-stu-id="57794-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57794-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="57794-129">See also</span></span>



[<span data-ttu-id="57794-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="57794-130">ReminderItemAction</span></span>](reminderitemaction.md)


- [<span data-ttu-id="57794-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="57794-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

