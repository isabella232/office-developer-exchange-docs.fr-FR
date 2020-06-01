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
ms.openlocfilehash: d8badd465fd5a93e1a6354d55ac5c4b080897152
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457094"
---
# <a name="rootitemid"></a><span data-ttu-id="124a9-103">RootItemId</span><span class="sxs-lookup"><span data-stu-id="124a9-103">RootItemId</span></span>

<span data-ttu-id="124a9-104">L’élément **RootItemId** identifie l’élément racine d’une pièce jointe supprimée.</span><span class="sxs-lookup"><span data-stu-id="124a9-104">The **RootItemId** element identifies the root item of a deleted attachment.</span></span> 
  
[<span data-ttu-id="124a9-105">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="124a9-105">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
  
[<span data-ttu-id="124a9-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="124a9-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="124a9-107">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="124a9-107">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
  
[<span data-ttu-id="124a9-108">RootItemId</span><span class="sxs-lookup"><span data-stu-id="124a9-108">RootItemId</span></span>](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="124a9-109">**RootItemIdType**</span><span class="sxs-lookup"><span data-stu-id="124a9-109">**RootItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="124a9-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="124a9-110">Attributes and elements</span></span>

<span data-ttu-id="124a9-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="124a9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="124a9-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="124a9-112">Attributes</span></span>

|<span data-ttu-id="124a9-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="124a9-113">**Attribute**</span></span>|<span data-ttu-id="124a9-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="124a9-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="124a9-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="124a9-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="124a9-116">Identifie l’élément racine d’une pièce jointe supprimée.</span><span class="sxs-lookup"><span data-stu-id="124a9-116">Identifies the root item of a deleted attachment.</span></span>  <br/> |
|<span data-ttu-id="124a9-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="124a9-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="124a9-118">Identifie la nouvelle clé de modification de l’élément racine d’une pièce jointe supprimée.</span><span class="sxs-lookup"><span data-stu-id="124a9-118">Identifies the new change key of the root item of a deleted attachment.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="124a9-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="124a9-119">Child elements</span></span>

<span data-ttu-id="124a9-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="124a9-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="124a9-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="124a9-121">Parent elements</span></span>

|<span data-ttu-id="124a9-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="124a9-122">**Element**</span></span>|<span data-ttu-id="124a9-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="124a9-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="124a9-124">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="124a9-124">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md) <br/> |<span data-ttu-id="124a9-125">Contient l’État et le résultat d’une demande DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="124a9-125">Contains the status and result of a DeleteAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="124a9-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="124a9-126">Remarks</span></span>

<span data-ttu-id="124a9-127">L’élément **RootItemId** est utilisé uniquement dans les réponses DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="124a9-127">The **RootItemId** element is only used in DeleteAttachment responses.</span></span> <span data-ttu-id="124a9-128">Cela identifie l’identificateur de l’élément racine et, plus important, la nouvelle clé de modification de l’élément parent.</span><span class="sxs-lookup"><span data-stu-id="124a9-128">This identifies the root item identifier, and more importantly, the new change key to the parent item.</span></span> 
  
<span data-ttu-id="124a9-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="124a9-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="124a9-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="124a9-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="124a9-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="124a9-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="124a9-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="124a9-132">Schema name</span></span>  <br/> |<span data-ttu-id="124a9-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="124a9-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="124a9-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="124a9-134">Validation file</span></span>  <br/> |<span data-ttu-id="124a9-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="124a9-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="124a9-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="124a9-136">Can be empty</span></span>  <br/> |<span data-ttu-id="124a9-137">False</span><span class="sxs-lookup"><span data-stu-id="124a9-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="124a9-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="124a9-138">See also</span></span>



[<span data-ttu-id="124a9-139">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="124a9-139">DeleteAttachment</span></span>](deleteattachment.md)
  
[<span data-ttu-id="124a9-140">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="124a9-140">DeleteAttachment operation</span></span>](deleteattachment-operation.md)


- [<span data-ttu-id="124a9-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="124a9-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

