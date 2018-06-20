---
title: Élément (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: L’élément représente un seul élément à télécharger dans une boîte aux lettres.
ms.openlocfilehash: 8fecef9a2368a44e38633eb9fddaa8197620f6a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828138"
---
# <a name="item-uploaditemtype"></a><span data-ttu-id="a3ab6-103">Élément (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="a3ab6-103">Item (UploadItemType)</span></span>

<span data-ttu-id="a3ab6-104">**L’élément** représente un seul élément à télécharger dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-104">The **Item** element represents a single item to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="a3ab6-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="a3ab6-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="a3ab6-106">Éléments (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="a3ab6-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
[<span data-ttu-id="a3ab6-107">Élément (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="a3ab6-107">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 <span data-ttu-id="a3ab6-108">**UploadItemType**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-108">**UploadItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3ab6-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a3ab6-109">Attributes and elements</span></span>

<span data-ttu-id="a3ab6-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3ab6-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="a3ab6-111">Attributes</span></span>

|<span data-ttu-id="a3ab6-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-112">**Attribute**</span></span>|<span data-ttu-id="a3ab6-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a3ab6-114">**CreateAction**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-114">**CreateAction**</span></span> <br/> |<span data-ttu-id="a3ab6-115">Spécifie l’action de téléchargement d’un élément dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-115">Specifies the action for uploading an item into a mailbox.</span></span> <span data-ttu-id="a3ab6-116">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="a3ab6-117">**IsAssociated**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-117">**IsAssociated**</span></span> <br/> |<span data-ttu-id="a3ab6-118">Indique si l’élément téléchargé est un élément de dossier associé.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-118">Specifies whether the uploaded item is a folder associated item.</span></span> <span data-ttu-id="a3ab6-119">Cet attribut est une valeur de type Boolean.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-119">This attribute is a Boolean value.</span></span> <span data-ttu-id="a3ab6-120">La valeur **true** indique que l’élément est un dossier associé item.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-120">A value of **true** indicates that the item is a folder associated item.</span></span> <span data-ttu-id="a3ab6-121">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-121">This attribute is optional.</span></span>  <br/> |
   
#### <a name="createaction-attribute"></a><span data-ttu-id="a3ab6-122">Attribut CreateAction</span><span class="sxs-lookup"><span data-stu-id="a3ab6-122">CreateAction Attribute</span></span>

|<span data-ttu-id="a3ab6-123">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-123">**Value**</span></span>|<span data-ttu-id="a3ab6-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a3ab6-125">**CreateNew**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-125">**CreateNew**</span></span> <br/> |<span data-ttu-id="a3ab6-126">Indique qu’une nouvelle copie de l’élément d’origine est téléchargée vers la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-126">Indicates that a new copy of the original item is uploaded to the mailbox.</span></span> <span data-ttu-id="a3ab6-127">L’élément [ItemId](itemid.md) ne doit pas être présent si la valeur CreateNew est utilisée.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-127">The [ItemId](itemid.md) element must not be present if the CreateNew value is used.</span></span> <span data-ttu-id="a3ab6-128">L’identificateur d’élément est retournée dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-128">The new item identifier is returned in the response.</span></span>  <br/> |
|<span data-ttu-id="a3ab6-129">**Mettre à jour**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-129">**Update**</span></span> <br/> |<span data-ttu-id="a3ab6-130">Spécifie que l’élément indiqué par l’élément **ItemId** est mis à jour.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-130">Specifies that the item indicated by the **ItemId** element will be updated.</span></span> <span data-ttu-id="a3ab6-131">Une erreur est renvoyée si l’élément **ItemId** n’est pas présent ou si l’élément n’existe pas dans le dossier identifié par l’élément [ParentFolderId](parentfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="a3ab6-131">An error is returned if the **ItemId** element is not present or if the item does not exist in the folder identified by the [ParentFolderId](parentfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="a3ab6-132">**UpdateOrCreate**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-132">**UpdateOrCreate**</span></span> <br/> |<span data-ttu-id="a3ab6-133">Indique qu’une tentative est tout d’abord à mettre à jour l’élément.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-133">Indicates that an attempt is first made to update the item.</span></span> <span data-ttu-id="a3ab6-134">Si l’élément n’existe pas dans le dossier spécifié par l’élément **ParentFolderId** , un nouvel élément est créé.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-134">If the item does not exist in the folder specified by the **ParentFolderId** element, a new item is created.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a3ab6-135">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a3ab6-135">Child elements</span></span>

|<span data-ttu-id="a3ab6-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-136">**Element**</span></span>|<span data-ttu-id="a3ab6-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3ab6-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="a3ab6-138">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="a3ab6-139">Représente l’identificateur du dossier parent où un nouvel élément est créé ou qui contient l’élément à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-139">Represents the identifier of the parent folder where a new item is created or that contains the item to update.</span></span>  <br/> |
|[<span data-ttu-id="a3ab6-140">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="a3ab6-140">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="a3ab6-141">Contient la clé unique identificateur et modification d’un élément pour créer ou mettre à jour dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-141">Contains the unique identifier and change key of an item to create or update in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a3ab6-142">Données (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="a3ab6-142">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="a3ab6-143">Contient les données d’un seul élément à télécharger dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-143">Contains the data of a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3ab6-144">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a3ab6-144">Parent elements</span></span>

|<span data-ttu-id="a3ab6-145">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-145">**Element**</span></span>|<span data-ttu-id="a3ab6-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="a3ab6-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3ab6-147">Éléments (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="a3ab6-147">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="a3ab6-148">Contient un tableau d’éléments à télécharger dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-148">Contains an array of item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a3ab6-149">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a3ab6-149">Text value</span></span>

<span data-ttu-id="a3ab6-150">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a3ab6-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a3ab6-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="a3ab6-151">Remarks</span></span>

<span data-ttu-id="a3ab6-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a3ab6-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3ab6-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a3ab6-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3ab6-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a3ab6-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a3ab6-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a3ab6-155">Schema Name</span></span>  <br/> |<span data-ttu-id="a3ab6-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a3ab6-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="a3ab6-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a3ab6-157">Validation File</span></span>  <br/> |<span data-ttu-id="a3ab6-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a3ab6-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a3ab6-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a3ab6-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3ab6-160">False</span><span class="sxs-lookup"><span data-stu-id="a3ab6-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3ab6-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a3ab6-161">See also</span></span>



[<span data-ttu-id="a3ab6-162">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="a3ab6-162">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="a3ab6-163">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="a3ab6-163">UploadItems operation</span></span>](uploaditems-operation.md)

