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
ms.openlocfilehash: 7cc734f5807fe039467065315c220341f47d3fb4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828730"
---
# <a name="permissionlevel"></a><span data-ttu-id="d4f4f-104">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="d4f4f-104">PermissionLevel</span></span>

<span data-ttu-id="d4f4f-105">L’élément **PermissionLevel** représente le niveau d’autorisation dont dispose un utilisateur sur un dossier.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-105">The **PermissionLevel** element represents the permission level that a user has on a folder.</span></span> <span data-ttu-id="d4f4f-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d4f4f-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 <span data-ttu-id="d4f4f-107">**PermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="d4f4f-107">**PermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4f4f-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4f4f-108">Attributes and elements</span></span>

<span data-ttu-id="d4f4f-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4f4f-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4f4f-110">Attributes</span></span>

<span data-ttu-id="d4f4f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4f4f-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4f4f-112">Child elements</span></span>

<span data-ttu-id="d4f4f-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4f4f-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4f4f-114">Parent elements</span></span>

|<span data-ttu-id="d4f4f-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4f4f-115">**Element**</span></span>|<span data-ttu-id="d4f4f-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4f4f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4f4f-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="d4f4f-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="d4f4f-p103">Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d4f4f-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d4f4f-120">Text value</span></span>

<span data-ttu-id="d4f4f-121">Le tableau suivant répertorie les valeurs possibles pour l’élément **PermissionLevel** .</span><span class="sxs-lookup"><span data-stu-id="d4f4f-121">The following table lists the possible values for the **PermissionLevel** element.</span></span> 
  
<span data-ttu-id="d4f4f-122">**Valeurs de texte des éléments PermissionLevel**</span><span class="sxs-lookup"><span data-stu-id="d4f4f-122">**PermissionLevel element text values**</span></span>

|<span data-ttu-id="d4f4f-123">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d4f4f-123">**Value**</span></span>|<span data-ttu-id="d4f4f-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4f4f-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4f4f-125">None</span><span class="sxs-lookup"><span data-stu-id="d4f4f-125">None</span></span>  <br/> |<span data-ttu-id="d4f4f-126">Indique que l’utilisateur n’a aucune autorisation sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="d4f4f-127">Owner</span><span class="sxs-lookup"><span data-stu-id="d4f4f-127">Owner</span></span>  <br/> |<span data-ttu-id="d4f4f-128">Indique que l’utilisateur peut créer, lire, modifier, supprimer tous les éléments dans le dossier et créer des sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="d4f4f-129">L’utilisateur est propriétaire du dossier et contact du dossier.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="d4f4f-130">Détenir</span><span class="sxs-lookup"><span data-stu-id="d4f4f-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="d4f4f-131">Indique que l’utilisateur peut créer, lire, modifier, supprimer tous les éléments dans le dossier et créer des sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="d4f4f-132">Editor</span><span class="sxs-lookup"><span data-stu-id="d4f4f-132">Editor</span></span>  <br/> |<span data-ttu-id="d4f4f-133">Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-133">Indicates that the user can create, read, edit, and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="d4f4f-134">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="d4f4f-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="d4f4f-135">Indique que l’utilisateur peut créer et lire tous les éléments dans le dossier, modifier et supprimer uniquement les éléments créés par l’utilisateur et créer des sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="d4f4f-136">Auteur</span><span class="sxs-lookup"><span data-stu-id="d4f4f-136">Author</span></span>  <br/> |<span data-ttu-id="d4f4f-137">Indique que l’utilisateur peut créer et lire tous les éléments dans le dossier, modifier et supprimer uniquement les éléments créés par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="d4f4f-138">NoneditingAuthor</span><span class="sxs-lookup"><span data-stu-id="d4f4f-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="d4f4f-139">Indique que l’utilisateur peut créer et lire tous les éléments dans le dossier et supprimer uniquement les éléments créés par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="d4f4f-140">Reviewer</span><span class="sxs-lookup"><span data-stu-id="d4f4f-140">Reviewer</span></span>  <br/> |<span data-ttu-id="d4f4f-141">Indique que l’utilisateur peut lire tous les éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="d4f4f-142">Collaborateur</span><span class="sxs-lookup"><span data-stu-id="d4f4f-142">Contributor</span></span>  <br/> |<span data-ttu-id="d4f4f-143">Indique que l’utilisateur peut créer des éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="d4f4f-144">Le contenu du dossier n’apparaître pas.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="d4f4f-145">Personnalisé</span><span class="sxs-lookup"><span data-stu-id="d4f4f-145">Custom</span></span>  <br/> |<span data-ttu-id="d4f4f-146">Indique que l’utilisateur dispose des autorisations d’accès personnalisées sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-146">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d4f4f-147">Remarques</span><span class="sxs-lookup"><span data-stu-id="d4f4f-147">Remarks</span></span>

<span data-ttu-id="d4f4f-148">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d4f4f-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4f4f-149">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4f4f-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4f4f-150">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4f4f-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4f4f-151">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4f4f-151">Schema Name</span></span>  <br/> |<span data-ttu-id="d4f4f-152">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d4f4f-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4f4f-153">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4f4f-153">Validation File</span></span>  <br/> |<span data-ttu-id="d4f4f-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4f4f-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4f4f-155">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4f4f-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4f4f-156">False</span><span class="sxs-lookup"><span data-stu-id="d4f4f-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4f4f-157">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4f4f-157">See also</span></span>



- [<span data-ttu-id="d4f4f-158">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d4f4f-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d4f4f-159">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="d4f4f-159">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

