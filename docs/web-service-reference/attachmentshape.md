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
description: L’élément AttachmentShape identifie les propriétés supplémentaires à renvoyer dans une réponse à une demande GetAttachment.
ms.openlocfilehash: e70fbaad0f649c5afdc151b777efef0f8927ba1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529664"
---
# <a name="attachmentshape"></a><span data-ttu-id="fb761-103">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="fb761-103">AttachmentShape</span></span>

<span data-ttu-id="fb761-104">L’élément **AttachmentShape** identifie les propriétés supplémentaires à renvoyer dans une réponse à une demande [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="fb761-104">The **AttachmentShape** element identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> 
  
- [<span data-ttu-id="fb761-105">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="fb761-105">GetAttachment</span></span>](getattachment.md)
  
- [<span data-ttu-id="fb761-106">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="fb761-106">AttachmentShape</span></span>](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 <span data-ttu-id="fb761-107">**AttachmentResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="fb761-107">**AttachmentResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb761-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fb761-108">Attributes and elements</span></span>

<span data-ttu-id="fb761-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fb761-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb761-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="fb761-110">Attributes</span></span>

<span data-ttu-id="fb761-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fb761-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb761-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fb761-112">Child elements</span></span>

|<span data-ttu-id="fb761-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fb761-113">**Element**</span></span>|<span data-ttu-id="fb761-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb761-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb761-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="fb761-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="fb761-116">Indique si le contenu MIME (Multipurpose Internet Mail Extensions) d’un élément ou d’une pièce jointe est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="fb761-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> <span data-ttu-id="fb761-117">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="fb761-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="fb761-118">BodyType</span><span class="sxs-lookup"><span data-stu-id="fb761-118">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="fb761-119">Identifie la façon dont le corps de texte est mis en forme dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="fb761-119">Identifies how the body text is formatted in the response.</span></span> <span data-ttu-id="fb761-120">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="fb761-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="fb761-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="fb761-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="fb761-122">Indique si le contenu HTML potentiellement dangereux est filtré à partir d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="fb761-122">Specifies whether potentially unsafe HTML content is filtered from an attachment.</span></span> <span data-ttu-id="fb761-123">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="fb761-123">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="fb761-124">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="fb761-124">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="fb761-125">Identifie les propriétés supplémentaires à renvoyer dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="fb761-125">Identifies additional properties to return in a response.</span></span> <span data-ttu-id="fb761-126">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="fb761-126">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb761-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fb761-127">Parent elements</span></span>

|<span data-ttu-id="fb761-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fb761-128">**Element**</span></span>|<span data-ttu-id="fb761-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb761-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb761-130">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="fb761-130">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="fb761-131">Élément qui définit une demande d’obtention d’une pièce jointe à partir d’une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb761-131">The element that defines a request to get an attachment from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="fb761-132">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="fb761-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb761-133">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="fb761-133">Text value</span></span>

<span data-ttu-id="fb761-134">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fb761-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb761-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="fb761-135">Remarks</span></span>

<span data-ttu-id="fb761-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb761-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb761-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fb761-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb761-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fb761-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fb761-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fb761-139">Schema Name</span></span>  <br/> |<span data-ttu-id="fb761-140">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="fb761-140">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fb761-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fb761-141">Validation File</span></span>  <br/> |<span data-ttu-id="fb761-142">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fb761-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb761-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fb761-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb761-144">False</span><span class="sxs-lookup"><span data-stu-id="fb761-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb761-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fb761-145">See also</span></span>

- [<span data-ttu-id="fb761-146">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="fb761-146">GetAttachment operation</span></span>](getattachment-operation.md)
- [<span data-ttu-id="fb761-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fb761-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

