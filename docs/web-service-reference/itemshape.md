---
title: ItemShape
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemShape
api_type:
- schema
ms.assetid: c5604161-bbc0-40bc-ad75-ff7e837d745f
description: L’élément ItemShape identifie un ensemble de propriétés à retourner dans une opération GetItem, FindItem opération ou une réponse d’opération SyncFolderItems.
ms.openlocfilehash: 95174a85a8fa05cb2612e1289d46c8db32b6e052
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828191"
---
# <a name="itemshape"></a><span data-ttu-id="a42c5-103">ItemShape</span><span class="sxs-lookup"><span data-stu-id="a42c5-103">ItemShape</span></span>

<span data-ttu-id="a42c5-104">L’élément **ItemShape** identifie un ensemble de propriétés à retourner dans une réponse [GetItem operation](getitem-operation.md), [opération FindItem](finditem-operation.md)ou [SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a42c5-104">The **ItemShape** element identifies a set of properties to return in a [GetItem operation](getitem-operation.md), [FindItem operation](finditem-operation.md), or [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> 
  
```XML
<ItemShape>
   <BaseShape/>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <ConvertHtmlCodePageToUTF8/>
   <AdditionalProperties/>
</ItemShape>
```

 <span data-ttu-id="a42c5-105">**ItemResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="a42c5-105">**ItemResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a42c5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a42c5-106">Attributes and elements</span></span>

<span data-ttu-id="a42c5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a42c5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a42c5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a42c5-108">Attributes</span></span>

<span data-ttu-id="a42c5-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a42c5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a42c5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a42c5-110">Child elements</span></span>

|<span data-ttu-id="a42c5-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a42c5-111">**Element**</span></span>|<span data-ttu-id="a42c5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a42c5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a42c5-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="a42c5-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="a42c5-114">Identifie la configuration de propriétés à retourner dans une réponse de l’élément ou le dossier de base.</span><span class="sxs-lookup"><span data-stu-id="a42c5-114">Identifies the basic configuration of properties to return in an item or folder response.</span></span>  <br/> |
|[<span data-ttu-id="a42c5-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="a42c5-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="a42c5-116">Spécifie si le contenu Multipurpose Internet Mail Extensions (MIME) d’un élément est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="a42c5-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item is returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="a42c5-117">BodyType</span><span class="sxs-lookup"><span data-stu-id="a42c5-117">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="a42c5-118">Identifie la mise en forme le corps du texte dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="a42c5-118">Identifies how the body text is formatted in the response.</span></span>  <br/> |
|[<span data-ttu-id="a42c5-119">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="a42c5-119">ConvertHtmlCodePageToUTF8</span></span>](converthtmlcodepagetoutf8.md) <br/> |<span data-ttu-id="a42c5-120">Indique si l’élément corps HTML est converti en UTF-8.</span><span class="sxs-lookup"><span data-stu-id="a42c5-120">Indicates whether the item HTML body is converted to UTF8.</span></span>  <br/> |
|[<span data-ttu-id="a42c5-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="a42c5-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="a42c5-122">Spécifie si le filtrage du contenu HTML est activé.</span><span class="sxs-lookup"><span data-stu-id="a42c5-122">Specifies whether HTML content filtering is enabled.</span></span>  <br/> |
|[<span data-ttu-id="a42c5-123">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="a42c5-123">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="a42c5-124">Identifie les propriétés supplémentaires pour retourner une réponse.</span><span class="sxs-lookup"><span data-stu-id="a42c5-124">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a42c5-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a42c5-125">Parent elements</span></span>

|<span data-ttu-id="a42c5-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a42c5-126">**Element**</span></span>|<span data-ttu-id="a42c5-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="a42c5-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a42c5-128">GetItem</span><span class="sxs-lookup"><span data-stu-id="a42c5-128">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="a42c5-129">Définit une requête pour récupérer des éléments à partir d’une boîte aux lettres dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a42c5-129">Defines a request to retrieve items from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="a42c5-130">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="a42c5-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="a42c5-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="a42c5-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="a42c5-132">Définit une requête pour rechercher tous les éléments contenus dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="a42c5-132">Defines a request to find all items that are contained in a folder.</span></span>  <br/> <span data-ttu-id="a42c5-133">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="a42c5-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="a42c5-134">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="a42c5-134">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="a42c5-135">Définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="a42c5-135">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="a42c5-136">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="a42c5-136">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a42c5-137">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a42c5-137">Text value</span></span>

<span data-ttu-id="a42c5-138">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a42c5-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a42c5-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="a42c5-139">Remarks</span></span>

<span data-ttu-id="a42c5-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a42c5-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a42c5-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a42c5-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a42c5-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a42c5-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a42c5-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a42c5-143">Schema Name</span></span>  <br/> |<span data-ttu-id="a42c5-144">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a42c5-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a42c5-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a42c5-145">Validation File</span></span>  <br/> |<span data-ttu-id="a42c5-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a42c5-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a42c5-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a42c5-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="a42c5-148">False</span><span class="sxs-lookup"><span data-stu-id="a42c5-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a42c5-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a42c5-149">See also</span></span>



[<span data-ttu-id="a42c5-150">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="a42c5-150">GetItem operation</span></span>](getitem-operation.md)
  
[<span data-ttu-id="a42c5-151">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="a42c5-151">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="a42c5-152">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="a42c5-152">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="a42c5-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a42c5-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

