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
ms.openlocfilehash: 7bd3d22430fe04f1b28ae240102500609fe8d703
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353146"
---
# <a name="itemattachment"></a><span data-ttu-id="ff531-103">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="ff531-103">ItemAttachment</span></span>

<span data-ttu-id="ff531-104">L’élément **ItemAttachment** représente un élément Exchange qui est attaché à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff531-104">The **ItemAttachment** element represents an Exchange item that is attached to another Exchange item.</span></span> 
  
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

<span data-ttu-id="ff531-105">**ItemAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="ff531-105">**ItemAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ff531-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ff531-106">Attributes and elements</span></span>

<span data-ttu-id="ff531-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ff531-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff531-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ff531-108">Attributes</span></span>

<span data-ttu-id="ff531-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ff531-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff531-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ff531-110">Child elements</span></span>

|<span data-ttu-id="ff531-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ff531-111">**Element**</span></span>|<span data-ttu-id="ff531-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ff531-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff531-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="ff531-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="ff531-114">Identifie la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ff531-114">Identifies the attachment.</span></span>  <br/> |
|[<span data-ttu-id="ff531-115">Name (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="ff531-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="ff531-116">Représente le nom de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ff531-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="ff531-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="ff531-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="ff531-118">Décrit le type Multipurpose Internet Mail Extensions (MIME) du contenu des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="ff531-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="ff531-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="ff531-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="ff531-120">Représente un identificateur pour le contenu de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ff531-120">Represents an identifier to the contents of the attachment.</span></span> <span data-ttu-id="ff531-121">[ContentId](contentid.md) peut être définie à n’importe quelle valeur de chaîne.</span><span class="sxs-lookup"><span data-stu-id="ff531-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="ff531-122">Applications peuvent utiliser [ContentId](contentid.md) pour implémenter leurs propres mécanismes d’identification.</span><span class="sxs-lookup"><span data-stu-id="ff531-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="ff531-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="ff531-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="ff531-124">Contient l’identificateur de ressource uniforme (URI) qui correspond à l’emplacement du contenu de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ff531-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="ff531-125">Size</span><span class="sxs-lookup"><span data-stu-id="ff531-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="ff531-126">Représente la taille en octets de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ff531-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="ff531-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="ff531-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="ff531-128">Représente la dernière modification de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ff531-128">Represents when the attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="ff531-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="ff531-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="ff531-130">Indique si la pièce jointe apparaît en ligne au sein d’un élément.</span><span class="sxs-lookup"><span data-stu-id="ff531-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="ff531-131">Item</span><span class="sxs-lookup"><span data-stu-id="ff531-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="ff531-132">Représente une pièce jointe d’élément Exchange générique.</span><span class="sxs-lookup"><span data-stu-id="ff531-132">Represents a generic Exchange item attachment.</span></span>  <br/> |
|[<span data-ttu-id="ff531-133">Message</span><span class="sxs-lookup"><span data-stu-id="ff531-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ff531-134">Représente une pièce jointe du message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff531-134">Represents an Exchange e-mail message attachment.</span></span>  <br/> |
|[<span data-ttu-id="ff531-135">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ff531-135">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ff531-136">Représente une pièce jointe élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff531-136">Represents an Exchange calendar item attachment.</span></span>  <br/> |
|[<span data-ttu-id="ff531-137">Contact</span><span class="sxs-lookup"><span data-stu-id="ff531-137">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="ff531-138">Représente les pièces jointes à un élément de contact d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff531-138">Represents an Exchange contact item attachment.</span></span>  <br/> |
|[<span data-ttu-id="ff531-139">Tâche</span><span class="sxs-lookup"><span data-stu-id="ff531-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="ff531-140">Représente une pièce jointe de tâche Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff531-140">Represents an Exchange task attachment.</span></span>  <br/> |
|[<span data-ttu-id="ff531-141">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ff531-141">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="ff531-142">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff531-142">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ff531-143">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ff531-143">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ff531-144">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff531-144">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ff531-145">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="ff531-145">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="ff531-146">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff531-146">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ff531-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="ff531-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="ff531-148">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff531-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff531-149">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ff531-149">Parent elements</span></span>

|<span data-ttu-id="ff531-150">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ff531-150">**Element**</span></span>|<span data-ttu-id="ff531-151">**Description**</span><span class="sxs-lookup"><span data-stu-id="ff531-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff531-152">Pièces jointes</span><span class="sxs-lookup"><span data-stu-id="ff531-152">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ff531-153">Contient les articles et/ou les fichiers associés à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff531-153">Contains the items and/or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ff531-154">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ff531-154">Text value</span></span>

<span data-ttu-id="ff531-155">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ff531-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ff531-156">Remarques</span><span class="sxs-lookup"><span data-stu-id="ff531-156">Remarks</span></span>

<span data-ttu-id="ff531-157">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff531-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff531-158">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ff531-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff531-159">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ff531-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ff531-160">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ff531-160">Schema Name</span></span>  <br/> |<span data-ttu-id="ff531-161">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ff531-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="ff531-162">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ff531-162">Validation File</span></span>  <br/> |<span data-ttu-id="ff531-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ff531-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ff531-164">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ff531-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff531-165">False</span><span class="sxs-lookup"><span data-stu-id="ff531-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff531-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ff531-166">See also</span></span>

- [<span data-ttu-id="ff531-167">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ff531-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

