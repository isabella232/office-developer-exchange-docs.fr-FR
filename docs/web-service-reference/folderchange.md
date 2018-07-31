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
description: L’élément FolderChange représente une collection des modifications à effectuer sur un seul dossier.
ms.openlocfilehash: f25defa9974f7b5dd0c683c7657983741890d45d
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354329"
---
# <a name="folderchange"></a><span data-ttu-id="9b315-103">FolderChange</span><span class="sxs-lookup"><span data-stu-id="9b315-103">FolderChange</span></span>

<span data-ttu-id="9b315-104">L’élément **FolderChange** représente une collection des modifications à effectuer sur un seul dossier.</span><span class="sxs-lookup"><span data-stu-id="9b315-104">The **FolderChange** element represents a collection of changes to be performed on a single folder.</span></span> 
  
- [<span data-ttu-id="9b315-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="9b315-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="9b315-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="9b315-106">FolderChanges</span></span>](folderchanges.md) 
- [<span data-ttu-id="9b315-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="9b315-107">FolderChange</span></span>](folderchange.md)
  
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

<span data-ttu-id="9b315-108">**FolderChangeType**</span><span class="sxs-lookup"><span data-stu-id="9b315-108">**FolderChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9b315-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9b315-109">Attributes and elements</span></span>

<span data-ttu-id="9b315-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9b315-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b315-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="9b315-111">Attributes</span></span>

<span data-ttu-id="9b315-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9b315-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b315-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9b315-113">Child elements</span></span>

|<span data-ttu-id="9b315-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9b315-114">**Element**</span></span>|<span data-ttu-id="9b315-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="9b315-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b315-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="9b315-116">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="9b315-117">Contient la clé d’identificateur et de modification d’un dossier à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="9b315-117">Contains the identifier and change key of a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="9b315-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="9b315-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="9b315-119">Identifie les dossiers MicrosoftExchange Server 2007 qui peuvent être référencés par son nom.</span><span class="sxs-lookup"><span data-stu-id="9b315-119">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
|[<span data-ttu-id="9b315-120">Updates (Folder)</span><span class="sxs-lookup"><span data-stu-id="9b315-120">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="9b315-121">Définit le type de mise à jour est effectuée sur un dossier identifié par [l’ID FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) élément.</span><span class="sxs-lookup"><span data-stu-id="9b315-121">Defines the type of update that is performed on a folder that is identified by either the [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b315-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9b315-122">Parent elements</span></span>

|<span data-ttu-id="9b315-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9b315-123">**Element**</span></span>|<span data-ttu-id="9b315-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="9b315-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b315-125">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="9b315-125">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="9b315-126">Représente une collection des modifications pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="9b315-126">Represents a collection of changes for a folder.</span></span>  <br/> <span data-ttu-id="9b315-127">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="9b315-127">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b315-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="9b315-128">Remarks</span></span>

<span data-ttu-id="9b315-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="9b315-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b315-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9b315-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b315-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9b315-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b315-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9b315-132">Schema name</span></span>  <br/> |<span data-ttu-id="9b315-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9b315-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b315-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9b315-134">Validation file</span></span>  <br/> |<span data-ttu-id="9b315-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9b315-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b315-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9b315-136">Can be empty</span></span>  <br/> |<span data-ttu-id="9b315-137">False</span><span class="sxs-lookup"><span data-stu-id="9b315-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b315-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9b315-138">See also</span></span>

- [<span data-ttu-id="9b315-139">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="9b315-139">UpdateFolder operation</span></span>](updatefolder-operation.md)

