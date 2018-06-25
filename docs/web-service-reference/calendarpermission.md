---
title: CalendarPermission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermission
api_type:
- schema
ms.assetid: 3aafb221-a04b-41f6-804e-eda810f1ba28
description: L’élément CalendarPermission définit l’accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 7f6ceb6895add3fdd82cdd595463b3a80db822e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755475"
---
# <a name="calendarpermission"></a><span data-ttu-id="d50bb-104">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="d50bb-104">CalendarPermission</span></span>

<span data-ttu-id="d50bb-105">L’élément **CalendarPermission** définit l’accès dont dispose un utilisateur dans un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-105">The **CalendarPermission** element defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="d50bb-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d50bb-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Permission>
   <CalendarPermissionLevel/>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 <span data-ttu-id="d50bb-107">**CalendarPermissionType**</span><span class="sxs-lookup"><span data-stu-id="d50bb-107">**CalendarPermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d50bb-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d50bb-108">Attributes and elements</span></span>

<span data-ttu-id="d50bb-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d50bb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d50bb-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d50bb-110">Attributes</span></span>

<span data-ttu-id="d50bb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d50bb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d50bb-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d50bb-112">Child elements</span></span>

|<span data-ttu-id="d50bb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d50bb-113">**Element**</span></span>|<span data-ttu-id="d50bb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d50bb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d50bb-115">CalendarPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="d50bb-115">CalendarPermissionLevel</span></span>](calendarpermissionlevel.md) <br/> |<span data-ttu-id="d50bb-116">Représente le niveau d’autorisation dont dispose un utilisateur sur un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-116">Represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="d50bb-117">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d50bb-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d50bb-118">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="d50bb-118">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="d50bb-119">Indique si un utilisateur est autorisé à créer des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-119">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="d50bb-120">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d50bb-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d50bb-121">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="d50bb-121">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="d50bb-122">Indique si un utilisateur est autorisé à créer des sous-dossiers dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-122">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="d50bb-123">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d50bb-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d50bb-124">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="d50bb-124">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="d50bb-125">Indique si un utilisateur est autorisé à supprimer des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-125">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="d50bb-126">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d50bb-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d50bb-127">Modifier les éléments</span><span class="sxs-lookup"><span data-stu-id="d50bb-127">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="d50bb-128">Indique si un utilisateur est autorisé à modifier des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-128">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="d50bb-129">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d50bb-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d50bb-130">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="d50bb-130">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="d50bb-131">Indique si un utilisateur est un contact d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-131">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="d50bb-132">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d50bb-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d50bb-133">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="d50bb-133">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="d50bb-134">Indique si un utilisateur est le propriétaire d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-134">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="d50bb-135">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d50bb-135">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d50bb-136">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="d50bb-136">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="d50bb-137">Indique si un utilisateur peut afficher un dossier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-137">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="d50bb-138">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d50bb-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d50bb-139">ReadItems (CalendarPermissionType)</span><span class="sxs-lookup"><span data-stu-id="d50bb-139">ReadItems (CalendarPermissionType)</span></span>](readitems-calendarpermissiontype.md) <br/> |<span data-ttu-id="d50bb-140">Indique si un utilisateur est autorisé à lire les éléments dans un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-140">Indicates whether a user has permission to read items within a calendar folder.</span></span> <span data-ttu-id="d50bb-141">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d50bb-141">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d50bb-142">Nom d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="d50bb-142">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="d50bb-143">Identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-143">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="d50bb-144">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d50bb-144">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d50bb-145">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d50bb-145">Parent elements</span></span>

|<span data-ttu-id="d50bb-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d50bb-146">**Element**</span></span>|<span data-ttu-id="d50bb-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="d50bb-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d50bb-148">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="d50bb-148">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="d50bb-149">Contient un tableau d’autorisations pour un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="d50bb-149">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="d50bb-150">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d50bb-150">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d50bb-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="d50bb-151">Remarks</span></span>

<span data-ttu-id="d50bb-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d50bb-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d50bb-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d50bb-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d50bb-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d50bb-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d50bb-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d50bb-155">Schema Name</span></span>  <br/> |<span data-ttu-id="d50bb-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d50bb-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="d50bb-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d50bb-157">Validation File</span></span>  <br/> |<span data-ttu-id="d50bb-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d50bb-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d50bb-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d50bb-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="d50bb-160">False</span><span class="sxs-lookup"><span data-stu-id="d50bb-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d50bb-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d50bb-161">See also</span></span>



- [<span data-ttu-id="d50bb-162">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d50bb-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d50bb-163">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="d50bb-163">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

