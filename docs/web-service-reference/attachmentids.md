---
title: AttachmentIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentIds
api_type:
- schema
ms.assetid: 46ce3ad7-4b20-43ae-8c63-39f1e3c2666b
description: L’élément AttachmentIds contient un tableau d’identificateurs de pièce jointe.
ms.openlocfilehash: f205aefe6a7dc4ec208e8a96b8a6b47094aa741b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755338"
---
# <a name="attachmentids"></a><span data-ttu-id="3a131-103">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="3a131-103">AttachmentIds</span></span>

<span data-ttu-id="3a131-104">L’élément **AttachmentIds** contient un tableau d’identificateurs de pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="3a131-104">The **AttachmentIds** element contains an array of attachment identifiers.</span></span> 
  
```xml
<AttachmentIds>
   <AttachmentId Id=""/>
</AttachmentIds>
```

 <span data-ttu-id="3a131-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span><span class="sxs-lookup"><span data-stu-id="3a131-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a131-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3a131-106">Attributes and elements</span></span>

<span data-ttu-id="3a131-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3a131-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a131-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3a131-108">Attributes</span></span>

<span data-ttu-id="3a131-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3a131-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a131-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3a131-110">Child elements</span></span>

|<span data-ttu-id="3a131-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3a131-111">**Element**</span></span>|<span data-ttu-id="3a131-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3a131-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a131-113">AttachmentId (GetAttachment et DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="3a131-113">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md) <br/> |<span data-ttu-id="3a131-114">L’élément qui identifie une seule pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="3a131-114">The element that identifies a single attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a131-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3a131-115">Parent elements</span></span>

|<span data-ttu-id="3a131-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3a131-116">**Element**</span></span>|<span data-ttu-id="3a131-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="3a131-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a131-118">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="3a131-118">DeleteAttachment</span></span>](deleteattachment.md) <br/> |<span data-ttu-id="3a131-119">L’élément qui définit une requête de suppression d’une pièce jointe à partir de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a131-119">The element that defines a request to delete an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="3a131-120">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="3a131-120">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteAttachment` <br/> |
|[<span data-ttu-id="3a131-121">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="3a131-121">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="3a131-122">L’élément qui définit une demande pour obtenir une pièce jointe à partir de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a131-122">The element that defines a request to get an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="3a131-123">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="3a131-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3a131-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="3a131-124">Remarks</span></span>

<span data-ttu-id="3a131-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3a131-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a131-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3a131-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a131-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3a131-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a131-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3a131-128">Schema Name</span></span>  <br/> |<span data-ttu-id="3a131-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3a131-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a131-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3a131-130">Validation File</span></span>  <br/> |<span data-ttu-id="3a131-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3a131-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a131-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3a131-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a131-133">False</span><span class="sxs-lookup"><span data-stu-id="3a131-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a131-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3a131-134">See also</span></span>

- [<span data-ttu-id="3a131-135">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="3a131-135">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="3a131-136">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="3a131-136">GetAttachment operation</span></span>](getattachment-operation.md)

