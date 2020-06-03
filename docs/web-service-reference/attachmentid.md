---
title: AttachmentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: L’élément AttachmentId identifie un élément ou une pièce jointe. Cet élément est utilisé dans les réponses CreateAttachment.
ms.openlocfilehash: b5dc9299b615f0fc01b8afcbaabf0ec7996e53d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459110"
---
# <a name="attachmentid"></a><span data-ttu-id="319ef-104">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="319ef-104">AttachmentId</span></span>

<span data-ttu-id="319ef-105">L’élément **attachmentid** identifie un élément ou une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="319ef-105">The **AttachmentId** element identifies an item or file attachment.</span></span> <span data-ttu-id="319ef-106">Cet élément est utilisé dans les réponses CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="319ef-106">This element is used in CreateAttachment responses.</span></span> 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="319ef-107">**AttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="319ef-107">**AttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="319ef-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="319ef-108">Attributes and elements</span></span>

<span data-ttu-id="319ef-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="319ef-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="319ef-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="319ef-110">Attributes</span></span>

|<span data-ttu-id="319ef-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="319ef-111">**Attribute**</span></span>|<span data-ttu-id="319ef-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="319ef-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="319ef-113">**Id**</span><span class="sxs-lookup"><span data-stu-id="319ef-113">**Id**</span></span> <br/> |<span data-ttu-id="319ef-114">Identifie l’identificateur unique de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="319ef-114">Identifies the unique identifier of the attachment.</span></span>  <br/> |
|<span data-ttu-id="319ef-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="319ef-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="319ef-116">Identifie l’identificateur unique de l’élément de magasin racine auquel la pièce jointe est attachée.</span><span class="sxs-lookup"><span data-stu-id="319ef-116">Identifies the unique identifier of the root store item to which the attachment is attached.</span></span>  <br/> |
|<span data-ttu-id="319ef-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="319ef-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="319ef-118">Identifie la clé de modification de l’élément de magasin racine auquel la pièce jointe est attachée.</span><span class="sxs-lookup"><span data-stu-id="319ef-118">Identifies the change key of the root store item to which the attachment is attached.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="319ef-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="319ef-119">Child elements</span></span>

<span data-ttu-id="319ef-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="319ef-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="319ef-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="319ef-121">Parent elements</span></span>

|<span data-ttu-id="319ef-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="319ef-122">**Element**</span></span>|<span data-ttu-id="319ef-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="319ef-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="319ef-124">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="319ef-124">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="319ef-125">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="319ef-125">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="319ef-126">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="319ef-126">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="319ef-127">Représente un fichier joint à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="319ef-127">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="319ef-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="319ef-128">Remarks</span></span>

<span data-ttu-id="319ef-129">Il est important de noter que lors de la création d’une pièce jointe, la clé de modification de l’élément racine est modifiée.</span><span class="sxs-lookup"><span data-stu-id="319ef-129">It is important to note that when an attachment is created, the change key of the root item is altered.</span></span>
  
<span data-ttu-id="319ef-130">L’élément [attachmentid (GetAttachment et DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) est utilisé dans les requêtes DeleteAttachment et GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="319ef-130">The [AttachmentId (GetAttachment and DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) element is used in DeleteAttachment and GetAttachment requests.</span></span> 
  
<span data-ttu-id="319ef-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="319ef-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="319ef-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="319ef-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="319ef-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="319ef-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="319ef-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="319ef-134">Schema name</span></span>  <br/> |<span data-ttu-id="319ef-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="319ef-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="319ef-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="319ef-136">Validation file</span></span>  <br/> |<span data-ttu-id="319ef-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="319ef-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="319ef-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="319ef-138">Can be empty</span></span>  <br/> |<span data-ttu-id="319ef-139">False</span><span class="sxs-lookup"><span data-stu-id="319ef-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="319ef-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="319ef-140">See also</span></span>

- [<span data-ttu-id="319ef-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="319ef-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

