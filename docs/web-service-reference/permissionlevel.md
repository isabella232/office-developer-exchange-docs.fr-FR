---
title: PermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionLevel
api_type:
- schema
ms.assetid: 87978600-3523-451e-a725-ef092c543e2a
description: L’élément PermissionLevel représente le niveau d’autorisation dont dispose un utilisateur sur un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e1e441c53b5c40c16051eb852a6b35a8af7476e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458039"
---
# <a name="permissionlevel"></a><span data-ttu-id="1f97c-104">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="1f97c-104">PermissionLevel</span></span>

<span data-ttu-id="1f97c-105">L’élément **permissionLevel** représente le niveau d’autorisation dont dispose un utilisateur sur un dossier.</span><span class="sxs-lookup"><span data-stu-id="1f97c-105">The **PermissionLevel** element represents the permission level that a user has on a folder.</span></span> <span data-ttu-id="1f97c-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1f97c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 <span data-ttu-id="1f97c-107">**PermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="1f97c-107">**PermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f97c-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1f97c-108">Attributes and elements</span></span>

<span data-ttu-id="1f97c-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1f97c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f97c-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="1f97c-110">Attributes</span></span>

<span data-ttu-id="1f97c-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1f97c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f97c-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1f97c-112">Child elements</span></span>

<span data-ttu-id="1f97c-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1f97c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1f97c-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1f97c-114">Parent elements</span></span>

|<span data-ttu-id="1f97c-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1f97c-115">**Element**</span></span>|<span data-ttu-id="1f97c-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f97c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f97c-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="1f97c-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="1f97c-p103">Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1f97c-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1f97c-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="1f97c-120">Text value</span></span>

<span data-ttu-id="1f97c-121">Le tableau suivant répertorie les valeurs possibles pour l’élément **permissionLevel** .</span><span class="sxs-lookup"><span data-stu-id="1f97c-121">The following table lists the possible values for the **PermissionLevel** element.</span></span> 
  
<span data-ttu-id="1f97c-122">**Valeurs de texte de l’élément PermissionLevel**</span><span class="sxs-lookup"><span data-stu-id="1f97c-122">**PermissionLevel element text values**</span></span>

|<span data-ttu-id="1f97c-123">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1f97c-123">**Value**</span></span>|<span data-ttu-id="1f97c-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f97c-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f97c-125">Aucun</span><span class="sxs-lookup"><span data-stu-id="1f97c-125">None</span></span>  <br/> |<span data-ttu-id="1f97c-126">Indique que l’utilisateur ne dispose pas d’autorisations sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="1f97c-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="1f97c-127">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="1f97c-127">Owner</span></span>  <br/> |<span data-ttu-id="1f97c-128">Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments du dossier, et créer des sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="1f97c-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="1f97c-129">L’utilisateur est le propriétaire du dossier et le contact du dossier.</span><span class="sxs-lookup"><span data-stu-id="1f97c-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="1f97c-130">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="1f97c-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="1f97c-131">Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments du dossier, et créer des sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="1f97c-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="1f97c-132">Éditeur</span><span class="sxs-lookup"><span data-stu-id="1f97c-132">Editor</span></span>  <br/> |<span data-ttu-id="1f97c-133">Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments du dossier.</span><span class="sxs-lookup"><span data-stu-id="1f97c-133">Indicates that the user can create, read, edit, and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="1f97c-134">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="1f97c-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="1f97c-135">Indique que l’utilisateur peut créer et lire tous les éléments du dossier, modifier et supprimer uniquement les éléments que l’utilisateur crée et créer des sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="1f97c-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="1f97c-136">Auteur</span><span class="sxs-lookup"><span data-stu-id="1f97c-136">Author</span></span>  <br/> |<span data-ttu-id="1f97c-137">Indique que l’utilisateur peut créer et lire tous les éléments du dossier, et modifier et supprimer uniquement les éléments créés par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1f97c-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="1f97c-138">Noneditingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="1f97c-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="1f97c-139">Indique que l’utilisateur peut créer et lire tous les éléments du dossier, et supprimer uniquement les éléments créés par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1f97c-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="1f97c-140">Relecteur</span><span class="sxs-lookup"><span data-stu-id="1f97c-140">Reviewer</span></span>  <br/> |<span data-ttu-id="1f97c-141">Indique que l’utilisateur peut lire tous les éléments du dossier.</span><span class="sxs-lookup"><span data-stu-id="1f97c-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="1f97c-142">Collaborateur</span><span class="sxs-lookup"><span data-stu-id="1f97c-142">Contributor</span></span>  <br/> |<span data-ttu-id="1f97c-143">Indique que l’utilisateur peut créer des éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="1f97c-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="1f97c-144">Le contenu du dossier n’apparaît pas.</span><span class="sxs-lookup"><span data-stu-id="1f97c-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="1f97c-145">Personnalisé</span><span class="sxs-lookup"><span data-stu-id="1f97c-145">Custom</span></span>  <br/> |<span data-ttu-id="1f97c-146">Indique que l’utilisateur dispose d’autorisations d’accès personnalisées sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="1f97c-146">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1f97c-147">Remarques</span><span class="sxs-lookup"><span data-stu-id="1f97c-147">Remarks</span></span>

<span data-ttu-id="1f97c-148">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1f97c-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f97c-149">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1f97c-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f97c-150">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1f97c-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f97c-151">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1f97c-151">Schema Name</span></span>  <br/> |<span data-ttu-id="1f97c-152">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1f97c-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="1f97c-153">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1f97c-153">Validation File</span></span>  <br/> |<span data-ttu-id="1f97c-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1f97c-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f97c-155">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1f97c-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f97c-156">False</span><span class="sxs-lookup"><span data-stu-id="1f97c-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f97c-157">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1f97c-157">See also</span></span>



- [<span data-ttu-id="1f97c-158">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1f97c-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="1f97c-159">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="1f97c-159">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

