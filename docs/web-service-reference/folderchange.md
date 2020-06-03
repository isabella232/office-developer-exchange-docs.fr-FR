---
title: FolderChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderChange
api_type:
- schema
ms.assetid: 23279750-131b-4e1a-b7d1-be235c4e0891
description: L’élément FolderChange, représente une collection de modifications à effectuer sur un seul dossier.
ms.openlocfilehash: e4a025bef100fdd478be545b6448b15886e47c60
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530238"
---
# <a name="folderchange"></a><span data-ttu-id="1f93e-103">FolderChange</span><span class="sxs-lookup"><span data-stu-id="1f93e-103">FolderChange</span></span>

<span data-ttu-id="1f93e-104">L’élément **FolderChange,** représente une collection de modifications à effectuer sur un seul dossier.</span><span class="sxs-lookup"><span data-stu-id="1f93e-104">The **FolderChange** element represents a collection of changes to be performed on a single folder.</span></span> 
  
- [<span data-ttu-id="1f93e-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="1f93e-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="1f93e-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="1f93e-106">FolderChanges</span></span>](folderchanges.md) 
- [<span data-ttu-id="1f93e-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="1f93e-107">FolderChange</span></span>](folderchange.md)
  
```xml
<FolderChange>
   <FolderId/>
   <Updates/>
</FolderChange>
```

```xml
<FolderChange>
   <DistinguishedFolderId/>
   <Updates/>
</FolderChange>
```

<span data-ttu-id="1f93e-108">**FolderChangeType**</span><span class="sxs-lookup"><span data-stu-id="1f93e-108">**FolderChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1f93e-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1f93e-109">Attributes and elements</span></span>

<span data-ttu-id="1f93e-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1f93e-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f93e-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="1f93e-111">Attributes</span></span>

<span data-ttu-id="1f93e-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1f93e-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f93e-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1f93e-113">Child elements</span></span>

|<span data-ttu-id="1f93e-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1f93e-114">**Element**</span></span>|<span data-ttu-id="1f93e-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f93e-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f93e-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="1f93e-116">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="1f93e-117">Contient l’identificateur et la clé de modification d’un dossier à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="1f93e-117">Contains the identifier and change key of a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="1f93e-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="1f93e-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="1f93e-119">Identifie les dossiers MicrosoftExchange Server 2007 qui peuvent être référencés par nom.</span><span class="sxs-lookup"><span data-stu-id="1f93e-119">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
|[<span data-ttu-id="1f93e-120">Mises à jour (dossier)</span><span class="sxs-lookup"><span data-stu-id="1f93e-120">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="1f93e-121">Définit le type de mise à jour effectué sur un dossier identifié par l’élément [FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="1f93e-121">Defines the type of update that is performed on a folder that is identified by either the [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f93e-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1f93e-122">Parent elements</span></span>

|<span data-ttu-id="1f93e-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1f93e-123">**Element**</span></span>|<span data-ttu-id="1f93e-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f93e-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f93e-125">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="1f93e-125">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="1f93e-126">Représente une collection de modifications apportées à un dossier.</span><span class="sxs-lookup"><span data-stu-id="1f93e-126">Represents a collection of changes for a folder.</span></span>  <br/> <span data-ttu-id="1f93e-127">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="1f93e-127">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1f93e-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="1f93e-128">Remarks</span></span>

<span data-ttu-id="1f93e-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1f93e-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f93e-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1f93e-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f93e-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1f93e-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f93e-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1f93e-132">Schema name</span></span>  <br/> |<span data-ttu-id="1f93e-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1f93e-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="1f93e-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1f93e-134">Validation file</span></span>  <br/> |<span data-ttu-id="1f93e-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1f93e-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f93e-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1f93e-136">Can be empty</span></span>  <br/> |<span data-ttu-id="1f93e-137">False</span><span class="sxs-lookup"><span data-stu-id="1f93e-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f93e-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1f93e-138">See also</span></span>

- [<span data-ttu-id="1f93e-139">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="1f93e-139">UpdateFolder operation</span></span>](updatefolder-operation.md)

