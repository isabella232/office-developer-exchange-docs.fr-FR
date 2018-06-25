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
description: L’élément DeleteFolder définit une demande pour supprimer des dossiers à partir d’une boîte aux lettres dans la banque d’informations Exchange.
ms.openlocfilehash: d31f98f26f537104e40b303de4199f45c65f49c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755862"
---
# <a name="deletefolder"></a><span data-ttu-id="c4809-103">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="c4809-103">DeleteFolder</span></span>

<span data-ttu-id="c4809-104">L’élément **DeleteFolder** définit une demande pour supprimer des dossiers à partir d’une boîte aux lettres dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4809-104">The **DeleteFolder** element defines a request to delete folders from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 <span data-ttu-id="c4809-105">**DeleteFolderType**</span><span class="sxs-lookup"><span data-stu-id="c4809-105">**DeleteFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4809-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c4809-106">Attributes and elements</span></span>

<span data-ttu-id="c4809-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c4809-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4809-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c4809-108">Attributes</span></span>

|<span data-ttu-id="c4809-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="c4809-109">**Attribute**</span></span>|<span data-ttu-id="c4809-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="c4809-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c4809-111">**DeleType**</span><span class="sxs-lookup"><span data-stu-id="c4809-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="c4809-112">Décrit comment un dossier est supprimé.</span><span class="sxs-lookup"><span data-stu-id="c4809-112">Describes how a folder is deleted.</span></span> <span data-ttu-id="c4809-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="c4809-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="c4809-114">Attribut DeleType</span><span class="sxs-lookup"><span data-stu-id="c4809-114">DeleteType attribute</span></span>

|<span data-ttu-id="c4809-115">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="c4809-115">**Value**</span></span>|<span data-ttu-id="c4809-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="c4809-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c4809-117">HardDelete</span><span class="sxs-lookup"><span data-stu-id="c4809-117">HardDelete</span></span>  <br/> |<span data-ttu-id="c4809-118">Un dossier est définitivement supprimé de la banque.</span><span class="sxs-lookup"><span data-stu-id="c4809-118">A folder is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="c4809-119">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="c4809-119">SoftDelete</span></span>  <br/> |<span data-ttu-id="c4809-120">Un dossier est déplacé vers la benne si la benne est activé.</span><span class="sxs-lookup"><span data-stu-id="c4809-120">A folder is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="c4809-121">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="c4809-121">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="c4809-122">Un dossier est déplacé vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="c4809-122">A folder is moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c4809-123">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c4809-123">Child elements</span></span>

|<span data-ttu-id="c4809-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c4809-124">**Element**</span></span>|<span data-ttu-id="c4809-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="c4809-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4809-126">FolderIds</span><span class="sxs-lookup"><span data-stu-id="c4809-126">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="c4809-127">Contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers à supprimer.</span><span class="sxs-lookup"><span data-stu-id="c4809-127">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c4809-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c4809-128">Parent elements</span></span>

<span data-ttu-id="c4809-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c4809-129">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c4809-130">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c4809-130">Text value</span></span>

<span data-ttu-id="c4809-131">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c4809-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c4809-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="c4809-132">Remarks</span></span>

<span data-ttu-id="c4809-133">Les options **MoveToDeletedItems** et **HardDelete** sont transactionnelles, ce qui signifie qu’au moment où un appel au service Web est terminée, la base de données a déplacé l’élément vers le dossier éléments supprimés ou définitivement supprimé l’élément de la base de données Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4809-133">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="c4809-134">Ce comportement est la même valeur MicrosoftExchange Server 2007 et Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="c4809-134">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="c4809-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4809-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4809-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c4809-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4809-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c4809-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c4809-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c4809-138">Schema Name</span></span>  <br/> |<span data-ttu-id="c4809-139">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="c4809-139">Message schema</span></span>  <br/> |
|<span data-ttu-id="c4809-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c4809-140">Validation File</span></span>  <br/> |<span data-ttu-id="c4809-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c4809-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c4809-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c4809-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="c4809-143">False</span><span class="sxs-lookup"><span data-stu-id="c4809-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4809-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c4809-144">See also</span></span>

- [<span data-ttu-id="c4809-145">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="c4809-145">DeleteFolder operation</span></span>](deletefolder-operation.md)

