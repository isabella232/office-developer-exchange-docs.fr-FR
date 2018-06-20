---
title: SharingEffectiveRights (CalendarPermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: b519f642-a9ef-4300-92e6-ed8202855fde
description: L’élément SharingEffectiveRights indique les autorisations dont dispose l’utilisateur pour les données de calendrier qui sont partagées.
ms.openlocfilehash: e7d2aa061650c33d27de042ae8a6348f9a7d3430
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829480"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a><span data-ttu-id="98ef9-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="98ef9-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>

<span data-ttu-id="98ef9-104">L’élément **SharingEffectiveRights** indique les autorisations dont dispose l’utilisateur pour les données de calendrier qui sont partagées.</span><span class="sxs-lookup"><span data-stu-id="98ef9-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the calendar data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 <span data-ttu-id="98ef9-105">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="98ef9-105">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98ef9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="98ef9-106">Attributes and elements</span></span>

<span data-ttu-id="98ef9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="98ef9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98ef9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="98ef9-108">Attributes</span></span>

<span data-ttu-id="98ef9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="98ef9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98ef9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="98ef9-110">Child elements</span></span>

<span data-ttu-id="98ef9-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="98ef9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98ef9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="98ef9-112">Parent elements</span></span>

|<span data-ttu-id="98ef9-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="98ef9-113">**Element**</span></span>|<span data-ttu-id="98ef9-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="98ef9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98ef9-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="98ef9-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="98ef9-116">Représente un dossier contenant principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="98ef9-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98ef9-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="98ef9-117">Text value</span></span>

<span data-ttu-id="98ef9-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **SharingEffectiveRights** .</span><span class="sxs-lookup"><span data-stu-id="98ef9-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
|<span data-ttu-id="98ef9-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="98ef9-119">**Value**</span></span>|<span data-ttu-id="98ef9-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="98ef9-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="98ef9-121">None</span><span class="sxs-lookup"><span data-stu-id="98ef9-121">None</span></span>  <br/> |<span data-ttu-id="98ef9-122">Indique que l’utilisateur ne dispose pas d’autorisation d’afficher des éléments dans le calendrier.</span><span class="sxs-lookup"><span data-stu-id="98ef9-122">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="98ef9-123">TimeOnly</span><span class="sxs-lookup"><span data-stu-id="98ef9-123">TimeOnly</span></span>  <br/> |<span data-ttu-id="98ef9-124">Indique que l’utilisateur est autorisé à afficher uniquement formulées dans le calendrier.</span><span class="sxs-lookup"><span data-stu-id="98ef9-124">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="98ef9-125">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="98ef9-125">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="98ef9-126">Indique que l’utilisateur est autorisé à afficher le temps de disponibilité dans le calendrier et le sujet et l’emplacement du rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="98ef9-126">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="98ef9-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="98ef9-127">FullDetails</span></span>  <br/> |<span data-ttu-id="98ef9-128">Indique que l’utilisateur est autorisé à afficher tous les éléments dans le calendrier, notamment formulées et subject, emplacement et les détails des rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="98ef9-128">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="98ef9-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="98ef9-129">Remarks</span></span>

<span data-ttu-id="98ef9-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="98ef9-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98ef9-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="98ef9-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98ef9-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="98ef9-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="98ef9-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="98ef9-133">Schema Name</span></span>  <br/> |<span data-ttu-id="98ef9-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="98ef9-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="98ef9-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="98ef9-135">Validation File</span></span>  <br/> |<span data-ttu-id="98ef9-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="98ef9-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="98ef9-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="98ef9-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="98ef9-138">False</span><span class="sxs-lookup"><span data-stu-id="98ef9-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98ef9-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="98ef9-139">See also</span></span>



- [<span data-ttu-id="98ef9-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="98ef9-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

