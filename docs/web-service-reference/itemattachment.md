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
ms.openlocfilehash: 87e0331664f1fdf8857afc78500014d138f05401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828137"
---
# <a name="itemattachment"></a><span data-ttu-id="ce755-103">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="ce755-103">ItemAttachment</span></span>

<span data-ttu-id="ce755-104">L’élément **ItemAttachment** représente un élément Exchange qui est attaché à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce755-104">The **ItemAttachment** element represents an Exchange item that is attached to another Exchange item.</span></span> 
  
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

 <span data-ttu-id="ce755-105">**ItemAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="ce755-105">**ItemAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce755-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ce755-106">Attributes and elements</span></span>

<span data-ttu-id="ce755-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ce755-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce755-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ce755-108">Attributes</span></span>

<span data-ttu-id="ce755-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ce755-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce755-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ce755-110">Child elements</span></span>

|<span data-ttu-id="ce755-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ce755-111">**Element**</span></span>|<span data-ttu-id="ce755-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ce755-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce755-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="ce755-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="ce755-114">Identifie la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ce755-114">Identifies the attachment.</span></span>  <br/> |
|[<span data-ttu-id="ce755-115">Nom (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="ce755-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="ce755-116">Représente le nom de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ce755-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="ce755-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="ce755-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="ce755-118">Décrit le type Multipurpose Internet Mail Extensions (MIME) du contenu des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="ce755-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="ce755-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="ce755-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="ce755-120">Représente un identificateur pour le contenu de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ce755-120">Represents an identifier to the contents of the attachment.</span></span> <span data-ttu-id="ce755-121">[ContentId](contentid.md) peut être définie à n’importe quelle valeur de chaîne.</span><span class="sxs-lookup"><span data-stu-id="ce755-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="ce755-122">Applications peuvent utiliser [ContentId](contentid.md) pour implémenter leurs propres mécanismes d’identification.</span><span class="sxs-lookup"><span data-stu-id="ce755-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="ce755-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="ce755-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="ce755-124">Contient l’identificateur de ressource uniforme (URI) qui correspond à l’emplacement du contenu de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ce755-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="ce755-125">Size</span><span class="sxs-lookup"><span data-stu-id="ce755-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="ce755-126">Représente la taille en octets de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ce755-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="ce755-127">Heure de dernière modification</span><span class="sxs-lookup"><span data-stu-id="ce755-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="ce755-128">Représente la dernière modification de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ce755-128">Represents when the attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="ce755-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="ce755-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="ce755-130">Indique si la pièce jointe apparaît en ligne au sein d’un élément.</span><span class="sxs-lookup"><span data-stu-id="ce755-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="ce755-131">Item</span><span class="sxs-lookup"><span data-stu-id="ce755-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="ce755-132">Représente une pièce jointe d’élément Exchange générique.</span><span class="sxs-lookup"><span data-stu-id="ce755-132">Represents a generic Exchange item attachment.</span></span>  <br/> |
|[<span data-ttu-id="ce755-133">Message</span><span class="sxs-lookup"><span data-stu-id="ce755-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ce755-134">Représente une pièce jointe du message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce755-134">Represents an Exchange e-mail message attachment.</span></span>  <br/> |
|[<span data-ttu-id="ce755-135">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ce755-135">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ce755-136">Représente une pièce jointe élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce755-136">Represents an Exchange calendar item attachment.</span></span>  <br/> |
|[<span data-ttu-id="ce755-137">Contact</span><span class="sxs-lookup"><span data-stu-id="ce755-137">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="ce755-138">Représente les pièces jointes à un élément de contact d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce755-138">Represents an Exchange contact item attachment.</span></span>  <br/> |
|[<span data-ttu-id="ce755-139">Tâche</span><span class="sxs-lookup"><span data-stu-id="ce755-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="ce755-140">Représente une pièce jointe de tâche Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce755-140">Represents an Exchange task attachment.</span></span>  <br/> |
|[<span data-ttu-id="ce755-141">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ce755-141">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="ce755-142">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce755-142">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce755-143">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ce755-143">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ce755-144">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce755-144">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce755-145">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="ce755-145">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="ce755-146">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce755-146">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce755-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="ce755-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="ce755-148">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce755-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce755-149">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ce755-149">Parent elements</span></span>

|<span data-ttu-id="ce755-150">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ce755-150">**Element**</span></span>|<span data-ttu-id="ce755-151">**Description**</span><span class="sxs-lookup"><span data-stu-id="ce755-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce755-152">Pièces jointes</span><span class="sxs-lookup"><span data-stu-id="ce755-152">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ce755-153">Contient les articles et/ou les fichiers associés à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce755-153">Contains the items and/or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ce755-154">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ce755-154">Text value</span></span>

<span data-ttu-id="ce755-155">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ce755-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ce755-156">Remarques</span><span class="sxs-lookup"><span data-stu-id="ce755-156">Remarks</span></span>

<span data-ttu-id="ce755-157">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce755-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce755-158">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ce755-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce755-159">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ce755-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ce755-160">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ce755-160">Schema Name</span></span>  <br/> |<span data-ttu-id="ce755-161">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ce755-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="ce755-162">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ce755-162">Validation File</span></span>  <br/> |<span data-ttu-id="ce755-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ce755-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ce755-164">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ce755-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce755-165">False</span><span class="sxs-lookup"><span data-stu-id="ce755-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce755-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ce755-166">See also</span></span>



- [<span data-ttu-id="ce755-167">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ce755-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

