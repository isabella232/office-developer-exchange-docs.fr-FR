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
ms.openlocfilehash: 9f3f509942c673c916cc646cd9519240aef6ea06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828531"
---
# <a name="newremindertime"></a><span data-ttu-id="f3866-103">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="f3866-103">NewReminderTime</span></span>

<span data-ttu-id="f3866-104">L’élément **NewReminderTime** spécifie une nouvelle heure pour un rappel.</span><span class="sxs-lookup"><span data-stu-id="f3866-104">The **NewReminderTime** element specifies a new time for a reminder.</span></span> 
  
```XML
<NewReminderTime/>
```

 <span data-ttu-id="f3866-105">**string**</span><span class="sxs-lookup"><span data-stu-id="f3866-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3866-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f3866-106">Attributes and elements</span></span>

<span data-ttu-id="f3866-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f3866-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3866-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f3866-108">Attributes</span></span>

<span data-ttu-id="f3866-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f3866-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3866-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f3866-110">Child elements</span></span>

<span data-ttu-id="f3866-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f3866-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3866-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f3866-112">Parent elements</span></span>

[<span data-ttu-id="f3866-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="f3866-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="f3866-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f3866-114">Text value</span></span>

<span data-ttu-id="f3866-115">La valeur de texte de l’élément **NewReminderTime** est une nouvelle heure pour le rappel.</span><span class="sxs-lookup"><span data-stu-id="f3866-115">The text value of the **NewReminderTime** element is a new time for the reminder.</span></span> <span data-ttu-id="f3866-116">L’élément **NewReminderTime** est utilisé lorsque l’élément [ActionType](actiontype-reminderactiontype.md) est défini sur **Répéter**, afin de différer le rappel.</span><span class="sxs-lookup"><span data-stu-id="f3866-116">The **NewReminderTime** element is used when the [ActionType](actiontype-reminderactiontype.md) element is set to **Snooze**, in order to delay the reminder.</span></span> <span data-ttu-id="f3866-117">La valeur de la **NewReminderTime** doit être supérieure à la [ReminderTime](remindertime.md) retournées par l' [opération GetReminders](getreminders-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f3866-117">The value of the **NewReminderTime** must be greater than the [ReminderTime](remindertime.md) returned by the [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f3866-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="f3866-118">Remarks</span></span>

<span data-ttu-id="f3866-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f3866-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f3866-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3866-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3866-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f3866-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3866-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f3866-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f3866-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f3866-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f3866-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f3866-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="f3866-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f3866-125">Validation File</span></span>  <br/> |<span data-ttu-id="f3866-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f3866-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f3866-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f3866-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3866-128">False</span><span class="sxs-lookup"><span data-stu-id="f3866-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3866-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f3866-129">See also</span></span>



[<span data-ttu-id="f3866-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="f3866-130">ReminderItemAction</span></span>](reminderitemaction.md)


- [<span data-ttu-id="f3866-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f3866-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

