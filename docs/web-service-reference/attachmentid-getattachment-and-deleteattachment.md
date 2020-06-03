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
description: L’élément AttachmentId identifie une pièce jointe unique.
ms.openlocfilehash: 1096487490f6066f70d2da861b3015f0fbf5a68f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460854"
---
# <a name="attachmentid-getattachment-and-deleteattachment"></a><span data-ttu-id="4abcc-103">AttachmentId (GetAttachment et DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="4abcc-103">AttachmentId (GetAttachment and DeleteAttachment)</span></span>

<span data-ttu-id="4abcc-104">L’élément **attachmentid** identifie une pièce jointe unique.</span><span class="sxs-lookup"><span data-stu-id="4abcc-104">The **AttachmentId** element identifies a single attachment.</span></span> 
  
```xml
<AttachmentId Id="" />
```

 <span data-ttu-id="4abcc-105">**RequestAttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="4abcc-105">**RequestAttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4abcc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4abcc-106">Attributes and elements</span></span>

<span data-ttu-id="4abcc-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4abcc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4abcc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4abcc-108">Attributes</span></span>

|<span data-ttu-id="4abcc-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4abcc-109">**Attribute**</span></span>|<span data-ttu-id="4abcc-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="4abcc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4abcc-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="4abcc-111">**Id**</span></span> <br/> |<span data-ttu-id="4abcc-112">Spécifie l’identificateur de pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="4abcc-112">Specifies the attachment identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4abcc-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4abcc-113">Child elements</span></span>

<span data-ttu-id="4abcc-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4abcc-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4abcc-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4abcc-115">Parent elements</span></span>

|<span data-ttu-id="4abcc-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4abcc-116">**Element**</span></span>|<span data-ttu-id="4abcc-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="4abcc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4abcc-118">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="4abcc-118">AttachmentIds</span></span>](attachmentids.md) <br/> | <span data-ttu-id="4abcc-119">Contient un tableau d’identificateurs de pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="4abcc-119">Contains an array of attachment identifiers.</span></span><br/><br/>  <span data-ttu-id="4abcc-120">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="4abcc-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/DeleteAttachment/AttachmentIds`<br/><br/>`/GetAttachment/AttachmentIds` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4abcc-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="4abcc-121">Remarks</span></span>

<span data-ttu-id="4abcc-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4abcc-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4abcc-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4abcc-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4abcc-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4abcc-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4abcc-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4abcc-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4abcc-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4abcc-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="4abcc-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4abcc-127">Validation File</span></span>  <br/> |<span data-ttu-id="4abcc-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4abcc-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4abcc-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4abcc-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="4abcc-130">False</span><span class="sxs-lookup"><span data-stu-id="4abcc-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4abcc-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4abcc-131">See also</span></span>

- [<span data-ttu-id="4abcc-132">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="4abcc-132">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="4abcc-133">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="4abcc-133">GetAttachment operation</span></span>](getattachment-operation.md)

