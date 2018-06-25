---
title: ReadItems (CalendarPermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: bec01982-26a1-4373-b1e6-2e0c838d83c4
description: L’élément ReadItems indique si un utilisateur est autorisé à lire les éléments dans un dossier de calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 532b90c47cca7117a89d59e7012436268be9ebb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828964"
---
# <a name="readitems-calendarpermissiontype"></a><span data-ttu-id="5d1c9-104">ReadItems (CalendarPermissionType)</span><span class="sxs-lookup"><span data-stu-id="5d1c9-104">ReadItems (CalendarPermissionType)</span></span>

<span data-ttu-id="5d1c9-105">L’élément **ReadItems** indique si un utilisateur est autorisé à lire les éléments dans un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="5d1c9-105">The **ReadItems** element indicates whether a user has permission to read items within a Calendar folder.</span></span> <span data-ttu-id="5d1c9-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5d1c9-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 <span data-ttu-id="5d1c9-107">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="5d1c9-107">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d1c9-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5d1c9-108">Attributes and elements</span></span>

<span data-ttu-id="5d1c9-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5d1c9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d1c9-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="5d1c9-110">Attributes</span></span>

<span data-ttu-id="5d1c9-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5d1c9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d1c9-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5d1c9-112">Child elements</span></span>

<span data-ttu-id="5d1c9-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5d1c9-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5d1c9-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5d1c9-114">Parent elements</span></span>

|<span data-ttu-id="5d1c9-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5d1c9-115">**Element**</span></span>|<span data-ttu-id="5d1c9-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="5d1c9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d1c9-117">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="5d1c9-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="5d1c9-p103">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="5d1c9-p103">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5d1c9-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5d1c9-120">Text value</span></span>

<span data-ttu-id="5d1c9-121">Le tableau suivant répertorie les valeurs possibles pour l’élément **ReadItems** .</span><span class="sxs-lookup"><span data-stu-id="5d1c9-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="5d1c9-122">**Valeurs de texte des éléments ReadItems**</span><span class="sxs-lookup"><span data-stu-id="5d1c9-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="5d1c9-123">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="5d1c9-123">**Value**</span></span>|<span data-ttu-id="5d1c9-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="5d1c9-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5d1c9-125">None</span><span class="sxs-lookup"><span data-stu-id="5d1c9-125">None</span></span>  <br/> |<span data-ttu-id="5d1c9-126">Indique que l’utilisateur ne dispose pas d’autorisation d’afficher des éléments dans le calendrier.</span><span class="sxs-lookup"><span data-stu-id="5d1c9-126">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="5d1c9-127">TimeOnly</span><span class="sxs-lookup"><span data-stu-id="5d1c9-127">TimeOnly</span></span>  <br/> |<span data-ttu-id="5d1c9-128">Indique que l’utilisateur est autorisé à afficher uniquement formulées dans le calendrier.</span><span class="sxs-lookup"><span data-stu-id="5d1c9-128">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="5d1c9-129">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="5d1c9-129">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="5d1c9-130">Indique que l’utilisateur est autorisé à afficher le temps de disponibilité dans le calendrier et le sujet et l’emplacement du rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="5d1c9-130">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="5d1c9-131">FullDetails</span><span class="sxs-lookup"><span data-stu-id="5d1c9-131">FullDetails</span></span>  <br/> |<span data-ttu-id="5d1c9-132">Indique que l’utilisateur est autorisé à afficher tous les éléments dans le calendrier, notamment formulées et subject, emplacement et les détails des rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="5d1c9-132">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5d1c9-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="5d1c9-133">Remarks</span></span>

<span data-ttu-id="5d1c9-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5d1c9-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d1c9-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5d1c9-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d1c9-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5d1c9-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5d1c9-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5d1c9-137">Schema Name</span></span>  <br/> |<span data-ttu-id="5d1c9-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5d1c9-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="5d1c9-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5d1c9-139">Validation File</span></span>  <br/> |<span data-ttu-id="5d1c9-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5d1c9-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5d1c9-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5d1c9-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d1c9-142">False</span><span class="sxs-lookup"><span data-stu-id="5d1c9-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d1c9-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5d1c9-143">See also</span></span>



- [<span data-ttu-id="5d1c9-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5d1c9-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5d1c9-145">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="5d1c9-145">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

