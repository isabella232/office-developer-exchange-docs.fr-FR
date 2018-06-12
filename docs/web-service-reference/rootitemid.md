---
title: RootItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootItemId
api_type:
- schema
ms.assetid: f613c705-17ce-48ce-aa64-4dc2cea25e31
description: L’élément RootItemId identifie l’élément racine d’une pièce jointe supprimée.
ms.openlocfilehash: 484b185db63c9692eaca7e43c49d6e95375a1a98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829251"
---
# <a name="rootitemid"></a><span data-ttu-id="d462e-103">RootItemId</span><span class="sxs-lookup"><span data-stu-id="d462e-103">RootItemId</span></span>

<span data-ttu-id="d462e-104">L’élément **RootItemId** identifie l’élément racine d’une pièce jointe supprimée.</span><span class="sxs-lookup"><span data-stu-id="d462e-104">The **RootItemId** element identifies the root item of a deleted attachment.</span></span> 
  
[<span data-ttu-id="d462e-105">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="d462e-105">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
  
[<span data-ttu-id="d462e-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d462e-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="d462e-107">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d462e-107">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
  
[<span data-ttu-id="d462e-108">RootItemId</span><span class="sxs-lookup"><span data-stu-id="d462e-108">RootItemId</span></span>](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="d462e-109">**RootItemIdType**</span><span class="sxs-lookup"><span data-stu-id="d462e-109">**RootItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d462e-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d462e-110">Attributes and elements</span></span>

<span data-ttu-id="d462e-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d462e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d462e-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="d462e-112">Attributes</span></span>

|<span data-ttu-id="d462e-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d462e-113">**Attribute**</span></span>|<span data-ttu-id="d462e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d462e-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d462e-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="d462e-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="d462e-116">Identifie l’élément racine d’une pièce jointe supprimée.</span><span class="sxs-lookup"><span data-stu-id="d462e-116">Identifies the root item of a deleted attachment.</span></span>  <br/> |
|<span data-ttu-id="d462e-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="d462e-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="d462e-118">Identifie la nouvelle clé de modification de l’élément racine d’une pièce jointe supprimée.</span><span class="sxs-lookup"><span data-stu-id="d462e-118">Identifies the new change key of the root item of a deleted attachment.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d462e-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d462e-119">Child elements</span></span>

<span data-ttu-id="d462e-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d462e-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d462e-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d462e-121">Parent elements</span></span>

|<span data-ttu-id="d462e-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d462e-122">**Element**</span></span>|<span data-ttu-id="d462e-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="d462e-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d462e-124">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d462e-124">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md) <br/> |<span data-ttu-id="d462e-125">Contient l’état et les résultats d’une demande DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="d462e-125">Contains the status and result of a DeleteAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d462e-126">Note</span><span class="sxs-lookup"><span data-stu-id="d462e-126">Remarks</span></span>

<span data-ttu-id="d462e-127">L’élément **RootItemId** est utilisé uniquement dans les réponses DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="d462e-127">The **RootItemId** element is only used in DeleteAttachment responses.</span></span> <span data-ttu-id="d462e-128">Identifie l’identificateur d’élément racine et plus important, la nouvelle clé de modification à l’élément parent.</span><span class="sxs-lookup"><span data-stu-id="d462e-128">This identifies the root item identifier, and more importantly, the new change key to the parent item.</span></span> 
  
<span data-ttu-id="d462e-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d462e-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d462e-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d462e-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d462e-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d462e-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d462e-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d462e-132">Schema name</span></span>  <br/> |<span data-ttu-id="d462e-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d462e-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d462e-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d462e-134">Validation file</span></span>  <br/> |<span data-ttu-id="d462e-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d462e-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d462e-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d462e-136">Can be empty</span></span>  <br/> |<span data-ttu-id="d462e-137">False</span><span class="sxs-lookup"><span data-stu-id="d462e-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d462e-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d462e-138">See also</span></span>



[<span data-ttu-id="d462e-139">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="d462e-139">DeleteAttachment</span></span>](deleteattachment.md)
  
[<span data-ttu-id="d462e-140">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="d462e-140">DeleteAttachment operation</span></span>](deleteattachment-operation.md)


- [<span data-ttu-id="d462e-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d462e-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

