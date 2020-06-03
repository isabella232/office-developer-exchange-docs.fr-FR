---
title: TasksFolder
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
description: L’élément TasksFolder représente un dossier tâches contenu dans une boîte aux lettres.
ms.openlocfilehash: 522fe485482bd8159927f9925b7a5582ba2e1c22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465337"
---
# <a name="tasksfolder"></a><span data-ttu-id="ef857-103">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="ef857-103">TasksFolder</span></span>

<span data-ttu-id="ef857-104">L’élément **TasksFolder** représente un dossier tâches contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ef857-104">The **TasksFolder** element represents a Tasks folder that is contained in a mailbox.</span></span> 
  
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

<span data-ttu-id="ef857-105">**TasksFolderType**</span><span class="sxs-lookup"><span data-stu-id="ef857-105">**TasksFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ef857-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ef857-106">Attributes and elements</span></span>

<span data-ttu-id="ef857-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ef857-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef857-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ef857-108">Attributes</span></span>

<span data-ttu-id="ef857-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ef857-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef857-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ef857-110">Child elements</span></span>

|<span data-ttu-id="ef857-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ef857-111">**Element**</span></span>|<span data-ttu-id="ef857-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ef857-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef857-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="ef857-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="ef857-114">Contient l’identificateur et la clé de modification d’un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="ef857-114">Contains the identifier and change key of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="ef857-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ef857-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ef857-116">Représente l’identificateur du dossier parent qui contient le dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="ef857-116">Represents the identifier of the parent folder that contains the Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="ef857-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="ef857-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="ef857-118">Représente la classe Folder d’un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="ef857-118">Represents the folder class for a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="ef857-119">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="ef857-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="ef857-120">Contient le nom complet d’un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="ef857-120">Contains the display name of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="ef857-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ef857-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="ef857-122">Représente le nombre total d’éléments au sein d’un dossier de tâches.</span><span class="sxs-lookup"><span data-stu-id="ef857-122">Represents the total count of items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="ef857-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="ef857-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="ef857-124">Représente le nombre de dossiers enfants contenus dans un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="ef857-124">Represents the number of child folders that are contained within a Tasks folder.</span></span> <span data-ttu-id="ef857-125">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="ef857-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ef857-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="ef857-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="ef857-127">Identifie les propriétés étendues d’un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="ef857-127">Identifies extended properties on a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="ef857-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="ef857-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="ef857-129">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="ef857-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="ef857-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="ef857-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="ef857-131">Représente le nombre d’éléments non lus dans un dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="ef857-131">Represents the count of unread items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="ef857-132">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="ef857-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="ef857-133">Contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="ef857-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="ef857-134">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ef857-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="ef857-135">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="ef857-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="ef857-136">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="ef857-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="ef857-137">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="ef857-137">This element is read-only.</span></span> <span data-ttu-id="ef857-138">Cet élément a été introduit dans Microsoft Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ef857-138">This element was introduced in Microsoft Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ef857-139">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ef857-139">Parent elements</span></span>

|<span data-ttu-id="ef857-140">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ef857-140">**Element**</span></span>|<span data-ttu-id="ef857-141">**Description**</span><span class="sxs-lookup"><span data-stu-id="ef857-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef857-142">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="ef857-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="ef857-143">Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ef857-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ef857-144">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="ef857-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="ef857-145">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="ef857-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ef857-146">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="ef857-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="ef857-147">Représente une mise à jour d’une propriété unique sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ef857-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ef857-148">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="ef857-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="ef857-149">Identifie un dossier unique à mettre à jour dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="ef857-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ef857-150">Dossiers</span><span class="sxs-lookup"><span data-stu-id="ef857-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ef857-151">Contient un tableau de dossiers utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="ef857-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ef857-152">Remarques</span><span class="sxs-lookup"><span data-stu-id="ef857-152">Remarks</span></span>

<span data-ttu-id="ef857-153">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ef857-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef857-154">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ef857-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef857-155">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ef857-155">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ef857-156">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ef857-156">Schema Name</span></span>  <br/> |<span data-ttu-id="ef857-157">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ef857-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="ef857-158">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ef857-158">Validation File</span></span>  <br/> |<span data-ttu-id="ef857-159">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ef857-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ef857-160">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ef857-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef857-161">False</span><span class="sxs-lookup"><span data-stu-id="ef857-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef857-162">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ef857-162">See also</span></span>

- [<span data-ttu-id="ef857-163">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ef857-163">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

