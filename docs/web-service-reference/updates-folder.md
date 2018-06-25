---
title: Mises à jour (dossier)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: b047e3a4-a5ab-4098-b7a0-273bc809e702
description: L’élément de mises à jour contient un ensemble d’éléments qui définissent append, définir et supprimer les modifications apportées aux propriétés d’un dossier.
ms.openlocfilehash: 31f25b1e88fb8756f189a6d75259dd4fc198582f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838915"
---
# <a name="updates-folder"></a><span data-ttu-id="870ff-103">Mises à jour (dossier)</span><span class="sxs-lookup"><span data-stu-id="870ff-103">Updates (Folder)</span></span>

<span data-ttu-id="870ff-104">L’élément de **mises à jour** contient un ensemble d’éléments qui définissent append, définir et supprimer les modifications apportées aux propriétés d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="870ff-104">The **Updates** element contains a set of elements that define append, set, and delete changes to folder properties.</span></span> 
  
- [<span data-ttu-id="870ff-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="870ff-105">UpdateFolder</span></span>](updatefolder.md)
  
- [<span data-ttu-id="870ff-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="870ff-106">FolderChanges</span></span>](folderchanges.md)
  
- [<span data-ttu-id="870ff-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="870ff-107">FolderChange</span></span>](folderchange.md)
  
- [<span data-ttu-id="870ff-108">Mises à jour (dossier)</span><span class="sxs-lookup"><span data-stu-id="870ff-108">Updates (Folder)</span></span>](updates-folder.md)
  
```xml
<Updates>
   <AppendToFolderField/>
   <SetFolderField/>
   <DeleteFolderField/>
</Updates>
```

<span data-ttu-id="870ff-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="870ff-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="870ff-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="870ff-110">Attributes and elements</span></span>

<span data-ttu-id="870ff-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="870ff-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="870ff-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="870ff-112">Attributes</span></span>

<span data-ttu-id="870ff-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="870ff-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="870ff-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="870ff-114">Child elements</span></span>

|<span data-ttu-id="870ff-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="870ff-115">**Element**</span></span>|<span data-ttu-id="870ff-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="870ff-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="870ff-117">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="870ff-117">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="870ff-118">Représente les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="870ff-118">Represents data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="870ff-119">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="870ff-119">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="870ff-120">Représente une mise à jour d’une propriété donnée sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="870ff-120">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="870ff-121">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="870ff-121">DeleteFolderField</span></span>](deletefolderfield.md) <br/> |<span data-ttu-id="870ff-122">Représente une opération de suppression d’une propriété donnée d’un dossier pendant une [opération UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="870ff-122">Represents an operation to delete a given property from a folder during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="870ff-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="870ff-123">Parent elements</span></span>

|<span data-ttu-id="870ff-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="870ff-124">**Element**</span></span>|<span data-ttu-id="870ff-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="870ff-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="870ff-126">FolderChange</span><span class="sxs-lookup"><span data-stu-id="870ff-126">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="870ff-127">Représente une collection des modifications à effectuer sur un seul dossier.</span><span class="sxs-lookup"><span data-stu-id="870ff-127">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="870ff-128">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/UpdateFolder/FolderChanges/FolderChange[i]`</span><span class="sxs-lookup"><span data-stu-id="870ff-128">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="870ff-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="870ff-129">Remarks</span></span>

<span data-ttu-id="870ff-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="870ff-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="870ff-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="870ff-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="870ff-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="870ff-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="870ff-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="870ff-133">Schema Name</span></span>  <br/> |<span data-ttu-id="870ff-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="870ff-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="870ff-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="870ff-135">Validation File</span></span>  <br/> |<span data-ttu-id="870ff-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="870ff-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="870ff-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="870ff-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="870ff-138">False</span><span class="sxs-lookup"><span data-stu-id="870ff-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="870ff-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="870ff-139">See also</span></span>

- [<span data-ttu-id="870ff-140">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="870ff-140">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="870ff-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="870ff-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

