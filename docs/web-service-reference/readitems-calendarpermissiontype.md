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
description: L’élément ReadItems indique si un utilisateur est autorisé à lire des éléments dans un dossier de calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e040b643016781f9f890050f189191356f8d4f0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468298"
---
# <a name="readitems-calendarpermissiontype"></a><span data-ttu-id="2ecec-104">ReadItems (CalendarPermissionType)</span><span class="sxs-lookup"><span data-stu-id="2ecec-104">ReadItems (CalendarPermissionType)</span></span>

<span data-ttu-id="2ecec-105">L’élément **ReadItems** indique si un utilisateur est autorisé à lire des éléments dans un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="2ecec-105">The **ReadItems** element indicates whether a user has permission to read items within a Calendar folder.</span></span> <span data-ttu-id="2ecec-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2ecec-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 <span data-ttu-id="2ecec-107">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="2ecec-107">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ecec-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2ecec-108">Attributes and elements</span></span>

<span data-ttu-id="2ecec-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2ecec-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ecec-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="2ecec-110">Attributes</span></span>

<span data-ttu-id="2ecec-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2ecec-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ecec-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2ecec-112">Child elements</span></span>

<span data-ttu-id="2ecec-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ecec-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ecec-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2ecec-114">Parent elements</span></span>

|<span data-ttu-id="2ecec-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ecec-115">**Element**</span></span>|<span data-ttu-id="2ecec-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ecec-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ecec-117">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="2ecec-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="2ecec-p103">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="2ecec-p103">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ecec-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="2ecec-120">Text value</span></span>

<span data-ttu-id="2ecec-121">Le tableau suivant répertorie les valeurs possibles pour l’élément **ReadItems** .</span><span class="sxs-lookup"><span data-stu-id="2ecec-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="2ecec-122">**Valeurs de texte de l’élément ReadItems**</span><span class="sxs-lookup"><span data-stu-id="2ecec-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="2ecec-123">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="2ecec-123">**Value**</span></span>|<span data-ttu-id="2ecec-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ecec-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2ecec-125">Aucun</span><span class="sxs-lookup"><span data-stu-id="2ecec-125">None</span></span>  <br/> |<span data-ttu-id="2ecec-126">Indique que l’utilisateur n’est pas autorisé à afficher des éléments dans le calendrier.</span><span class="sxs-lookup"><span data-stu-id="2ecec-126">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="2ecec-127">TimeOnly</span><span class="sxs-lookup"><span data-stu-id="2ecec-127">TimeOnly</span></span>  <br/> |<span data-ttu-id="2ecec-128">Indique que l’utilisateur est autorisé à afficher uniquement les disponibilités dans le calendrier.</span><span class="sxs-lookup"><span data-stu-id="2ecec-128">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="2ecec-129">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="2ecec-129">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="2ecec-130">Indique que l’utilisateur est autorisé à afficher les heures de disponibilité dans le calendrier et l’objet et l’emplacement des rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="2ecec-130">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="2ecec-131">FullDetails</span><span class="sxs-lookup"><span data-stu-id="2ecec-131">FullDetails</span></span>  <br/> |<span data-ttu-id="2ecec-132">Indique que l’utilisateur est autorisé à afficher tous les éléments du calendrier, notamment la disponibilité et l’objet, le lieu et les détails des rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="2ecec-132">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2ecec-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="2ecec-133">Remarks</span></span>

<span data-ttu-id="2ecec-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2ecec-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ecec-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2ecec-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ecec-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2ecec-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ecec-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2ecec-137">Schema Name</span></span>  <br/> |<span data-ttu-id="2ecec-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2ecec-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="2ecec-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2ecec-139">Validation File</span></span>  <br/> |<span data-ttu-id="2ecec-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2ecec-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ecec-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2ecec-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ecec-142">False</span><span class="sxs-lookup"><span data-stu-id="2ecec-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ecec-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2ecec-143">See also</span></span>



- [<span data-ttu-id="2ecec-144">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2ecec-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="2ecec-145">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="2ecec-145">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

