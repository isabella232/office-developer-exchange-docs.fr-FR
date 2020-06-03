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
description: L’élément CalendarPermission définit l’accès d’un utilisateur à un dossier de calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: c43f75e6cf5abc2dce9af6c04122ec9a589dcd58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529475"
---
# <a name="calendarpermission"></a><span data-ttu-id="09ad4-104">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="09ad4-104">CalendarPermission</span></span>

<span data-ttu-id="09ad4-105">L’élément **CalendarPermission** définit l’accès d’un utilisateur à un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-105">The **CalendarPermission** element defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="09ad4-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="09ad4-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
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

 <span data-ttu-id="09ad4-107">**CalendarPermissionType**</span><span class="sxs-lookup"><span data-stu-id="09ad4-107">**CalendarPermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09ad4-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="09ad4-108">Attributes and elements</span></span>

<span data-ttu-id="09ad4-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="09ad4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09ad4-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="09ad4-110">Attributes</span></span>

<span data-ttu-id="09ad4-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="09ad4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09ad4-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="09ad4-112">Child elements</span></span>

|<span data-ttu-id="09ad4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="09ad4-113">**Element**</span></span>|<span data-ttu-id="09ad4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="09ad4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09ad4-115">CalendarPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="09ad4-115">CalendarPermissionLevel</span></span>](calendarpermissionlevel.md) <br/> |<span data-ttu-id="09ad4-116">Représente le niveau d’autorisation d’un utilisateur sur un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-116">Represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="09ad4-117">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="09ad4-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="09ad4-118">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="09ad4-118">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="09ad4-119">Indique si un utilisateur est autorisé à créer des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-119">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="09ad4-120">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="09ad4-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="09ad4-121">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="09ad4-121">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="09ad4-122">Indique si un utilisateur est autorisé à créer des sous-dossiers dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-122">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="09ad4-123">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="09ad4-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="09ad4-124">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="09ad4-124">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="09ad4-125">Indique si un utilisateur est autorisé à supprimer des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-125">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="09ad4-126">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="09ad4-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="09ad4-127">EditItems</span><span class="sxs-lookup"><span data-stu-id="09ad4-127">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="09ad4-128">Indique si un utilisateur est autorisé à modifier les éléments d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-128">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="09ad4-129">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="09ad4-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="09ad4-130">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="09ad4-130">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="09ad4-131">Indique si un utilisateur est un contact pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-131">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="09ad4-132">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="09ad4-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="09ad4-133">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="09ad4-133">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="09ad4-134">Indique si un utilisateur est le propriétaire d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-134">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="09ad4-135">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="09ad4-135">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="09ad4-136">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="09ad4-136">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="09ad4-137">Indique si un utilisateur peut afficher un dossier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-137">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="09ad4-138">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="09ad4-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="09ad4-139">ReadItems (CalendarPermissionType)</span><span class="sxs-lookup"><span data-stu-id="09ad4-139">ReadItems (CalendarPermissionType)</span></span>](readitems-calendarpermissiontype.md) <br/> |<span data-ttu-id="09ad4-140">Indique si un utilisateur est autorisé à lire des éléments dans un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-140">Indicates whether a user has permission to read items within a calendar folder.</span></span> <span data-ttu-id="09ad4-141">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="09ad4-141">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="09ad4-142">UserId</span><span class="sxs-lookup"><span data-stu-id="09ad4-142">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="09ad4-143">Identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-143">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="09ad4-144">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="09ad4-144">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="09ad4-145">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="09ad4-145">Parent elements</span></span>

|<span data-ttu-id="09ad4-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="09ad4-146">**Element**</span></span>|<span data-ttu-id="09ad4-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="09ad4-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09ad4-148">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="09ad4-148">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="09ad4-149">Contient un tableau des autorisations de calendrier pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="09ad4-149">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="09ad4-150">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="09ad4-150">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="09ad4-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="09ad4-151">Remarks</span></span>

<span data-ttu-id="09ad4-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="09ad4-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09ad4-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="09ad4-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09ad4-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="09ad4-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="09ad4-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="09ad4-155">Schema Name</span></span>  <br/> |<span data-ttu-id="09ad4-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="09ad4-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="09ad4-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="09ad4-157">Validation File</span></span>  <br/> |<span data-ttu-id="09ad4-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="09ad4-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="09ad4-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="09ad4-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="09ad4-160">False</span><span class="sxs-lookup"><span data-stu-id="09ad4-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09ad4-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="09ad4-161">See also</span></span>



- [<span data-ttu-id="09ad4-162">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="09ad4-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="09ad4-163">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="09ad4-163">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

