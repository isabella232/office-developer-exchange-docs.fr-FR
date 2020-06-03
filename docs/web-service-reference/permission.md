---
title: Autorisation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permission
api_type:
- schema
ms.assetid: b8d0429a-0e58-4480-9847-4901970c7033
description: L’élément permission définit l’accès d’un utilisateur à un dossier.
ms.openlocfilehash: 0f7515dbb06f8423f8d4d95e1391496e8ac73653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459257"
---
# <a name="permission"></a><span data-ttu-id="f9783-103">Autorisation</span><span class="sxs-lookup"><span data-stu-id="f9783-103">Permission</span></span>

<span data-ttu-id="f9783-104">L’élément **permission** définit l’accès d’un utilisateur à un dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-104">The **Permission** element defines the access that a user has to a folder.</span></span> 
  
```XML
<Permission>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <PermissionLevel/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 <span data-ttu-id="f9783-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="f9783-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9783-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f9783-106">Attributes and elements</span></span>

<span data-ttu-id="f9783-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f9783-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9783-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f9783-108">Attributes</span></span>

<span data-ttu-id="f9783-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f9783-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9783-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f9783-110">Child elements</span></span>

|<span data-ttu-id="f9783-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f9783-111">**Element**</span></span>|<span data-ttu-id="f9783-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f9783-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9783-113">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="f9783-113">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="f9783-114">Indique si un utilisateur est autorisé à créer des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-114">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="f9783-115">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f9783-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f9783-116">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="f9783-116">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="f9783-117">Indique si un utilisateur est autorisé à créer des sous-dossiers dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-117">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="f9783-118">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f9783-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f9783-119">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="f9783-119">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="f9783-120">Indique si un utilisateur est autorisé à supprimer des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-120">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="f9783-121">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f9783-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f9783-122">EditItems</span><span class="sxs-lookup"><span data-stu-id="f9783-122">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="f9783-123">Indique si un utilisateur est autorisé à modifier les éléments d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-123">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="f9783-124">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f9783-124">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f9783-125">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="f9783-125">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="f9783-126">Indique si un utilisateur est un contact pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-126">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="f9783-127">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f9783-127">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f9783-128">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="f9783-128">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="f9783-129">Indique si un utilisateur est le propriétaire d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-129">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="f9783-130">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f9783-130">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f9783-131">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="f9783-131">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="f9783-132">Indique si un utilisateur peut afficher un dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-132">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="f9783-133">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f9783-133">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f9783-134">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="f9783-134">PermissionLevel</span></span>](permissionlevel.md) <br/> |<span data-ttu-id="f9783-135">Représente la combinaison d’autorisations dont dispose un utilisateur sur un dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-135">Represents the combination of permissions that a user has on a folder.</span></span> <span data-ttu-id="f9783-136">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f9783-136">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f9783-137">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="f9783-137">ReadItems (PermissionType)</span></span>](readitems-permissiontype.md) <br/> |<span data-ttu-id="f9783-138">Indique si un utilisateur est autorisé à lire des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-138">Indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="f9783-139">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f9783-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f9783-140">UserId</span><span class="sxs-lookup"><span data-stu-id="f9783-140">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="f9783-141">Identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-141">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="f9783-142">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f9783-142">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f9783-143">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f9783-143">Parent elements</span></span>

|<span data-ttu-id="f9783-144">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f9783-144">**Element**</span></span>|<span data-ttu-id="f9783-145">**Description**</span><span class="sxs-lookup"><span data-stu-id="f9783-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9783-146">Autorisations</span><span class="sxs-lookup"><span data-stu-id="f9783-146">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="f9783-147">Contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="f9783-147">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="f9783-148">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f9783-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9783-149">Remarques</span><span class="sxs-lookup"><span data-stu-id="f9783-149">Remarks</span></span>

<span data-ttu-id="f9783-150">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9783-150">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="f9783-151">Cet élément a été introduit dans Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f9783-151">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="f9783-152">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="f9783-152">Version differences</span></span>

<span data-ttu-id="f9783-153">Pour les applications qui ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange à partir d’Exchange 2013, les autorisations de dossiers ne sont pas renvoyées lorsque l’élément [BaseShape](baseshape.md) a une valeur de **AllProperties** dans la demande d’opération [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f9783-153">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="f9783-154">Pour récupérer les autorisations de dossier, ajoutez l’élément [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) à l’élément [AdditionalProperties](additionalproperties.md) dans la demande **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="f9783-154">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f9783-155">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f9783-155">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9783-156">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f9783-156">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9783-157">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f9783-157">Schema Name</span></span>  <br/> |<span data-ttu-id="f9783-158">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f9783-158">Types schema</span></span>  <br/> |
|<span data-ttu-id="f9783-159">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f9783-159">Validation File</span></span>  <br/> |<span data-ttu-id="f9783-160">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f9783-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9783-161">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f9783-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="f9783-162">False</span><span class="sxs-lookup"><span data-stu-id="f9783-162">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9783-163">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f9783-163">See also</span></span>



- [<span data-ttu-id="f9783-164">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f9783-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f9783-165">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="f9783-165">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

