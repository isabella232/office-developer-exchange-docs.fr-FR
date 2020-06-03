---
title: ManagedFolderInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderInformation
api_type:
- schema
ms.assetid: dea980eb-8303-47fe-a380-20a8efc9ead6
description: L’élément ManagedFolderInformation contient des informations sur un dossier personnalisé géré.
ms.openlocfilehash: ce15dcb15cccdce253494beefd2f4a2a7a0c0ad8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44450948"
---
# <a name="managedfolderinformation"></a><span data-ttu-id="a4292-103">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="a4292-103">ManagedFolderInformation</span></span>

<span data-ttu-id="a4292-104">L’élément **ManagedFolderInformation** contient des informations sur un dossier personnalisé géré.</span><span class="sxs-lookup"><span data-stu-id="a4292-104">The **ManagedFolderInformation** element contains information about a managed custom folder.</span></span> 
  
```xml
<ManagedFolderInformation>
   <CanDelete/>
   <CanRenameOrMove/>
   <MustDisplayComment/>
   <HasQuota/>
   <IsManagedFoldersRoot/>
   <ManagedFolderId/>
   <Comment/>
   <StorageQuota/>
   <FolderSize/>
   <HomePage/>
</ManagedFolderInformation>
```

 <span data-ttu-id="a4292-105">**ManagedFolderInformationType**</span><span class="sxs-lookup"><span data-stu-id="a4292-105">**ManagedFolderInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4292-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a4292-106">Attributes and elements</span></span>

<span data-ttu-id="a4292-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a4292-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4292-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a4292-108">Attributes</span></span>

<span data-ttu-id="a4292-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a4292-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4292-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a4292-110">Child elements</span></span>

|<span data-ttu-id="a4292-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a4292-111">**Element**</span></span>|<span data-ttu-id="a4292-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a4292-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4292-113">CanDelete</span><span class="sxs-lookup"><span data-stu-id="a4292-113">CanDelete</span></span>](candelete.md) <br/> |<span data-ttu-id="a4292-114">Indique si un dossier géré peut être supprimé par un client.</span><span class="sxs-lookup"><span data-stu-id="a4292-114">Indicates whether a managed folder can be deleted by a customer.</span></span>  <br/> |
|[<span data-ttu-id="a4292-115">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="a4292-115">CanRenameOrMove</span></span>](canrenameormove.md) <br/> |<span data-ttu-id="a4292-116">Indique si un dossier géré donné peut être renommé ou déplacé par le client.</span><span class="sxs-lookup"><span data-stu-id="a4292-116">Indicates whether a given managed folder can be renamed or moved by the customer.</span></span>  <br/> |
|[<span data-ttu-id="a4292-117">MustDisplayComment</span><span class="sxs-lookup"><span data-stu-id="a4292-117">MustDisplayComment</span></span>](mustdisplaycomment.md) <br/> |<span data-ttu-id="a4292-118">Indique si le commentaire du dossier géré doit être affiché.</span><span class="sxs-lookup"><span data-stu-id="a4292-118">Indicates whether the managed folder comment must be displayed.</span></span>  <br/> |
|[<span data-ttu-id="a4292-119">HasQuota</span><span class="sxs-lookup"><span data-stu-id="a4292-119">HasQuota</span></span>](hasquota.md) <br/> |<span data-ttu-id="a4292-120">Indique si le dossier géré a un quota.</span><span class="sxs-lookup"><span data-stu-id="a4292-120">Indicates whether the managed folder has a quota.</span></span>  <br/> |
|[<span data-ttu-id="a4292-121">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="a4292-121">IsManagedFoldersRoot</span></span>](ismanagedfoldersroot.md) <br/> |<span data-ttu-id="a4292-122">Indique si le dossier géré est la racine de tous les dossiers gérés.</span><span class="sxs-lookup"><span data-stu-id="a4292-122">Indicates whether the managed folder is the root for all managed folders.</span></span>  <br/> |
|[<span data-ttu-id="a4292-123">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="a4292-123">ManagedFolderId</span></span>](managedfolderid.md) <br/> |<span data-ttu-id="a4292-124">Contient l’ID de dossier du dossier géré.</span><span class="sxs-lookup"><span data-stu-id="a4292-124">Contains the folder ID of the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="a4292-125">Comment</span><span class="sxs-lookup"><span data-stu-id="a4292-125">Comment</span></span>](comment.md) <br/> |<span data-ttu-id="a4292-126">Contient le commentaire associé à un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="a4292-126">Contains the comment that is associated with a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="a4292-127">StorageQuota</span><span class="sxs-lookup"><span data-stu-id="a4292-127">StorageQuota</span></span>](storagequota.md) <br/> |<span data-ttu-id="a4292-128">Décrit le quota de stockage pour le dossier géré.</span><span class="sxs-lookup"><span data-stu-id="a4292-128">Describes the storage quota for the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="a4292-129">FolderSize</span><span class="sxs-lookup"><span data-stu-id="a4292-129">FolderSize</span></span>](foldersize.md) <br/> |<span data-ttu-id="a4292-130">Décrit la taille totale de tout le contenu d’un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="a4292-130">Describes the total size of all the contents of a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="a4292-131">HomePage</span><span class="sxs-lookup"><span data-stu-id="a4292-131">HomePage</span></span>](homepage.md) <br/> |<span data-ttu-id="a4292-132">Spécifie l’URL qui sera la page d’accueil par défaut pour le dossier géré.</span><span class="sxs-lookup"><span data-stu-id="a4292-132">Specifies the URL that will be the default home page for the managed folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a4292-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a4292-133">Parent elements</span></span>

|<span data-ttu-id="a4292-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a4292-134">**Element**</span></span>|<span data-ttu-id="a4292-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="a4292-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4292-136">Folder</span><span class="sxs-lookup"><span data-stu-id="a4292-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="a4292-137">Représente un dossier dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="a4292-137">Represents a folder in the Exchange store.</span></span> <span data-ttu-id="a4292-138">Les dossiers personnalisés gérés ne peuvent être que des sous-dossiers du dossier nommé **Managed Folders**.</span><span class="sxs-lookup"><span data-stu-id="a4292-138">Managed custom folders can only be subfolders of the folder named **Managed Folders**.</span></span>  <br/> |
|[<span data-ttu-id="a4292-139">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="a4292-139">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="a4292-140">Non applicable</span><span class="sxs-lookup"><span data-stu-id="a4292-140">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="a4292-141">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="a4292-141">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="a4292-142">Non applicable</span><span class="sxs-lookup"><span data-stu-id="a4292-142">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="a4292-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="a4292-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="a4292-144">Non applicable</span><span class="sxs-lookup"><span data-stu-id="a4292-144">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="a4292-145">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="a4292-145">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="a4292-146">Non applicable</span><span class="sxs-lookup"><span data-stu-id="a4292-146">Not applicable.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a4292-147">Remarques</span><span class="sxs-lookup"><span data-stu-id="a4292-147">Remarks</span></span>

<span data-ttu-id="a4292-148">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a4292-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4292-149">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a4292-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4292-150">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a4292-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a4292-151">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a4292-151">Schema name</span></span>  <br/> |<span data-ttu-id="a4292-152">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a4292-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="a4292-153">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a4292-153">Validation file</span></span>  <br/> |<span data-ttu-id="a4292-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a4292-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a4292-155">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a4292-155">Can be empty</span></span>  <br/> |<span data-ttu-id="a4292-156">False</span><span class="sxs-lookup"><span data-stu-id="a4292-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4292-157">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a4292-157">See also</span></span>



[<span data-ttu-id="a4292-158">Opération CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="a4292-158">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="a4292-159">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a4292-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a4292-160">Ajout de dossiers gérés</span><span class="sxs-lookup"><span data-stu-id="a4292-160">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

