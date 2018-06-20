---
title: AttachmentShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentShape
api_type:
- schema
ms.assetid: 734914b5-3a16-4744-90a5-741fd30c4676
description: L’élément AttachmentShape identifie des propriétés supplémentaires pour retourner une réponse à une demande GetAttachment.
ms.openlocfilehash: dc6769faa5fd28ce31b796f86c507aec54abff7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755339"
---
# <a name="attachmentshape"></a><span data-ttu-id="5fec6-103">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="5fec6-103">AttachmentShape</span></span>

<span data-ttu-id="5fec6-104">L’élément **AttachmentShape** identifie des propriétés supplémentaires pour retourner une réponse à une demande [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="5fec6-104">The **AttachmentShape** element identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> 
  
- [<span data-ttu-id="5fec6-105">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="5fec6-105">GetAttachment</span></span>](getattachment.md)
  
- [<span data-ttu-id="5fec6-106">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="5fec6-106">AttachmentShape</span></span>](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 <span data-ttu-id="5fec6-107">**AttachmentResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="5fec6-107">**AttachmentResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5fec6-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5fec6-108">Attributes and elements</span></span>

<span data-ttu-id="5fec6-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5fec6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5fec6-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="5fec6-110">Attributes</span></span>

<span data-ttu-id="5fec6-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5fec6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5fec6-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5fec6-112">Child elements</span></span>

|<span data-ttu-id="5fec6-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5fec6-113">**Element**</span></span>|<span data-ttu-id="5fec6-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5fec6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fec6-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="5fec6-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="5fec6-116">Spécifie si le contenu Multipurpose Internet Mail Extensions (MIME) d’un élément ou d’une pièce jointe est retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="5fec6-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> <span data-ttu-id="5fec6-117">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="5fec6-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="5fec6-118">BodyType</span><span class="sxs-lookup"><span data-stu-id="5fec6-118">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="5fec6-119">Identifie la mise en forme le corps du texte dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="5fec6-119">Identifies how the body text is formatted in the response.</span></span> <span data-ttu-id="5fec6-120">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="5fec6-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="5fec6-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="5fec6-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="5fec6-122">Spécifie si le contenu HTML potentiellement dangereux est filtré à partir d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="5fec6-122">Specifies whether potentially unsafe HTML content is filtered from an attachment.</span></span> <span data-ttu-id="5fec6-123">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="5fec6-123">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="5fec6-124">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="5fec6-124">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="5fec6-125">Identifie les propriétés supplémentaires pour retourner une réponse.</span><span class="sxs-lookup"><span data-stu-id="5fec6-125">Identifies additional properties to return in a response.</span></span> <span data-ttu-id="5fec6-126">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="5fec6-126">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5fec6-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5fec6-127">Parent elements</span></span>

|<span data-ttu-id="5fec6-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5fec6-128">**Element**</span></span>|<span data-ttu-id="5fec6-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="5fec6-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fec6-130">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="5fec6-130">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="5fec6-131">L’élément qui définit une demande pour obtenir une pièce jointe à partir d’une boîte aux lettres dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5fec6-131">The element that defines a request to get an attachment from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="5fec6-132">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="5fec6-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5fec6-133">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5fec6-133">Text value</span></span>

<span data-ttu-id="5fec6-134">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5fec6-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5fec6-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="5fec6-135">Remarks</span></span>

<span data-ttu-id="5fec6-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5fec6-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5fec6-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5fec6-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5fec6-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5fec6-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5fec6-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5fec6-139">Schema Name</span></span>  <br/> |<span data-ttu-id="5fec6-140">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="5fec6-140">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5fec6-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5fec6-141">Validation File</span></span>  <br/> |<span data-ttu-id="5fec6-142">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5fec6-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5fec6-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5fec6-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="5fec6-144">False</span><span class="sxs-lookup"><span data-stu-id="5fec6-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5fec6-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5fec6-145">See also</span></span>

- [<span data-ttu-id="5fec6-146">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="5fec6-146">GetAttachment operation</span></span>](getattachment-operation.md)
- [<span data-ttu-id="5fec6-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5fec6-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

