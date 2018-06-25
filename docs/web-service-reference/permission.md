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
description: L’élément d’autorisation définit l’accès dont dispose un utilisateur dans un dossier.
ms.openlocfilehash: 600d60f481c4f1d407c3a39ab65d6ddcf46d04e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828735"
---
# <a name="permission"></a><span data-ttu-id="345f3-103">Autorisation</span><span class="sxs-lookup"><span data-stu-id="345f3-103">Permission</span></span>

<span data-ttu-id="345f3-104">L’élément **d’autorisation** définit l’accès dont dispose un utilisateur dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-104">The **Permission** element defines the access that a user has to a folder.</span></span> 
  
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

 <span data-ttu-id="345f3-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="345f3-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="345f3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="345f3-106">Attributes and elements</span></span>

<span data-ttu-id="345f3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="345f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="345f3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="345f3-108">Attributes</span></span>

<span data-ttu-id="345f3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="345f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="345f3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="345f3-110">Child elements</span></span>

|<span data-ttu-id="345f3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="345f3-111">**Element**</span></span>|<span data-ttu-id="345f3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="345f3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="345f3-113">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="345f3-113">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="345f3-114">Indique si un utilisateur est autorisé à créer des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-114">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="345f3-115">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="345f3-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="345f3-116">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="345f3-116">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="345f3-117">Indique si un utilisateur est autorisé à créer des sous-dossiers dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-117">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="345f3-118">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="345f3-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="345f3-119">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="345f3-119">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="345f3-120">Indique si un utilisateur est autorisé à supprimer des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-120">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="345f3-121">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="345f3-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="345f3-122">Modifier les éléments</span><span class="sxs-lookup"><span data-stu-id="345f3-122">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="345f3-123">Indique si un utilisateur est autorisé à modifier des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-123">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="345f3-124">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="345f3-124">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="345f3-125">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="345f3-125">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="345f3-126">Indique si un utilisateur est un contact d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-126">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="345f3-127">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="345f3-127">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="345f3-128">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="345f3-128">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="345f3-129">Indique si un utilisateur est le propriétaire d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-129">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="345f3-130">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="345f3-130">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="345f3-131">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="345f3-131">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="345f3-132">Indique si un utilisateur peut afficher un dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-132">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="345f3-133">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="345f3-133">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="345f3-134">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="345f3-134">PermissionLevel</span></span>](permissionlevel.md) <br/> |<span data-ttu-id="345f3-135">Représente la combinaison des autorisations dont dispose un utilisateur sur un dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-135">Represents the combination of permissions that a user has on a folder.</span></span> <span data-ttu-id="345f3-136">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="345f3-136">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="345f3-137">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="345f3-137">ReadItems (PermissionType)</span></span>](readitems-permissiontype.md) <br/> |<span data-ttu-id="345f3-138">Indique si un utilisateur est autorisé à lire les éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-138">Indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="345f3-139">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="345f3-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="345f3-140">Nom d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="345f3-140">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="345f3-141">Identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-141">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="345f3-142">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="345f3-142">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="345f3-143">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="345f3-143">Parent elements</span></span>

|<span data-ttu-id="345f3-144">**Élément**</span><span class="sxs-lookup"><span data-stu-id="345f3-144">**Element**</span></span>|<span data-ttu-id="345f3-145">**Description**</span><span class="sxs-lookup"><span data-stu-id="345f3-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="345f3-146">Autorisations</span><span class="sxs-lookup"><span data-stu-id="345f3-146">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="345f3-147">Contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="345f3-147">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="345f3-148">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="345f3-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="345f3-149">Remarques</span><span class="sxs-lookup"><span data-stu-id="345f3-149">Remarks</span></span>

<span data-ttu-id="345f3-150">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="345f3-150">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="345f3-151">Cet élément a été introduit dans Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="345f3-151">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="345f3-152">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="345f3-152">Version differences</span></span>

<span data-ttu-id="345f3-153">Pour les applications qui ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange commençant par Exchange 2013, les autorisations de dossier ne sont pas renvoyées lorsque l’élément [BaseShape](baseshape.md) a une valeur de **AllProperties** dans la requête d’opération [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="345f3-153">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="345f3-154">Pour récupérer les autorisations du dossier, ajoutez l’élément [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) à l’élément de [AdditionalProperties](additionalproperties.md) dans la demande **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="345f3-154">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="345f3-155">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="345f3-155">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="345f3-156">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="345f3-156">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="345f3-157">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="345f3-157">Schema Name</span></span>  <br/> |<span data-ttu-id="345f3-158">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="345f3-158">Types schema</span></span>  <br/> |
|<span data-ttu-id="345f3-159">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="345f3-159">Validation File</span></span>  <br/> |<span data-ttu-id="345f3-160">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="345f3-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="345f3-161">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="345f3-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="345f3-162">False</span><span class="sxs-lookup"><span data-stu-id="345f3-162">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="345f3-163">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="345f3-163">See also</span></span>



- [<span data-ttu-id="345f3-164">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="345f3-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="345f3-165">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="345f3-165">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

