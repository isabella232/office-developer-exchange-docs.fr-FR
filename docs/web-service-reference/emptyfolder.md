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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457276"
---
# <a name="emptyfolder"></a><span data-ttu-id="7d9b4-104">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="7d9b4-104">EmptyFolder</span></span>

<span data-ttu-id="7d9b4-105">L’élément **EmptyFolder** définit une demande de vidage d’un dossier dans une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-105">The **EmptyFolder** element defines a request to empty a folder in a mailbox in the Exchange store.</span></span> <span data-ttu-id="7d9b4-106">Vous pouvez également supprimer des sous-dossiers lorsque le dossier est vidé.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-106">Optionally, subfolders can also be deleted when the folder is emptied.</span></span> 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 <span data-ttu-id="7d9b4-107">**EmptyFolderType**</span><span class="sxs-lookup"><span data-stu-id="7d9b4-107">**EmptyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d9b4-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7d9b4-108">Attributes and elements</span></span>

<span data-ttu-id="7d9b4-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d9b4-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="7d9b4-110">Attributes</span></span>

|<span data-ttu-id="7d9b4-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7d9b4-111">**Attribute**</span></span>|<span data-ttu-id="7d9b4-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7d9b4-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7d9b4-113">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="7d9b4-113">**DeleteType**</span></span> <br/> |<span data-ttu-id="7d9b4-114">Spécifie le mode de vidage d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-114">Specifies how a folder is emptied.</span></span> <span data-ttu-id="7d9b4-115">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-115">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="7d9b4-116">**DeleteSubFolders**</span><span class="sxs-lookup"><span data-stu-id="7d9b4-116">**DeleteSubFolders**</span></span> <br/> |<span data-ttu-id="7d9b4-117">Indique si les sous-dossiers doivent être supprimés.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-117">Specifies whether subfolders are to be deleted.</span></span> <span data-ttu-id="7d9b4-118">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-118">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="7d9b4-119">Attribut DeleteType</span><span class="sxs-lookup"><span data-stu-id="7d9b4-119">DeleteType Attribute</span></span>

|<span data-ttu-id="7d9b4-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="7d9b4-120">**Value**</span></span>|<span data-ttu-id="7d9b4-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="7d9b4-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7d9b4-122">HardDelete</span><span class="sxs-lookup"><span data-stu-id="7d9b4-122">HardDelete</span></span>  <br/> |<span data-ttu-id="7d9b4-123">Les messages et les dossiers sont définitivement supprimés de la Banque.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-123">A messages and folders are permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="7d9b4-124">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="7d9b4-124">SoftDelete</span></span>  <br/> |<span data-ttu-id="7d9b4-125">Les messages et les dossiers sont déplacés vers la benne si la benne est activée.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-125">A messages and folders are moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="7d9b4-126">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="7d9b4-126">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="7d9b4-127">Les messages et les dossiers sont déplacés vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-127">A messages and folders are moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7d9b4-128">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7d9b4-128">Child elements</span></span>

|<span data-ttu-id="7d9b4-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7d9b4-129">**Element**</span></span>|<span data-ttu-id="7d9b4-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="7d9b4-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d9b4-131">FolderIds</span><span class="sxs-lookup"><span data-stu-id="7d9b4-131">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="7d9b4-132">Contient un tableau des identificateurs de dossier qui sont utilisés pour identifier les dossiers à supprimer.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-132">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7d9b4-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7d9b4-133">Parent elements</span></span>

<span data-ttu-id="7d9b4-134">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-134">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7d9b4-135">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7d9b4-135">Text value</span></span>

<span data-ttu-id="7d9b4-136">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7d9b4-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="7d9b4-137">Remarks</span></span>

<span data-ttu-id="7d9b4-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d9b4-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d9b4-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7d9b4-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d9b4-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7d9b4-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7d9b4-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7d9b4-141">Schema Name</span></span>  <br/> |<span data-ttu-id="7d9b4-142">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="7d9b4-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="7d9b4-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7d9b4-143">Validation File</span></span>  <br/> |<span data-ttu-id="7d9b4-144">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7d9b4-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d9b4-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7d9b4-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d9b4-146">False</span><span class="sxs-lookup"><span data-stu-id="7d9b4-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d9b4-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7d9b4-147">See also</span></span>



[<span data-ttu-id="7d9b4-148">Opération EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="7d9b4-148">EmptyFolder operation</span></span>](emptyfolder-operation.md)

