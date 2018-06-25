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
description: L’élément PermissionSet contient toutes les autorisations qui sont configurées pour un dossier de calendrier.
ms.openlocfilehash: b2e642fd2ee8ded4d0d4c67509a5587f7b1efa8a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828728"
---
# <a name="permissionset-calendarpermissionsettype"></a><span data-ttu-id="4c348-103">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="4c348-103">PermissionSet (CalendarPermissionSetType)</span></span>

<span data-ttu-id="4c348-104">L’élément **PermissionSet** contient toutes les autorisations qui sont configurées pour un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="4c348-104">The **PermissionSet** element contains all the permissions that are configured for a calendar folder.</span></span> 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="4c348-105">**CalendarPermissonSetType**</span><span class="sxs-lookup"><span data-stu-id="4c348-105">**CalendarPermissonSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4c348-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4c348-106">Attributes and elements</span></span>

<span data-ttu-id="4c348-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4c348-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c348-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4c348-108">Attributes</span></span>

<span data-ttu-id="4c348-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4c348-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c348-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4c348-110">Child elements</span></span>

|<span data-ttu-id="4c348-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4c348-111">**Element**</span></span>|<span data-ttu-id="4c348-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4c348-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c348-113">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="4c348-113">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="4c348-114">Contient un tableau d’autorisations pour un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="4c348-114">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="4c348-115">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4c348-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4c348-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="4c348-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="4c348-117">Contient un tableau d’entrées inconnus qui ne peut pas être résolu sur le service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4c348-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="4c348-118">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4c348-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4c348-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4c348-119">Parent elements</span></span>

|<span data-ttu-id="4c348-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4c348-120">**Element**</span></span>|<span data-ttu-id="4c348-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="4c348-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c348-122">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="4c348-122">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="4c348-123">Représente un dossier contenant principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="4c348-123">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4c348-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="4c348-124">Remarks</span></span>

<span data-ttu-id="4c348-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c348-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="4c348-126">Cet élément a été introduit dans Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4c348-126">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="4c348-127">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="4c348-127">Version differences</span></span>

<span data-ttu-id="4c348-128">Pour les applications qui ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange commençant par Exchange 2013, les autorisations de dossier ne sont pas renvoyées lorsque l’élément [BaseShape](baseshape.md) a une valeur de **AllProperties** dans la requête d’opération [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4c348-128">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="4c348-129">Pour récupérer les autorisations du dossier, ajoutez l’élément [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) à l’élément de [AdditionalProperties](additionalproperties.md) dans la demande **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="4c348-129">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="4c348-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4c348-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c348-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4c348-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4c348-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4c348-132">Schema Name</span></span>  <br/> |<span data-ttu-id="4c348-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4c348-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="4c348-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4c348-134">Validation File</span></span>  <br/> |<span data-ttu-id="4c348-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4c348-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4c348-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4c348-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="4c348-137">False</span><span class="sxs-lookup"><span data-stu-id="4c348-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4c348-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4c348-138">See also</span></span>



- [<span data-ttu-id="4c348-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4c348-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="4c348-140">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="4c348-140">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

