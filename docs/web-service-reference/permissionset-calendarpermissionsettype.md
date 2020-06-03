---
title: PermissionSet (CalendarPermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 75f20033-85eb-4627-b4f8-be85e4889e96
description: L’élément PermissionSet contient toutes les autorisations configurées pour un dossier de calendrier.
ms.openlocfilehash: 9564608397ac8a5ab0ddd4508eacd8cad665d76e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458032"
---
# <a name="permissionset-calendarpermissionsettype"></a><span data-ttu-id="d4ac9-103">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="d4ac9-103">PermissionSet (CalendarPermissionSetType)</span></span>

<span data-ttu-id="d4ac9-104">L’élément **PermissionSet** contient toutes les autorisations configurées pour un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="d4ac9-104">The **PermissionSet** element contains all the permissions that are configured for a calendar folder.</span></span> 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="d4ac9-105">**CalendarPermissonSetType**</span><span class="sxs-lookup"><span data-stu-id="d4ac9-105">**CalendarPermissonSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4ac9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4ac9-106">Attributes and elements</span></span>

<span data-ttu-id="d4ac9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4ac9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4ac9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4ac9-108">Attributes</span></span>

<span data-ttu-id="d4ac9-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d4ac9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4ac9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4ac9-110">Child elements</span></span>

|<span data-ttu-id="d4ac9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4ac9-111">**Element**</span></span>|<span data-ttu-id="d4ac9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4ac9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4ac9-113">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="d4ac9-113">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="d4ac9-114">Contient un tableau des autorisations de calendrier pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="d4ac9-114">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="d4ac9-115">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d4ac9-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d4ac9-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="d4ac9-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="d4ac9-117">Contient un tableau d’entrées inconnues qui ne peuvent pas être résolues par rapport au service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d4ac9-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="d4ac9-118">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d4ac9-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4ac9-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4ac9-119">Parent elements</span></span>

|<span data-ttu-id="d4ac9-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4ac9-120">**Element**</span></span>|<span data-ttu-id="d4ac9-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4ac9-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4ac9-122">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="d4ac9-122">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="d4ac9-123">Représente un dossier qui contient principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="d4ac9-123">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d4ac9-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="d4ac9-124">Remarks</span></span>

<span data-ttu-id="d4ac9-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4ac9-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="d4ac9-126">Cet élément a été introduit dans Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d4ac9-126">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="d4ac9-127">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="d4ac9-127">Version differences</span></span>

<span data-ttu-id="d4ac9-128">Pour les applications qui ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange à partir d’Exchange 2013, les autorisations de dossiers ne sont pas renvoyées lorsque l’élément [BaseShape](baseshape.md) a une valeur de **AllProperties** dans la demande d’opération [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d4ac9-128">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="d4ac9-129">Pour récupérer les autorisations de dossier, ajoutez l’élément [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) à l’élément [AdditionalProperties](additionalproperties.md) dans la demande **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="d4ac9-129">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d4ac9-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4ac9-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4ac9-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4ac9-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4ac9-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4ac9-132">Schema Name</span></span>  <br/> |<span data-ttu-id="d4ac9-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d4ac9-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4ac9-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4ac9-134">Validation File</span></span>  <br/> |<span data-ttu-id="d4ac9-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4ac9-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4ac9-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4ac9-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4ac9-137">False</span><span class="sxs-lookup"><span data-stu-id="d4ac9-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4ac9-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4ac9-138">See also</span></span>



- [<span data-ttu-id="d4ac9-139">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d4ac9-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d4ac9-140">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="d4ac9-140">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

