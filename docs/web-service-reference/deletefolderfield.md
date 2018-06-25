---
title: DeleteFolderField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderField
api_type:
- schema
ms.assetid: f9c2187b-4c60-4358-b4b4-ede50eadae48
description: L’élément DeleteFolderField représente une opération de suppression d’une propriété donnée d’un dossier pendant un appel UpdateFolder.
ms.openlocfilehash: d0a5fb18c5f3445982a6417007ad6af9b1b365af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755860"
---
# <a name="deletefolderfield"></a><span data-ttu-id="4f903-103">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="4f903-103">DeleteFolderField</span></span>

<span data-ttu-id="4f903-104">L’élément **DeleteFolderField** représente une opération de suppression d’une propriété donnée d’un dossier pendant un appel UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="4f903-104">The **DeleteFolderField** element represents an operation to delete a given property from a folder during an UpdateFolder call.</span></span> 
  
- [<span data-ttu-id="4f903-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="4f903-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="4f903-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="4f903-106">FolderChanges</span></span>](folderchanges.md)  
- [<span data-ttu-id="4f903-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="4f903-107">FolderChange</span></span>](folderchange.md)  
- [<span data-ttu-id="4f903-108">Mises à jour (dossier)</span><span class="sxs-lookup"><span data-stu-id="4f903-108">Updates (Folder)</span></span>](updates-folder.md) 
- [<span data-ttu-id="4f903-109">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="4f903-109">DeleteFolderField</span></span>](deletefolderfield.md)
  
```xml
<DeleteFolderField>
   <FieldURI/>
</DeleteFolderField>
```

 <span data-ttu-id="4f903-110">**DeleteFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="4f903-110">**DeleteFolderFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f903-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4f903-111">Attributes and elements</span></span>

<span data-ttu-id="4f903-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4f903-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f903-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="4f903-113">Attributes</span></span>

<span data-ttu-id="4f903-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4f903-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f903-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4f903-115">Child elements</span></span>

|<span data-ttu-id="4f903-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4f903-116">**Element**</span></span>|<span data-ttu-id="4f903-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f903-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f903-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="4f903-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="4f903-119">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="4f903-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="4f903-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="4f903-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="4f903-121">Identifie les membres individuels d’une propriété de dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="4f903-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="4f903-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="4f903-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="4f903-123">Identifie les propriétés MAPI étendues.</span><span class="sxs-lookup"><span data-stu-id="4f903-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4f903-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4f903-124">Parent elements</span></span>

|<span data-ttu-id="4f903-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4f903-125">**Element**</span></span>|<span data-ttu-id="4f903-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f903-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f903-127">Mises à jour (dossier)</span><span class="sxs-lookup"><span data-stu-id="4f903-127">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="4f903-128">Contient un ensemble d’éléments qui définissent append, définir et supprimer les modifications apportées aux propriétés d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="4f903-128">Contains a set of elements that define append, set, and delete changes to folder properties.</span></span>  <br/> <span data-ttu-id="4f903-129">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="4f903-129">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4f903-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="4f903-130">Remarks</span></span>

<span data-ttu-id="4f903-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4f903-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f903-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4f903-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f903-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4f903-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4f903-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4f903-134">Schema Name</span></span>  <br/> |<span data-ttu-id="4f903-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4f903-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="4f903-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4f903-136">Validation File</span></span>  <br/> |<span data-ttu-id="4f903-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4f903-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4f903-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4f903-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="4f903-139">False</span><span class="sxs-lookup"><span data-stu-id="4f903-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f903-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4f903-140">See also</span></span>

- [<span data-ttu-id="4f903-141">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="4f903-141">UpdateFolder operation</span></span>](updatefolder-operation.md)

