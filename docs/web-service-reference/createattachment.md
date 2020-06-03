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
description: L’élément CreateAttachment définit une demande de création d’une pièce jointe à un élément dans la Banque d’Exchange.
ms.openlocfilehash: 4cba1b8865dae5da58b9617b249a29314c67331a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466436"
---
# <a name="createattachment"></a><span data-ttu-id="9e154-103">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="9e154-103">CreateAttachment</span></span>

<span data-ttu-id="9e154-104">L’élément **CreateAttachment** définit une demande de création d’une pièce jointe à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e154-104">The **CreateAttachment** element defines a request to create an attachment to an item in the Exchange store.</span></span> 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 <span data-ttu-id="9e154-105">**CreateAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="9e154-105">**CreateAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e154-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9e154-106">Attributes and elements</span></span>

<span data-ttu-id="9e154-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9e154-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e154-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9e154-108">Attributes</span></span>

<span data-ttu-id="9e154-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9e154-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e154-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9e154-110">Child elements</span></span>

|<span data-ttu-id="9e154-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9e154-111">**Element**</span></span>|<span data-ttu-id="9e154-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9e154-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e154-113">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="9e154-113">ParentItemId</span></span>](parentitemid.md) <br/> |<span data-ttu-id="9e154-114">Identifie l’élément de la banque Exchange parente qui contient la pièce jointe créée.</span><span class="sxs-lookup"><span data-stu-id="9e154-114">Identifies the parent Exchange store item that contains the created attachment.</span></span> <span data-ttu-id="9e154-115">L’élément [parentItemId](parentitemid.md) doit fournir l’ID d’un élément réel de la Banque d’identités Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e154-115">The [ParentItemId](parentitemid.md) element must provide the ID of a real Exchange store item.</span></span> <span data-ttu-id="9e154-116">Les éléments de magasin réel peuvent être récupérés à l’aide de l' [opération GetItem](getitem-operation.md); les pièces jointes sont récupérées à l’aide de l' [opération GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9e154-116">Real store items can be retrieved by using the [GetItem operation](getitem-operation.md); attachments are retrieved by using the [GetAttachment operation](getattachment-operation.md).</span></span> <span data-ttu-id="9e154-117">Une erreur se produit si l’ID d’une pièce jointe est transmis à [parentItemId](parentitemid.md) .</span><span class="sxs-lookup"><span data-stu-id="9e154-117">An error occurs if the [ParentItemId](parentitemid.md) is passed the ID of a file attachment.</span></span> <span data-ttu-id="9e154-118">Si le [parentItemId](parentitemid.md) représente l’ID d’une pièce jointe d’un élément existant, l' [opération CreateAttachment](createattachment-operation.md) ajoute la nouvelle pièce jointe à la pièce jointe existante.</span><span class="sxs-lookup"><span data-stu-id="9e154-118">If the [ParentItemId](parentitemid.md) represents the ID of an existing item attachment, the [CreateAttachment operation](createattachment-operation.md) adds the new attachment to the existing attachment.</span></span>  <br/> <span data-ttu-id="9e154-119">Cet élément est requis pour l' [opération CreateAttachment](createattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9e154-119">This element is required for the [CreateAttachment operation](createattachment-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="9e154-120">Attachments</span><span class="sxs-lookup"><span data-stu-id="9e154-120">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9e154-121">Contient les éléments ou les fichiers à joindre à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e154-121">Contains the items or files to attach to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e154-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9e154-122">Parent elements</span></span>

<span data-ttu-id="9e154-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9e154-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e154-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="9e154-124">Remarks</span></span>

<span data-ttu-id="9e154-125">Une pièce jointe d’élément n’existe pas en tant qu’élément de la boutique.</span><span class="sxs-lookup"><span data-stu-id="9e154-125">An item attachment does not exist as a store item.</span></span> <span data-ttu-id="9e154-126">Il existe uniquement en tant que pièce jointe à un élément ou à une autre pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="9e154-126">It only exists as an attachment to an item or another attachment.</span></span> <span data-ttu-id="9e154-127">Les pièces jointes d’éléments ne peuvent être récupérées qu’à l’aide de la demande [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="9e154-127">Item attachments can only be retrieved by using the [GetAttachment](getattachment.md) request.</span></span> 
  
<span data-ttu-id="9e154-128">Les pièces jointes d’éléments suivantes peuvent être créées :</span><span class="sxs-lookup"><span data-stu-id="9e154-128">The following item attachments can be created:</span></span>
  
- <span data-ttu-id="9e154-129">Option</span><span class="sxs-lookup"><span data-stu-id="9e154-129">Item</span></span>
    
- <span data-ttu-id="9e154-130">Message</span><span class="sxs-lookup"><span data-stu-id="9e154-130">Message</span></span>
    
- <span data-ttu-id="9e154-131">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="9e154-131">CalendarItem</span></span>
    
- <span data-ttu-id="9e154-132">Contact</span><span class="sxs-lookup"><span data-stu-id="9e154-132">Contact</span></span>
    
- <span data-ttu-id="9e154-133">Tâche</span><span class="sxs-lookup"><span data-stu-id="9e154-133">Task</span></span>
    
- <span data-ttu-id="9e154-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="9e154-134">MeetingMessage</span></span>
    
- <span data-ttu-id="9e154-135">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="9e154-135">MeetingRequest</span></span>
    
<span data-ttu-id="9e154-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9e154-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="9e154-137">Exemple</span><span class="sxs-lookup"><span data-stu-id="9e154-137">Example</span></span>

<span data-ttu-id="9e154-138">L’exemple suivant montre comment créer et attacher un élément à un autre élément dans la Banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e154-138">The following example shows how to create and attach an item to another item in the Exchange store.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="9e154-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9e154-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e154-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9e154-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e154-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9e154-141">Schema Name</span></span>  <br/> |<span data-ttu-id="9e154-142">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9e154-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9e154-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9e154-143">Validation File</span></span>  <br/> |<span data-ttu-id="9e154-144">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9e154-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e154-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9e154-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e154-146">False</span><span class="sxs-lookup"><span data-stu-id="9e154-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e154-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9e154-147">See also</span></span>



[<span data-ttu-id="9e154-148">Opération CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="9e154-148">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="9e154-149">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="9e154-149">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="9e154-150">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="9e154-150">GetAttachment operation</span></span>](getattachment-operation.md)

