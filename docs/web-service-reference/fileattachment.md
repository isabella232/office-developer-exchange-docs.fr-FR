---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: L’élément FileAttachment représente un fichier joint à un élément dans la Banque d’Exchange.
ms.openlocfilehash: db9b541fb2527ae3c09cbdb33bedea7fb215bd30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461015"
---
# <a name="fileattachment"></a><span data-ttu-id="ea205-103">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="ea205-103">FileAttachment</span></span>

<span data-ttu-id="ea205-104">L’élément **FileAttachment** représente un fichier joint à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea205-104">The **FileAttachment** element represents a file that is attached to an item in the Exchange store.</span></span> 
  
```XML
<FileAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <IsContactPhoto/>
   <Content/>
</FileAttachment>
```

 <span data-ttu-id="ea205-105">**FileAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="ea205-105">**FileAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea205-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ea205-106">Attributes and elements</span></span>

<span data-ttu-id="ea205-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ea205-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea205-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ea205-108">Attributes</span></span>

<span data-ttu-id="ea205-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ea205-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea205-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ea205-110">Child elements</span></span>

|<span data-ttu-id="ea205-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ea205-111">**Element**</span></span>|<span data-ttu-id="ea205-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea205-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea205-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="ea205-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="ea205-114">Identifie le fichier en pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ea205-114">Identifies the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="ea205-115">Nom (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="ea205-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="ea205-116">Représente le nom de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ea205-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="ea205-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="ea205-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="ea205-118">Décrit le type MIME (Multipurpose Internet Mail Extensions) du contenu des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="ea205-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="ea205-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="ea205-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="ea205-120">Représente un identificateur pour le contenu d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ea205-120">Represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="ea205-121">[Contentid](contentid.md) peut être défini sur n’importe quelle valeur de chaîne.</span><span class="sxs-lookup"><span data-stu-id="ea205-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="ea205-122">Les applications peuvent utiliser [contentid](contentid.md) pour implémenter leurs propres mécanismes d’identification.</span><span class="sxs-lookup"><span data-stu-id="ea205-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="ea205-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="ea205-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="ea205-124">Contient l’URI (Uniform Resource Identifier) qui correspond à l’emplacement du contenu de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ea205-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="ea205-125">Taille</span><span class="sxs-lookup"><span data-stu-id="ea205-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="ea205-126">Représente la taille en octets de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ea205-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="ea205-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="ea205-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="ea205-128">Représente la dernière modification de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ea205-128">Represents when the file attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="ea205-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="ea205-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="ea205-130">Indique si la pièce jointe s’affiche en ligne dans un élément.</span><span class="sxs-lookup"><span data-stu-id="ea205-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="ea205-131">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="ea205-131">IsContactPhoto</span></span>](iscontactphoto.md) <br/> |<span data-ttu-id="ea205-132">Indique si la pièce jointe est une image de contact.</span><span class="sxs-lookup"><span data-stu-id="ea205-132">Indicates whether the file attachment is a contact picture.</span></span>  <br/> |
|[<span data-ttu-id="ea205-133">Content</span><span class="sxs-lookup"><span data-stu-id="ea205-133">Content</span></span>](content.md) <br/> |<span data-ttu-id="ea205-134">Contient le contenu encodé en base64 du fichier en pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ea205-134">Contains the Base64-encoded contents of the file attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea205-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ea205-135">Parent elements</span></span>

|<span data-ttu-id="ea205-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ea205-136">**Element**</span></span>|<span data-ttu-id="ea205-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea205-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea205-138">Attachments</span><span class="sxs-lookup"><span data-stu-id="ea205-138">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ea205-139">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea205-139">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ea205-140">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ea205-140">Text value</span></span>

<span data-ttu-id="ea205-141">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ea205-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ea205-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="ea205-142">Remarks</span></span>

<span data-ttu-id="ea205-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea205-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea205-144">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ea205-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea205-145">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ea205-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea205-146">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ea205-146">Schema name</span></span>  <br/> |<span data-ttu-id="ea205-147">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ea205-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="ea205-148">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ea205-148">Validation file</span></span>  <br/> |<span data-ttu-id="ea205-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ea205-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea205-150">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ea205-150">Can be empty</span></span>  <br/> |<span data-ttu-id="ea205-151">False</span><span class="sxs-lookup"><span data-stu-id="ea205-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea205-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ea205-152">See also</span></span>



- [<span data-ttu-id="ea205-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ea205-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

