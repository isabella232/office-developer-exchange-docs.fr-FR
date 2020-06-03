---
title: DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: e37963f4-af9e-4481-b389-16175711e66d
description: L’élément DeleteFolder définit une demande de suppression de dossiers d’une boîte aux lettres dans la Banque d’Exchange.
ms.openlocfilehash: eb705a47b78b19c79b2e87561ba3696ed40e09cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458767"
---
# <a name="deletefolder"></a><span data-ttu-id="385c4-103">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="385c4-103">DeleteFolder</span></span>

<span data-ttu-id="385c4-104">L’élément **DeleteFolder** définit une demande de suppression de dossiers d’une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="385c4-104">The **DeleteFolder** element defines a request to delete folders from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 <span data-ttu-id="385c4-105">**DeleteFolderType**</span><span class="sxs-lookup"><span data-stu-id="385c4-105">**DeleteFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="385c4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="385c4-106">Attributes and elements</span></span>

<span data-ttu-id="385c4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="385c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="385c4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="385c4-108">Attributes</span></span>

|<span data-ttu-id="385c4-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="385c4-109">**Attribute**</span></span>|<span data-ttu-id="385c4-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="385c4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="385c4-111">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="385c4-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="385c4-112">Décrit le mode de suppression d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="385c4-112">Describes how a folder is deleted.</span></span> <span data-ttu-id="385c4-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="385c4-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="385c4-114">Attribut DeleteType</span><span class="sxs-lookup"><span data-stu-id="385c4-114">DeleteType attribute</span></span>

|<span data-ttu-id="385c4-115">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="385c4-115">**Value**</span></span>|<span data-ttu-id="385c4-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="385c4-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="385c4-117">HardDelete</span><span class="sxs-lookup"><span data-stu-id="385c4-117">HardDelete</span></span>  <br/> |<span data-ttu-id="385c4-118">Un dossier est définitivement supprimé de la Banque.</span><span class="sxs-lookup"><span data-stu-id="385c4-118">A folder is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="385c4-119">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="385c4-119">SoftDelete</span></span>  <br/> |<span data-ttu-id="385c4-120">Un dossier est déplacé vers la benne si la benne est activée.</span><span class="sxs-lookup"><span data-stu-id="385c4-120">A folder is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="385c4-121">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="385c4-121">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="385c4-122">Un dossier est déplacé vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="385c4-122">A folder is moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="385c4-123">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="385c4-123">Child elements</span></span>

|<span data-ttu-id="385c4-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="385c4-124">**Element**</span></span>|<span data-ttu-id="385c4-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="385c4-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="385c4-126">FolderIds</span><span class="sxs-lookup"><span data-stu-id="385c4-126">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="385c4-127">Contient un tableau des identificateurs de dossier qui sont utilisés pour identifier les dossiers à supprimer.</span><span class="sxs-lookup"><span data-stu-id="385c4-127">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="385c4-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="385c4-128">Parent elements</span></span>

<span data-ttu-id="385c4-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="385c4-129">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="385c4-130">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="385c4-130">Text value</span></span>

<span data-ttu-id="385c4-131">Aucun.</span><span class="sxs-lookup"><span data-stu-id="385c4-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="385c4-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="385c4-132">Remarks</span></span>

<span data-ttu-id="385c4-133">Les options **MoveToDeletedItems** et **HardDelete** sont transactionnelles, ce qui signifie qu’au moment de la fin d’un appel de service Web, la base de données a déplacé l’élément dans le dossier éléments supprimés ou a définitivement supprimé l’élément de la base de données Exchange.</span><span class="sxs-lookup"><span data-stu-id="385c4-133">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="385c4-134">Ce comportement est le même pour MicrosoftExchange Server 2007 et Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="385c4-134">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="385c4-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="385c4-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="385c4-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="385c4-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="385c4-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="385c4-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="385c4-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="385c4-138">Schema Name</span></span>  <br/> |<span data-ttu-id="385c4-139">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="385c4-139">Message schema</span></span>  <br/> |
|<span data-ttu-id="385c4-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="385c4-140">Validation File</span></span>  <br/> |<span data-ttu-id="385c4-141">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="385c4-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="385c4-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="385c4-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="385c4-143">False</span><span class="sxs-lookup"><span data-stu-id="385c4-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="385c4-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="385c4-144">See also</span></span>

- [<span data-ttu-id="385c4-145">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="385c4-145">DeleteFolder operation</span></span>](deletefolder-operation.md)

