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
description: L’élément FileAttachment représente un fichier qui est attaché à un élément dans la banque d’informations Exchange.
ms.openlocfilehash: 5ce7aef753313aa9430f640bb3c26f652b8c1c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756368"
---
# <a name="fileattachment"></a><span data-ttu-id="8fedc-103">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="8fedc-103">FileAttachment</span></span>

<span data-ttu-id="8fedc-104">L’élément **FileAttachment** représente un fichier qui est attaché à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="8fedc-104">The **FileAttachment** element represents a file that is attached to an item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="8fedc-105">**FileAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="8fedc-105">**FileAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8fedc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8fedc-106">Attributes and elements</span></span>

<span data-ttu-id="8fedc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8fedc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fedc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8fedc-108">Attributes</span></span>

<span data-ttu-id="8fedc-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8fedc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8fedc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8fedc-110">Child elements</span></span>

|<span data-ttu-id="8fedc-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8fedc-111">**Element**</span></span>|<span data-ttu-id="8fedc-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8fedc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fedc-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="8fedc-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="8fedc-114">Identifie la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="8fedc-114">Identifies the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="8fedc-115">Nom (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="8fedc-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="8fedc-116">Représente le nom de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="8fedc-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="8fedc-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="8fedc-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="8fedc-118">Décrit le type Multipurpose Internet Mail Extensions (MIME) du contenu des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="8fedc-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="8fedc-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="8fedc-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="8fedc-120">Représente un identificateur pour le contenu d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="8fedc-120">Represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="8fedc-121">[ContentId](contentid.md) peut être définie à n’importe quelle valeur de chaîne.</span><span class="sxs-lookup"><span data-stu-id="8fedc-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="8fedc-122">Applications peuvent utiliser [ContentId](contentid.md) pour implémenter leurs propres mécanismes d’identification.</span><span class="sxs-lookup"><span data-stu-id="8fedc-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="8fedc-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="8fedc-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="8fedc-124">Contient l’identificateur de ressource uniforme (URI) qui correspond à l’emplacement du contenu de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="8fedc-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="8fedc-125">Size</span><span class="sxs-lookup"><span data-stu-id="8fedc-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="8fedc-126">Représente la taille en octets de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="8fedc-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="8fedc-127">Heure de dernière modification</span><span class="sxs-lookup"><span data-stu-id="8fedc-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="8fedc-128">Représente la dernière modification de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="8fedc-128">Represents when the file attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="8fedc-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="8fedc-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="8fedc-130">Indique si la pièce jointe apparaît en ligne au sein d’un élément.</span><span class="sxs-lookup"><span data-stu-id="8fedc-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="8fedc-131">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="8fedc-131">IsContactPhoto</span></span>](iscontactphoto.md) <br/> |<span data-ttu-id="8fedc-132">Indique si la pièce jointe est une image du contact.</span><span class="sxs-lookup"><span data-stu-id="8fedc-132">Indicates whether the file attachment is a contact picture.</span></span>  <br/> |
|[<span data-ttu-id="8fedc-133">Content</span><span class="sxs-lookup"><span data-stu-id="8fedc-133">Content</span></span>](content.md) <br/> |<span data-ttu-id="8fedc-134">Contient le contenu de la pièce jointe codée en Base64.</span><span class="sxs-lookup"><span data-stu-id="8fedc-134">Contains the Base64-encoded contents of the file attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8fedc-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8fedc-135">Parent elements</span></span>

|<span data-ttu-id="8fedc-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8fedc-136">**Element**</span></span>|<span data-ttu-id="8fedc-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="8fedc-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fedc-138">Attachments</span><span class="sxs-lookup"><span data-stu-id="8fedc-138">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8fedc-139">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="8fedc-139">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8fedc-140">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8fedc-140">Text value</span></span>

<span data-ttu-id="8fedc-141">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8fedc-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8fedc-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="8fedc-142">Remarks</span></span>

<span data-ttu-id="8fedc-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8fedc-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8fedc-144">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8fedc-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8fedc-145">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8fedc-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8fedc-146">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8fedc-146">Schema name</span></span>  <br/> |<span data-ttu-id="8fedc-147">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8fedc-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="8fedc-148">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8fedc-148">Validation file</span></span>  <br/> |<span data-ttu-id="8fedc-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8fedc-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8fedc-150">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8fedc-150">Can be empty</span></span>  <br/> |<span data-ttu-id="8fedc-151">False</span><span class="sxs-lookup"><span data-stu-id="8fedc-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8fedc-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8fedc-152">See also</span></span>



- [<span data-ttu-id="8fedc-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8fedc-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

