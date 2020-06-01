---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: L’élément EmptyFolder définit une demande de vidage d’un dossier dans une boîte aux lettres dans la Banque d’Exchange. Vous pouvez également supprimer des sous-dossiers lorsque le dossier est vidé.
ms.openlocfilehash: a42e4e3f25741a96ee65fe6f87fc3236b68f4dc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457276"
---
# <a name="emptyfolder"></a><span data-ttu-id="7c96e-104">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="7c96e-104">EmptyFolder</span></span>

<span data-ttu-id="7c96e-105">L’élément **EmptyFolder** définit une demande de vidage d’un dossier dans une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c96e-105">The **EmptyFolder** element defines a request to empty a folder in a mailbox in the Exchange store.</span></span> <span data-ttu-id="7c96e-106">Vous pouvez également supprimer des sous-dossiers lorsque le dossier est vidé.</span><span class="sxs-lookup"><span data-stu-id="7c96e-106">Optionally, subfolders can also be deleted when the folder is emptied.</span></span> 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 <span data-ttu-id="7c96e-107">**EmptyFolderType**</span><span class="sxs-lookup"><span data-stu-id="7c96e-107">**EmptyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c96e-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7c96e-108">Attributes and elements</span></span>

<span data-ttu-id="7c96e-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7c96e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c96e-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="7c96e-110">Attributes</span></span>

|<span data-ttu-id="7c96e-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7c96e-111">**Attribute**</span></span>|<span data-ttu-id="7c96e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7c96e-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7c96e-113">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="7c96e-113">**DeleteType**</span></span> <br/> |<span data-ttu-id="7c96e-114">Spécifie le mode de vidage d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="7c96e-114">Specifies how a folder is emptied.</span></span> <span data-ttu-id="7c96e-115">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="7c96e-115">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="7c96e-116">**DeleteSubFolders**</span><span class="sxs-lookup"><span data-stu-id="7c96e-116">**DeleteSubFolders**</span></span> <br/> |<span data-ttu-id="7c96e-117">Indique si les sous-dossiers doivent être supprimés.</span><span class="sxs-lookup"><span data-stu-id="7c96e-117">Specifies whether subfolders are to be deleted.</span></span> <span data-ttu-id="7c96e-118">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="7c96e-118">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="7c96e-119">Attribut DeleteType</span><span class="sxs-lookup"><span data-stu-id="7c96e-119">DeleteType Attribute</span></span>

|<span data-ttu-id="7c96e-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="7c96e-120">**Value**</span></span>|<span data-ttu-id="7c96e-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="7c96e-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7c96e-122">HardDelete</span><span class="sxs-lookup"><span data-stu-id="7c96e-122">HardDelete</span></span>  <br/> |<span data-ttu-id="7c96e-123">Les messages et les dossiers sont définitivement supprimés de la Banque.</span><span class="sxs-lookup"><span data-stu-id="7c96e-123">A messages and folders are permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="7c96e-124">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="7c96e-124">SoftDelete</span></span>  <br/> |<span data-ttu-id="7c96e-125">Les messages et les dossiers sont déplacés vers la benne si la benne est activée.</span><span class="sxs-lookup"><span data-stu-id="7c96e-125">A messages and folders are moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="7c96e-126">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="7c96e-126">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="7c96e-127">Les messages et les dossiers sont déplacés vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="7c96e-127">A messages and folders are moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7c96e-128">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7c96e-128">Child elements</span></span>

|<span data-ttu-id="7c96e-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7c96e-129">**Element**</span></span>|<span data-ttu-id="7c96e-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="7c96e-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c96e-131">FolderIds</span><span class="sxs-lookup"><span data-stu-id="7c96e-131">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="7c96e-132">Contient un tableau des identificateurs de dossier qui sont utilisés pour identifier les dossiers à supprimer.</span><span class="sxs-lookup"><span data-stu-id="7c96e-132">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c96e-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7c96e-133">Parent elements</span></span>

<span data-ttu-id="7c96e-134">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7c96e-134">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7c96e-135">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7c96e-135">Text value</span></span>

<span data-ttu-id="7c96e-136">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7c96e-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7c96e-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="7c96e-137">Remarks</span></span>

<span data-ttu-id="7c96e-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c96e-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c96e-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7c96e-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c96e-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7c96e-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7c96e-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7c96e-141">Schema Name</span></span>  <br/> |<span data-ttu-id="7c96e-142">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="7c96e-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="7c96e-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7c96e-143">Validation File</span></span>  <br/> |<span data-ttu-id="7c96e-144">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7c96e-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7c96e-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7c96e-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c96e-146">False</span><span class="sxs-lookup"><span data-stu-id="7c96e-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c96e-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7c96e-147">See also</span></span>



[<span data-ttu-id="7c96e-148">Opération EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="7c96e-148">EmptyFolder operation</span></span>](emptyfolder-operation.md)

