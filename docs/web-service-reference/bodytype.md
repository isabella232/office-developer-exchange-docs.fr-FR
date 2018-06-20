---
title: BodyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BodyType
api_type:
- schema
ms.assetid: d42ec77b-fb9f-404a-9bf2-1801e8744676
description: L’élément BodyType identifie la mise en forme le corps du texte dans la réponse.
ms.openlocfilehash: f8be2e96390b40faa367cf0d34c533accc3b8afb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755421"
---
# <a name="bodytype"></a><span data-ttu-id="9c66f-103">BodyType</span><span class="sxs-lookup"><span data-stu-id="9c66f-103">BodyType</span></span>

<span data-ttu-id="9c66f-104">L’élément **BodyType** identifie la mise en forme le corps du texte dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="9c66f-104">The **BodyType** element identifies how the body text is formatted in the response.</span></span> 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

<span data-ttu-id="9c66f-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="9c66f-105">**BodyTypeResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9c66f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9c66f-106">Attributes and elements</span></span>

<span data-ttu-id="9c66f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9c66f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c66f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9c66f-108">Attributes</span></span>

<span data-ttu-id="9c66f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9c66f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c66f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9c66f-110">Child elements</span></span>

<span data-ttu-id="9c66f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9c66f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9c66f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9c66f-112">Parent elements</span></span>

|<span data-ttu-id="9c66f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9c66f-113">**Element**</span></span>|<span data-ttu-id="9c66f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9c66f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c66f-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="9c66f-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="9c66f-116">Identifie les propriétés de l’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="9c66f-116">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/><br/><span data-ttu-id="9c66f-117">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="9c66f-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="9c66f-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="9c66f-118">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="9c66f-119">Identifie les propriétés totale de l’article à renvoyer dans une réponse à une demande [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="9c66f-119">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/><span data-ttu-id="9c66f-120">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="9c66f-120">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9c66f-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9c66f-121">Text value</span></span>

<span data-ttu-id="9c66f-122">Le tableau suivant répertorie les valeurs possibles pour l’élément **BodyType** .</span><span class="sxs-lookup"><span data-stu-id="9c66f-122">The following table lists the possible values for the **BodyType** element.</span></span> 
  
|<span data-ttu-id="9c66f-123">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="9c66f-123">**Value**</span></span>|<span data-ttu-id="9c66f-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="9c66f-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9c66f-125">Recommandé</span><span class="sxs-lookup"><span data-stu-id="9c66f-125">Best</span></span>  <br/> |<span data-ttu-id="9c66f-126">La réponse renvoie le contenu disponible plus riche du corps de texte.</span><span class="sxs-lookup"><span data-stu-id="9c66f-126">The response will return the richest available content of body text.</span></span> <span data-ttu-id="9c66f-127">Cela est utile si elle est inconnue ou non le contenu est texte ou HTML.</span><span class="sxs-lookup"><span data-stu-id="9c66f-127">This is useful if it is unknown whether the content is text or HTML.</span></span><br/><br/> <span data-ttu-id="9c66f-128">Le corps retourné sera texte si le corps stocké est en texte brut.</span><span class="sxs-lookup"><span data-stu-id="9c66f-128">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="9c66f-129">Dans le cas contraire, la réponse renverra HTML si le corps stocké est au format HTML ou RTF.</span><span class="sxs-lookup"><span data-stu-id="9c66f-129">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span><br/><br/> <span data-ttu-id="9c66f-130">Il s'agit de la valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="9c66f-130">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="9c66f-131">HTML</span><span class="sxs-lookup"><span data-stu-id="9c66f-131">HTML</span></span>  <br/> |<span data-ttu-id="9c66f-132">La réponse renvoie un corps de l’élément au format HTML.</span><span class="sxs-lookup"><span data-stu-id="9c66f-132">The response will return an item body as HTML.</span></span>  <br/> |
|<span data-ttu-id="9c66f-133">Texte</span><span class="sxs-lookup"><span data-stu-id="9c66f-133">Text</span></span>  <br/> |<span data-ttu-id="9c66f-134">La réponse renvoie un corps de l’élément en tant que texte brut.</span><span class="sxs-lookup"><span data-stu-id="9c66f-134">The response will return an item body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9c66f-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="9c66f-135">Remarks</span></span>

<span data-ttu-id="9c66f-136">Vous pouvez identifier le type de corps retourné dans la réponse en vérifiant l’attribut **BodyType** de l’élément [Body](body.md) .</span><span class="sxs-lookup"><span data-stu-id="9c66f-136">You can identify the type of body returned in the response by checking the **BodyType** attribute of the [Body](body.md) element.</span></span> <span data-ttu-id="9c66f-137">L’attribut **BodyType** identifie le corps HTML ou texte.</span><span class="sxs-lookup"><span data-stu-id="9c66f-137">The **BodyType** attribute will identify the body as either HTML or text.</span></span> 
  
<span data-ttu-id="9c66f-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9c66f-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="9c66f-139">Exemple</span><span class="sxs-lookup"><span data-stu-id="9c66f-139">Example</span></span>

<span data-ttu-id="9c66f-140">L’exemple suivant d’une demande montre où un élément **BodyType** est utilisé.</span><span class="sxs-lookup"><span data-stu-id="9c66f-140">The following example of a request shows where a **BodyType** element is used.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="9c66f-141">L’attribut Id a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="9c66f-141">The Id attribute has been shortened to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c66f-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9c66f-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c66f-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9c66f-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c66f-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9c66f-144">Schema Name</span></span>  <br/> |<span data-ttu-id="9c66f-145">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9c66f-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c66f-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9c66f-146">Validation File</span></span>  <br/> |<span data-ttu-id="9c66f-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9c66f-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c66f-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9c66f-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c66f-149">False</span><span class="sxs-lookup"><span data-stu-id="9c66f-149">False</span></span>  <br/> |
   

