---
title: GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: L’élément GetAttachment est l’élément racine dans une demande pour obtenir une pièce jointe à partir de la banque d’informations Exchange.
ms.openlocfilehash: fb639c86a0654e8f9e9601310f7c2f5b0fc7d729
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756524"
---
# <a name="getattachment"></a><span data-ttu-id="86f8a-103">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="86f8a-103">GetAttachment</span></span>

<span data-ttu-id="86f8a-104">L’élément **GetAttachment** est l’élément racine dans une demande pour obtenir une pièce jointe à partir de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="86f8a-104">The **GetAttachment** element is the root element in a request to get an attachment from the Exchange store.</span></span> 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 <span data-ttu-id="86f8a-105">**GetAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="86f8a-105">**GetAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86f8a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="86f8a-106">Attributes and elements</span></span>

<span data-ttu-id="86f8a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="86f8a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86f8a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="86f8a-108">Attributes</span></span>

<span data-ttu-id="86f8a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="86f8a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86f8a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="86f8a-110">Child elements</span></span>

|<span data-ttu-id="86f8a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="86f8a-111">**Element**</span></span>|<span data-ttu-id="86f8a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="86f8a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86f8a-113">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="86f8a-113">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="86f8a-114">Identifie les propriétés totale de l’article à renvoyer dans une réponse à une demande [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="86f8a-114">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> <span data-ttu-id="86f8a-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="86f8a-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="86f8a-116">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="86f8a-116">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="86f8a-117">Contient un tableau d’identificateurs de pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="86f8a-117">Contains an array of attachment identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="86f8a-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="86f8a-118">Parent elements</span></span>

<span data-ttu-id="86f8a-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="86f8a-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="86f8a-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="86f8a-120">Remarks</span></span>

<span data-ttu-id="86f8a-121">L’élément [AttachmentShape](attachmentshape.md) n’est pas nécessaire pour identifier les propriétés renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="86f8a-121">The [AttachmentShape](attachmentshape.md) element is not required to identify the properties returned in the response.</span></span> <span data-ttu-id="86f8a-122">L' [opération GetAttachment](getattachment-operation.md) renvoie le nom, ContentType, ContentId, ContentLocation et les propriétés du contenu des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="86f8a-122">The [GetAttachment operation](getattachment-operation.md) returns the Name, ContentType, ContentId, ContentLocation, and the Content properties for file attachments.</span></span> <span data-ttu-id="86f8a-123">Les pièces jointes d’élément, les propriétés retournées sont le nom, ContentType, ContentId, ContentLocation et toutes les attaché propriétés de l’élément.</span><span class="sxs-lookup"><span data-stu-id="86f8a-123">For item attachments, the returned properties are the Name, ContentType, ContentId, ContentLocation, and all the attached item's properties.</span></span> <span data-ttu-id="86f8a-124">Cela équivaut à l’utilisation de la forme de base AllProperties dans une demande de [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="86f8a-124">This is equivalent to using the AllProperties base shape in a [GetItem](getitem.md) request.</span></span> 
  
<span data-ttu-id="86f8a-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="86f8a-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86f8a-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="86f8a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86f8a-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="86f8a-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="86f8a-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="86f8a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="86f8a-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="86f8a-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="86f8a-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="86f8a-130">Validation File</span></span>  <br/> |<span data-ttu-id="86f8a-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="86f8a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="86f8a-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="86f8a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="86f8a-133">False</span><span class="sxs-lookup"><span data-stu-id="86f8a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86f8a-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="86f8a-134">See also</span></span>



[<span data-ttu-id="86f8a-135">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="86f8a-135">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="86f8a-136">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="86f8a-136">GetAttachmentResponse</span></span>](getattachmentresponse.md)

