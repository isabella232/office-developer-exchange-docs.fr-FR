---
title: AttachmentId (GetAttachment et DeleteAttachment)
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
ms.assetid: 4bea1cb5-0a0f-4e14-9b09-f91af8cf9899
description: L’élément AttachmentId identifie une seule pièce jointe.
ms.openlocfilehash: b0355b4a387c65e97fe973a1667e6b0a517ebf7e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755337"
---
# <a name="attachmentid-getattachment-and-deleteattachment"></a><span data-ttu-id="7ba4f-103">AttachmentId (GetAttachment et DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="7ba4f-103">AttachmentId (GetAttachment and DeleteAttachment)</span></span>

<span data-ttu-id="7ba4f-104">L’élément **AttachmentId** identifie une seule pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="7ba4f-104">The **AttachmentId** element identifies a single attachment.</span></span> 
  
```xml
<AttachmentId Id="" />
```

 <span data-ttu-id="7ba4f-105">**RequestAttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="7ba4f-105">**RequestAttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ba4f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7ba4f-106">Attributes and elements</span></span>

<span data-ttu-id="7ba4f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7ba4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ba4f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7ba4f-108">Attributes</span></span>

|<span data-ttu-id="7ba4f-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7ba4f-109">**Attribute**</span></span>|<span data-ttu-id="7ba4f-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="7ba4f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7ba4f-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="7ba4f-111">**Id**</span></span> <br/> |<span data-ttu-id="7ba4f-112">Spécifie l’identificateur de pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="7ba4f-112">Specifies the attachment identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7ba4f-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7ba4f-113">Child elements</span></span>

<span data-ttu-id="7ba4f-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7ba4f-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7ba4f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7ba4f-115">Parent elements</span></span>

|<span data-ttu-id="7ba4f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7ba4f-116">**Element**</span></span>|<span data-ttu-id="7ba4f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7ba4f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ba4f-118">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="7ba4f-118">AttachmentIds</span></span>](attachmentids.md) <br/> | <span data-ttu-id="7ba4f-119">Contient un tableau d’identificateurs de pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="7ba4f-119">Contains an array of attachment identifiers.</span></span><br/><br/>  <span data-ttu-id="7ba4f-120">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="7ba4f-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/DeleteAttachment/AttachmentIds`<br/><br/>`/GetAttachment/AttachmentIds` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ba4f-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="7ba4f-121">Remarks</span></span>

<span data-ttu-id="7ba4f-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7ba4f-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ba4f-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7ba4f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ba4f-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7ba4f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ba4f-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7ba4f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="7ba4f-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7ba4f-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ba4f-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7ba4f-127">Validation File</span></span>  <br/> |<span data-ttu-id="7ba4f-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7ba4f-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ba4f-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7ba4f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="7ba4f-130">False</span><span class="sxs-lookup"><span data-stu-id="7ba4f-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ba4f-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7ba4f-131">See also</span></span>

- [<span data-ttu-id="7ba4f-132">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="7ba4f-132">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="7ba4f-133">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="7ba4f-133">GetAttachment operation</span></span>](getattachment-operation.md)

