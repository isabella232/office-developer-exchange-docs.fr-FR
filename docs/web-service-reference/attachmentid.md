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
description: L’élément AttachmentId identifie un élément ou fichier des pièces jointes. Cet élément est utilisé dans les réponses CreateAttachment.
ms.openlocfilehash: 2910503d1661ca3aaeeb4e319deb39f6b57c5c0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755335"
---
# <a name="attachmentid"></a><span data-ttu-id="ce3d6-104">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="ce3d6-104">AttachmentId</span></span>

<span data-ttu-id="ce3d6-105">L’élément **AttachmentId** identifie un élément ou fichier des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-105">The **AttachmentId** element identifies an item or file attachment.</span></span> <span data-ttu-id="ce3d6-106">Cet élément est utilisé dans les réponses CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-106">This element is used in CreateAttachment responses.</span></span> 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="ce3d6-107">**AttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-107">**AttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce3d6-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ce3d6-108">Attributes and elements</span></span>

<span data-ttu-id="ce3d6-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce3d6-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="ce3d6-110">Attributes</span></span>

|<span data-ttu-id="ce3d6-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-111">**Attribute**</span></span>|<span data-ttu-id="ce3d6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ce3d6-113">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-113">**Id**</span></span> <br/> |<span data-ttu-id="ce3d6-114">Identifie l’identificateur unique de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-114">Identifies the unique identifier of the attachment.</span></span>  <br/> |
|<span data-ttu-id="ce3d6-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="ce3d6-116">Identifie l’identificateur unique de l’élément racine du magasin à laquelle la pièce jointe est associée.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-116">Identifies the unique identifier of the root store item to which the attachment is attached.</span></span>  <br/> |
|<span data-ttu-id="ce3d6-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="ce3d6-118">Identifie la touche de modification de l’élément racine du magasin à laquelle la pièce jointe est associée.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-118">Identifies the change key of the root store item to which the attachment is attached.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ce3d6-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ce3d6-119">Child elements</span></span>

<span data-ttu-id="ce3d6-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ce3d6-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ce3d6-121">Parent elements</span></span>

|<span data-ttu-id="ce3d6-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-122">**Element**</span></span>|<span data-ttu-id="ce3d6-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce3d6-124">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="ce3d6-124">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="ce3d6-125">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-125">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="ce3d6-126">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="ce3d6-126">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="ce3d6-127">Représente un fichier qui est attaché à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-127">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ce3d6-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="ce3d6-128">Remarks</span></span>

<span data-ttu-id="ce3d6-129">Il est important de noter que lorsqu’une pièce jointe est créée, la modifier la clé de l’élément racine est modifiée.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-129">It is important to note that when an attachment is created, the change key of the root item is altered.</span></span>
  
<span data-ttu-id="ce3d6-130">L’élément [AttachmentId (GetAttachment et DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) est utilisé dans les requêtes DeleteAttachment et GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-130">The [AttachmentId (GetAttachment and DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) element is used in DeleteAttachment and GetAttachment requests.</span></span> 
  
<span data-ttu-id="ce3d6-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ce3d6-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce3d6-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ce3d6-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce3d6-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ce3d6-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ce3d6-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ce3d6-134">Schema name</span></span>  <br/> |<span data-ttu-id="ce3d6-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ce3d6-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="ce3d6-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ce3d6-136">Validation file</span></span>  <br/> |<span data-ttu-id="ce3d6-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ce3d6-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ce3d6-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ce3d6-138">Can be empty</span></span>  <br/> |<span data-ttu-id="ce3d6-139">False</span><span class="sxs-lookup"><span data-stu-id="ce3d6-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce3d6-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ce3d6-140">See also</span></span>

- [<span data-ttu-id="ce3d6-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ce3d6-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

