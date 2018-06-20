---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: L’élément CreateAttachment définit une demande pour créer une pièce jointe à un élément dans la banque d’informations Exchange.
ms.openlocfilehash: d403eb5ca15623d3a973f7b224dbcde5529cf1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755683"
---
# <a name="createattachment"></a><span data-ttu-id="f2ffd-103">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="f2ffd-103">CreateAttachment</span></span>

<span data-ttu-id="f2ffd-104">L’élément **CreateAttachment** définit une demande pour créer une pièce jointe à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-104">The **CreateAttachment** element defines a request to create an attachment to an item in the Exchange store.</span></span> 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 <span data-ttu-id="f2ffd-105">**CreateAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="f2ffd-105">**CreateAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2ffd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f2ffd-106">Attributes and elements</span></span>

<span data-ttu-id="f2ffd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2ffd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f2ffd-108">Attributes</span></span>

<span data-ttu-id="f2ffd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2ffd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f2ffd-110">Child elements</span></span>

|<span data-ttu-id="f2ffd-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f2ffd-111">**Element**</span></span>|<span data-ttu-id="f2ffd-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f2ffd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2ffd-113">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="f2ffd-113">ParentItemId</span></span>](parentitemid.md) <br/> |<span data-ttu-id="f2ffd-114">Identifie l’élément de magasin Exchange parent qui contient la pièce jointe créée.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-114">Identifies the parent Exchange store item that contains the created attachment.</span></span> <span data-ttu-id="f2ffd-115">L’élément [ParentItemId](parentitemid.md) doit fournir l’élément de magasin de l’ID d’un véritable Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-115">The [ParentItemId](parentitemid.md) element must provide the ID of a real Exchange store item.</span></span> <span data-ttu-id="f2ffd-116">Éléments de la banque réel peuvent être récupérés à l’aide de l' [opération GetItem](getitem-operation.md); pièces jointes sont récupérées à l’aide de l' [opération GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f2ffd-116">Real store items can be retrieved by using the [GetItem operation](getitem-operation.md); attachments are retrieved by using the [GetAttachment operation](getattachment-operation.md).</span></span> <span data-ttu-id="f2ffd-117">Une erreur se produit si le [ParentItemId](parentitemid.md) est transmis à l’ID d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-117">An error occurs if the [ParentItemId](parentitemid.md) is passed the ID of a file attachment.</span></span> <span data-ttu-id="f2ffd-118">Si le [ParentItemId](parentitemid.md) représente l’ID de pièce jointe d’élément existant, l' [opération CreateAttachment](createattachment-operation.md) ajoute la nouvelle pièce jointe à la pièce jointe existante.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-118">If the [ParentItemId](parentitemid.md) represents the ID of an existing item attachment, the [CreateAttachment operation](createattachment-operation.md) adds the new attachment to the existing attachment.</span></span>  <br/> <span data-ttu-id="f2ffd-119">Cet élément est requis pour l' [opération CreateAttachment](createattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f2ffd-119">This element is required for the [CreateAttachment operation](createattachment-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="f2ffd-120">Pièces jointes</span><span class="sxs-lookup"><span data-stu-id="f2ffd-120">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f2ffd-121">Contient les éléments ou les fichiers pour attacher à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-121">Contains the items or files to attach to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2ffd-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f2ffd-122">Parent elements</span></span>

<span data-ttu-id="f2ffd-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f2ffd-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="f2ffd-124">Remarks</span></span>

<span data-ttu-id="f2ffd-125">Une pièce jointe d’élément n’existe pas comme un élément de magasin.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-125">An item attachment does not exist as a store item.</span></span> <span data-ttu-id="f2ffd-126">Il existe uniquement en tant que pièce jointe à un élément ou une autre pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-126">It only exists as an attachment to an item or another attachment.</span></span> <span data-ttu-id="f2ffd-127">Pièces jointes d’élément ne peuvent être extrait à l’aide de la demande [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="f2ffd-127">Item attachments can only be retrieved by using the [GetAttachment](getattachment.md) request.</span></span> 
  
<span data-ttu-id="f2ffd-128">Vous pouvez créer les pièces jointes d’éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="f2ffd-128">The following item attachments can be created:</span></span>
  
- <span data-ttu-id="f2ffd-129">Élément</span><span class="sxs-lookup"><span data-stu-id="f2ffd-129">Item</span></span>
    
- <span data-ttu-id="f2ffd-130">Message</span><span class="sxs-lookup"><span data-stu-id="f2ffd-130">Message</span></span>
    
- <span data-ttu-id="f2ffd-131">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f2ffd-131">CalendarItem</span></span>
    
- <span data-ttu-id="f2ffd-132">Contact</span><span class="sxs-lookup"><span data-stu-id="f2ffd-132">Contact</span></span>
    
- <span data-ttu-id="f2ffd-133">Tâche</span><span class="sxs-lookup"><span data-stu-id="f2ffd-133">Task</span></span>
    
- <span data-ttu-id="f2ffd-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="f2ffd-134">MeetingMessage</span></span>
    
- <span data-ttu-id="f2ffd-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f2ffd-135">MeetingRequest</span></span>
    
<span data-ttu-id="f2ffd-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="f2ffd-137">Exemple</span><span class="sxs-lookup"><span data-stu-id="f2ffd-137">Example</span></span>

<span data-ttu-id="f2ffd-138">L’exemple suivant montre comment créer et joindre un élément à un autre élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2ffd-138">The following example shows how to create and attach an item to another item in the Exchange store.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="ASkAS"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>MyAttachment</t:Name>
          <t:Message>
            <t:ItemClass>IPM>Note</t:ItemClass>
            <t:Subject>My attachment subject</t:Subject>
            <t:Body BodyType="Text">My attachment body</t:Body>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="f2ffd-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f2ffd-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2ffd-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f2ffd-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f2ffd-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f2ffd-141">Schema Name</span></span>  <br/> |<span data-ttu-id="f2ffd-142">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f2ffd-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f2ffd-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f2ffd-143">Validation File</span></span>  <br/> |<span data-ttu-id="f2ffd-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f2ffd-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f2ffd-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f2ffd-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2ffd-146">False</span><span class="sxs-lookup"><span data-stu-id="f2ffd-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2ffd-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f2ffd-147">See also</span></span>



[<span data-ttu-id="f2ffd-148">Opération CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="f2ffd-148">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="f2ffd-149">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="f2ffd-149">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="f2ffd-150">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="f2ffd-150">GetAttachment operation</span></span>](getattachment-operation.md)

