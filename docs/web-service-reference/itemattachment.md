---
title: ItemAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemAttachment
api_type:
- schema
ms.assetid: 089ee599-f45e-46f5-a18a-5cfb3d2851ff
description: L’élément ItemAttachment représente un élément Exchange qui est attaché à un autre élément Exchange.
ms.openlocfilehash: c3a07fa091c05654a03cbff58fb20204c26c9061
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526437"
---
# <a name="itemattachment"></a><span data-ttu-id="20f0d-103">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="20f0d-103">ItemAttachment</span></span>

<span data-ttu-id="20f0d-104">L’élément **ItemAttachment** représente un élément Exchange qui est attaché à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f0d-104">The **ItemAttachment** element represents an Exchange item that is attached to another Exchange item.</span></span> 
  
```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Item/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Message/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <CalendarItem/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Contact/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Task/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingMessage/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingRequest/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingResponse/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingCancellation/>
</ItemAttachment>
```

<span data-ttu-id="20f0d-105">**ItemAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="20f0d-105">**ItemAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="20f0d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="20f0d-106">Attributes and elements</span></span>

<span data-ttu-id="20f0d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="20f0d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20f0d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="20f0d-108">Attributes</span></span>

<span data-ttu-id="20f0d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="20f0d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20f0d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="20f0d-110">Child elements</span></span>

|<span data-ttu-id="20f0d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20f0d-111">**Element**</span></span>|<span data-ttu-id="20f0d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="20f0d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20f0d-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="20f0d-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="20f0d-114">Identifie la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="20f0d-114">Identifies the attachment.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-115">Nom (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="20f0d-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="20f0d-116">Représente le nom de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="20f0d-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="20f0d-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="20f0d-118">Décrit le type MIME (Multipurpose Internet Mail Extensions) du contenu des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="20f0d-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="20f0d-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="20f0d-120">Représente un identificateur du contenu de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="20f0d-120">Represents an identifier to the contents of the attachment.</span></span> <span data-ttu-id="20f0d-121">[Contentid](contentid.md) peut être défini sur n’importe quelle valeur de chaîne.</span><span class="sxs-lookup"><span data-stu-id="20f0d-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="20f0d-122">Les applications peuvent utiliser [contentid](contentid.md) pour implémenter leurs propres mécanismes d’identification.</span><span class="sxs-lookup"><span data-stu-id="20f0d-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="20f0d-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="20f0d-124">Contient l’URI (Uniform Resource Identifier) qui correspond à l’emplacement du contenu de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="20f0d-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-125">Taille</span><span class="sxs-lookup"><span data-stu-id="20f0d-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="20f0d-126">Représente la taille en octets de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="20f0d-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="20f0d-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="20f0d-128">Représente la dernière modification de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="20f0d-128">Represents when the attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="20f0d-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="20f0d-130">Indique si la pièce jointe s’affiche en ligne dans un élément.</span><span class="sxs-lookup"><span data-stu-id="20f0d-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-131">Élément</span><span class="sxs-lookup"><span data-stu-id="20f0d-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="20f0d-132">Représente une pièce jointe d’élément Exchange générique.</span><span class="sxs-lookup"><span data-stu-id="20f0d-132">Represents a generic Exchange item attachment.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-133">Message</span><span class="sxs-lookup"><span data-stu-id="20f0d-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="20f0d-134">Représente une pièce jointe de message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f0d-134">Represents an Exchange e-mail message attachment.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-135">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="20f0d-135">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="20f0d-136">Représente une pièce jointe d’un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f0d-136">Represents an Exchange calendar item attachment.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-137">Contact</span><span class="sxs-lookup"><span data-stu-id="20f0d-137">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="20f0d-138">Représente une pièce jointe d’un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f0d-138">Represents an Exchange contact item attachment.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-139">Task</span><span class="sxs-lookup"><span data-stu-id="20f0d-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="20f0d-140">Représente une pièce jointe de tâche Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f0d-140">Represents an Exchange task attachment.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-141">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="20f0d-141">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="20f0d-142">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f0d-142">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-143">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="20f0d-143">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="20f0d-144">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f0d-144">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-145">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="20f0d-145">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="20f0d-146">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f0d-146">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="20f0d-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="20f0d-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="20f0d-148">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f0d-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="20f0d-149">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="20f0d-149">Parent elements</span></span>

|<span data-ttu-id="20f0d-150">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20f0d-150">**Element**</span></span>|<span data-ttu-id="20f0d-151">**Description**</span><span class="sxs-lookup"><span data-stu-id="20f0d-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20f0d-152">Attachments</span><span class="sxs-lookup"><span data-stu-id="20f0d-152">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="20f0d-153">Contient les éléments et/ou les fichiers qui sont associés à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f0d-153">Contains the items and/or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20f0d-154">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="20f0d-154">Text value</span></span>

<span data-ttu-id="20f0d-155">Aucun.</span><span class="sxs-lookup"><span data-stu-id="20f0d-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="20f0d-156">Remarques</span><span class="sxs-lookup"><span data-stu-id="20f0d-156">Remarks</span></span>

<span data-ttu-id="20f0d-157">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f0d-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20f0d-158">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="20f0d-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20f0d-159">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="20f0d-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="20f0d-160">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="20f0d-160">Schema Name</span></span>  <br/> |<span data-ttu-id="20f0d-161">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="20f0d-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="20f0d-162">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="20f0d-162">Validation File</span></span>  <br/> |<span data-ttu-id="20f0d-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="20f0d-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="20f0d-164">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="20f0d-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="20f0d-165">False</span><span class="sxs-lookup"><span data-stu-id="20f0d-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20f0d-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="20f0d-166">See also</span></span>

- [<span data-ttu-id="20f0d-167">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="20f0d-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

