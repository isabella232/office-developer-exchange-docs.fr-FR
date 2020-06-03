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
description: L’élément DeleteFolderField représente une opération permettant de supprimer une propriété donnée d’un dossier lors d’un appel UpdateFolder.
ms.openlocfilehash: a0b48b667c8c8afbd5729d5deb84359a6a6ccc25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462156"
---
# <a name="deletefolderfield"></a><span data-ttu-id="eaf01-103">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="eaf01-103">DeleteFolderField</span></span>

<span data-ttu-id="eaf01-104">L’élément **DeleteFolderField** représente une opération permettant de supprimer une propriété donnée d’un dossier lors d’un appel UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="eaf01-104">The **DeleteFolderField** element represents an operation to delete a given property from a folder during an UpdateFolder call.</span></span> 
  
- [<span data-ttu-id="eaf01-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="eaf01-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="eaf01-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="eaf01-106">FolderChanges</span></span>](folderchanges.md)  
- [<span data-ttu-id="eaf01-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="eaf01-107">FolderChange</span></span>](folderchange.md)  
- [<span data-ttu-id="eaf01-108">Mises à jour (dossier)</span><span class="sxs-lookup"><span data-stu-id="eaf01-108">Updates (Folder)</span></span>](updates-folder.md) 
- [<span data-ttu-id="eaf01-109">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="eaf01-109">DeleteFolderField</span></span>](deletefolderfield.md)
  
```xml
<DeleteFolderField>
   <FieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <ExtendedFieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <IndexedFieldURI/>
</DeleteFolderField>
```

<span data-ttu-id="eaf01-110">**DeleteFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="eaf01-110">**DeleteFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="eaf01-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="eaf01-111">Attributes and elements</span></span>

<span data-ttu-id="eaf01-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="eaf01-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eaf01-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="eaf01-113">Attributes</span></span>

<span data-ttu-id="eaf01-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="eaf01-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eaf01-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="eaf01-115">Child elements</span></span>

|<span data-ttu-id="eaf01-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eaf01-116">**Element**</span></span>|<span data-ttu-id="eaf01-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="eaf01-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eaf01-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="eaf01-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="eaf01-119">Identifie les propriétés référencées fréquemment par URI.</span><span class="sxs-lookup"><span data-stu-id="eaf01-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="eaf01-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="eaf01-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="eaf01-121">Identifie les membres individuels d’une propriété de dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="eaf01-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="eaf01-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="eaf01-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="eaf01-123">Identifie les propriétés MAPI étendues.</span><span class="sxs-lookup"><span data-stu-id="eaf01-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eaf01-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="eaf01-124">Parent elements</span></span>

|<span data-ttu-id="eaf01-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eaf01-125">**Element**</span></span>|<span data-ttu-id="eaf01-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="eaf01-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eaf01-127">Mises à jour (dossier)</span><span class="sxs-lookup"><span data-stu-id="eaf01-127">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="eaf01-128">Contient un ensemble d’éléments qui définissent les modifications apportées par l’ajout, la définition et la suppression aux propriétés du dossier.</span><span class="sxs-lookup"><span data-stu-id="eaf01-128">Contains a set of elements that define append, set, and delete changes to folder properties.</span></span>  <br/> <span data-ttu-id="eaf01-129">Voici l’expression XPath de cet élément :`/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="eaf01-129">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eaf01-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="eaf01-130">Remarks</span></span>

<span data-ttu-id="eaf01-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="eaf01-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eaf01-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="eaf01-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eaf01-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="eaf01-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eaf01-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="eaf01-134">Schema Name</span></span>  <br/> |<span data-ttu-id="eaf01-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="eaf01-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="eaf01-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="eaf01-136">Validation File</span></span>  <br/> |<span data-ttu-id="eaf01-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eaf01-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eaf01-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="eaf01-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="eaf01-139">False</span><span class="sxs-lookup"><span data-stu-id="eaf01-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eaf01-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="eaf01-140">See also</span></span>

- [<span data-ttu-id="eaf01-141">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="eaf01-141">UpdateFolder operation</span></span>](updatefolder-operation.md)

