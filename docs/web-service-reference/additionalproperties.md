---
title: AdditionalProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdditionalProperties
api_type:
- schema
ms.assetid: 7a269aed-dcfd-4c3e-9e14-094e53828101
description: L’élément AdditionalProperties identifie des propriétés supplémentaires pour l’utilisation de GetItem, UpdateItem, CreateItem, FindItem ou Demandes FindFolder.
ms.openlocfilehash: 64e4f1ee6b24cf8015b7893dc4a904ca8b32d58e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755172"
---
# <a name="additionalproperties"></a><span data-ttu-id="b1d3e-103">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="b1d3e-103">AdditionalProperties</span></span>

<span data-ttu-id="b1d3e-104">L’élément **AdditionalProperties** identifie des propriétés supplémentaires pour l’utilisation de [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)ou demandes [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="b1d3e-104">The **AdditionalProperties** element identifies additional properties for use in [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 <span data-ttu-id="b1d3e-105">**NonEmptyArrayOfPathsToElementType**</span><span class="sxs-lookup"><span data-stu-id="b1d3e-105">**NonEmptyArrayOfPathsToElementType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1d3e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b1d3e-106">Attributes and elements</span></span>

<span data-ttu-id="b1d3e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b1d3e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1d3e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b1d3e-108">Attributes</span></span>

<span data-ttu-id="b1d3e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b1d3e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b1d3e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b1d3e-110">Child elements</span></span>

|<span data-ttu-id="b1d3e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b1d3e-111">**Element**</span></span>|<span data-ttu-id="b1d3e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b1d3e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1d3e-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b1d3e-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="b1d3e-114">Identifie les propriétés MAPI étendues pour obtenir, définir ou créer.</span><span class="sxs-lookup"><span data-stu-id="b1d3e-114">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="b1d3e-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="b1d3e-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="b1d3e-116">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="b1d3e-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="b1d3e-117">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b1d3e-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="b1d3e-118">Identifie les propriétés du dictionnaire fréquemment référencées par URI.</span><span class="sxs-lookup"><span data-stu-id="b1d3e-118">Identifies frequently referenced dictionary properties by URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b1d3e-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b1d3e-119">Parent elements</span></span>

|<span data-ttu-id="b1d3e-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b1d3e-120">**Element**</span></span>|<span data-ttu-id="b1d3e-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="b1d3e-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1d3e-122">FolderShape</span><span class="sxs-lookup"><span data-stu-id="b1d3e-122">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="b1d3e-123">Identifie les propriétés du dossier à inclure dans une réponse [GetFolder](getfolder.md), [FindFolder](findfolder.md)ou [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="b1d3e-123">Identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span><br/><br/>  <span data-ttu-id="b1d3e-124">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="b1d3e-124">The following are the XPath expressions to this element:</span></span><br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="b1d3e-125">ItemShape</span><span class="sxs-lookup"><span data-stu-id="b1d3e-125">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="b1d3e-126">Identifie les propriétés de l’élément et le contenu à inclure dans une réponse [GetItem](getitem.md), [FindItem](finditem.md)ou [SyncFolderItems](syncfolderitems.md) .</span><span class="sxs-lookup"><span data-stu-id="b1d3e-126">Identifies the item properties and content to include in a [GetItem](getitem.md), [FindItem](finditem.md), or [SyncFolderItems](syncfolderitems.md) response.</span></span><br/><br/>  <span data-ttu-id="b1d3e-127">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="b1d3e-127">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="b1d3e-128">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="b1d3e-128">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="b1d3e-129">Identifie les propriétés totale de l’article à renvoyer dans une réponse à une demande de [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="b1d3e-129">Identifies additional extended item properties to return in a response to a [GetItem](getitem.md) request.</span></span><br/><br/> <span data-ttu-id="b1d3e-130">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="b1d3e-130">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b1d3e-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="b1d3e-131">Remarks</span></span>

<span data-ttu-id="b1d3e-132">Pas tous les éléments enfants peuvent être utilisés avec [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)ou demandes [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="b1d3e-132">Not all the child elements can be used with [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> <span data-ttu-id="b1d3e-133">La propriété doit être applicable dans le dossier ou l’élément est accessible.</span><span class="sxs-lookup"><span data-stu-id="b1d3e-133">The property must be applicable to the folder or item that is accessed.</span></span> <span data-ttu-id="b1d3e-134">Utilisez les propriétés étendues pour accéder aux autres propriétés.</span><span class="sxs-lookup"><span data-stu-id="b1d3e-134">Use extended properties to access other properties.</span></span> <span data-ttu-id="b1d3e-135">Si la propriété n’existe pas pour un élément donné, aucun élément correspondant ne sera émis dans le code XML qui en résulte.</span><span class="sxs-lookup"><span data-stu-id="b1d3e-135">If the property does not exist for a given item, no corresponding element will be emitted into the resulting XML.</span></span> 
  
<span data-ttu-id="b1d3e-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b1d3e-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="b1d3e-137">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="b1d3e-137">This element is optional.</span></span>
  
## <a name="example"></a><span data-ttu-id="b1d3e-138">Exemple</span><span class="sxs-lookup"><span data-stu-id="b1d3e-138">Example</span></span>

<span data-ttu-id="b1d3e-139">L’exemple de requête suivant montre comment obtenir un objet de l’élément à l’aide de l’élément **AdditionalProperties** .</span><span class="sxs-lookup"><span data-stu-id="b1d3e-139">The following request example shows how to get an item subject by using the **AdditionalProperties** element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="ASkAS="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="b1d3e-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b1d3e-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1d3e-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b1d3e-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b1d3e-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b1d3e-142">Schema Name</span></span>  <br/> |<span data-ttu-id="b1d3e-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b1d3e-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="b1d3e-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b1d3e-144">Validation File</span></span>  <br/> |<span data-ttu-id="b1d3e-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b1d3e-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b1d3e-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b1d3e-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="b1d3e-147">False</span><span class="sxs-lookup"><span data-stu-id="b1d3e-147">False</span></span>  <br/> |
   

