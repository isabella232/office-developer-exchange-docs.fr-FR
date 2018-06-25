---
title: Dossier tâches
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolder
api_type:
- schema
ms.assetid: 5a9a4612-8064-4986-b467-c44f268c64df
description: L’élément du dossier tâches représente un dossier de tâches qui se trouve dans une boîte aux lettres.
ms.openlocfilehash: b2151c68519a6ff15fbc74b48fc93a7e06af9e76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838674"
---
# <a name="tasksfolder"></a><span data-ttu-id="61c30-103">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="61c30-103">TasksFolder</span></span>

<span data-ttu-id="61c30-104">L’élément du **dossier tâches** représente un dossier de tâches qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="61c30-104">The **TasksFolder** element represents a Tasks folder that is contained in a mailbox.</span></span> 
  
```xml
<TasksFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <PermissionSet/>
      <EffectiveRights/>
</TasksFolder>
```

<span data-ttu-id="61c30-105">**TasksFolderType**</span><span class="sxs-lookup"><span data-stu-id="61c30-105">**TasksFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="61c30-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="61c30-106">Attributes and elements</span></span>

<span data-ttu-id="61c30-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="61c30-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61c30-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="61c30-108">Attributes</span></span>

<span data-ttu-id="61c30-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="61c30-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61c30-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="61c30-110">Child elements</span></span>

|<span data-ttu-id="61c30-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="61c30-111">**Element**</span></span>|<span data-ttu-id="61c30-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="61c30-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61c30-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="61c30-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="61c30-114">Contient la clé d’identificateur et de modification d’un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="61c30-114">Contains the identifier and change key of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="61c30-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="61c30-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="61c30-116">Représente l’identificateur du dossier parent qui contient le dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="61c30-116">Represents the identifier of the parent folder that contains the Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="61c30-117">Classe FolderClass</span><span class="sxs-lookup"><span data-stu-id="61c30-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="61c30-118">Représente la classe de dossier pour un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="61c30-118">Represents the folder class for a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="61c30-119">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="61c30-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="61c30-120">Contient le nom complet d’un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="61c30-120">Contains the display name of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="61c30-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="61c30-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="61c30-122">Représente le nombre total d’éléments dans un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="61c30-122">Represents the total count of items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="61c30-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="61c30-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="61c30-124">Représente le nombre de dossiers enfants qui sont contenues dans un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="61c30-124">Represents the number of child folders that are contained within a Tasks folder.</span></span> <span data-ttu-id="61c30-125">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="61c30-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="61c30-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="61c30-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="61c30-127">Identifie les propriétés étendues sur un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="61c30-127">Identifies extended properties on a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="61c30-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="61c30-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="61c30-129">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="61c30-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="61c30-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="61c30-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="61c30-131">Représente le nombre d’éléments non lus dans un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="61c30-131">Represents the count of unread items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="61c30-132">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="61c30-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="61c30-133">Contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="61c30-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="61c30-134">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="61c30-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="61c30-135">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="61c30-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="61c30-136">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="61c30-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="61c30-137">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="61c30-137">This element is read-only.</span></span> <span data-ttu-id="61c30-138">Cet élément a été introduit dans Microsoft Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="61c30-138">This element was introduced in Microsoft Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="61c30-139">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="61c30-139">Parent elements</span></span>

|<span data-ttu-id="61c30-140">**Élément**</span><span class="sxs-lookup"><span data-stu-id="61c30-140">**Element**</span></span>|<span data-ttu-id="61c30-141">**Description**</span><span class="sxs-lookup"><span data-stu-id="61c30-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61c30-142">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="61c30-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="61c30-143">Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="61c30-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="61c30-144">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="61c30-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="61c30-145">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="61c30-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="61c30-146">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="61c30-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="61c30-147">Représente une mise à jour d’une propriété donnée sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="61c30-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="61c30-148">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="61c30-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="61c30-149">Identifie un seul dossier pour mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="61c30-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="61c30-150">Dossiers</span><span class="sxs-lookup"><span data-stu-id="61c30-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="61c30-151">Contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="61c30-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="61c30-152">Remarques</span><span class="sxs-lookup"><span data-stu-id="61c30-152">Remarks</span></span>

<span data-ttu-id="61c30-153">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="61c30-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61c30-154">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="61c30-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61c30-155">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="61c30-155">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61c30-156">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="61c30-156">Schema Name</span></span>  <br/> |<span data-ttu-id="61c30-157">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="61c30-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="61c30-158">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="61c30-158">Validation File</span></span>  <br/> |<span data-ttu-id="61c30-159">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="61c30-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61c30-160">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="61c30-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="61c30-161">False</span><span class="sxs-lookup"><span data-stu-id="61c30-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61c30-162">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="61c30-162">See also</span></span>

- [<span data-ttu-id="61c30-163">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="61c30-163">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

