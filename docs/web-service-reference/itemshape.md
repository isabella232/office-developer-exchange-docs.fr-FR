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
description: L’élément ItemShape identifie un jeu de propriétés à renvoyer dans une opération GetItem, FindItem ou SyncFolderItems.
ms.openlocfilehash: ffb666ee331b55a4f04cad076c705e4bec980e03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458123"
---
# <a name="itemshape"></a><span data-ttu-id="887e2-103">ItemShape</span><span class="sxs-lookup"><span data-stu-id="887e2-103">ItemShape</span></span>

<span data-ttu-id="887e2-104">L’élément **ItemShape** identifie un jeu de propriétés à renvoyer dans une [opération GetItem](getitem-operation.md), [FindItem](finditem-operation.md)ou [SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="887e2-104">The **ItemShape** element identifies a set of properties to return in a [GetItem operation](getitem-operation.md), [FindItem operation](finditem-operation.md), or [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> 
  
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

 <span data-ttu-id="887e2-105">**ItemResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="887e2-105">**ItemResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="887e2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="887e2-106">Attributes and elements</span></span>

<span data-ttu-id="887e2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="887e2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="887e2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="887e2-108">Attributes</span></span>

<span data-ttu-id="887e2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="887e2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="887e2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="887e2-110">Child elements</span></span>

|<span data-ttu-id="887e2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="887e2-111">**Element**</span></span>|<span data-ttu-id="887e2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="887e2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="887e2-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="887e2-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="887e2-114">Identifie la configuration de base des propriétés à renvoyer dans une réponse d’un élément ou d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="887e2-114">Identifies the basic configuration of properties to return in an item or folder response.</span></span>  <br/> |
|[<span data-ttu-id="887e2-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="887e2-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="887e2-116">Indique si le contenu MIME (Multipurpose Internet Mail Extensions) d’un élément est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="887e2-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item is returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="887e2-117">BodyType</span><span class="sxs-lookup"><span data-stu-id="887e2-117">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="887e2-118">Identifie la façon dont le corps de texte est mis en forme dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="887e2-118">Identifies how the body text is formatted in the response.</span></span>  <br/> |
|[<span data-ttu-id="887e2-119">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="887e2-119">ConvertHtmlCodePageToUTF8</span></span>](converthtmlcodepagetoutf8.md) <br/> |<span data-ttu-id="887e2-120">Indique si le corps HTML de l’élément est converti en UTF8.</span><span class="sxs-lookup"><span data-stu-id="887e2-120">Indicates whether the item HTML body is converted to UTF8.</span></span>  <br/> |
|[<span data-ttu-id="887e2-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="887e2-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="887e2-122">Indique si le filtrage du contenu HTML est activé.</span><span class="sxs-lookup"><span data-stu-id="887e2-122">Specifies whether HTML content filtering is enabled.</span></span>  <br/> |
|[<span data-ttu-id="887e2-123">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="887e2-123">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="887e2-124">Identifie les propriétés supplémentaires à renvoyer dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="887e2-124">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="887e2-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="887e2-125">Parent elements</span></span>

|<span data-ttu-id="887e2-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="887e2-126">**Element**</span></span>|<span data-ttu-id="887e2-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="887e2-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="887e2-128">GetItem</span><span class="sxs-lookup"><span data-stu-id="887e2-128">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="887e2-129">Définit une demande de récupération des éléments d’une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="887e2-129">Defines a request to retrieve items from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="887e2-130">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="887e2-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="887e2-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="887e2-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="887e2-132">Définit une requête pour rechercher tous les éléments contenus dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="887e2-132">Defines a request to find all items that are contained in a folder.</span></span>  <br/> <span data-ttu-id="887e2-133">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="887e2-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="887e2-134">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="887e2-134">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="887e2-135">Définit une demande de synchronisation des éléments dans un dossier de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="887e2-135">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="887e2-136">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="887e2-136">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="887e2-137">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="887e2-137">Text value</span></span>

<span data-ttu-id="887e2-138">Aucun.</span><span class="sxs-lookup"><span data-stu-id="887e2-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="887e2-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="887e2-139">Remarks</span></span>

<span data-ttu-id="887e2-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="887e2-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="887e2-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="887e2-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="887e2-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="887e2-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="887e2-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="887e2-143">Schema Name</span></span>  <br/> |<span data-ttu-id="887e2-144">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="887e2-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="887e2-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="887e2-145">Validation File</span></span>  <br/> |<span data-ttu-id="887e2-146">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="887e2-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="887e2-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="887e2-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="887e2-148">False</span><span class="sxs-lookup"><span data-stu-id="887e2-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="887e2-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="887e2-149">See also</span></span>



[<span data-ttu-id="887e2-150">Opération GetItem</span><span class="sxs-lookup"><span data-stu-id="887e2-150">GetItem operation</span></span>](getitem-operation.md)
  
[<span data-ttu-id="887e2-151">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="887e2-151">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="887e2-152">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="887e2-152">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="887e2-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="887e2-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

