---
title: DeleteAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 43d0c1cb-92ca-4399-9b3a-acb2b5c22624
description: L’élément DeleteAttachment est l’élément racine dans une requête de suppression d’une pièce jointe à partir de la banque d’informations Exchange.
ms.openlocfilehash: 2beedd647febf025f6e3140ec37b196c9aeb7611
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755844"
---
# <a name="deleteattachment"></a><span data-ttu-id="933a1-103">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="933a1-103">DeleteAttachment</span></span>

<span data-ttu-id="933a1-104">L’élément **DeleteAttachment** est l’élément racine dans une requête de suppression d’une pièce jointe à partir de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="933a1-104">The **DeleteAttachment** element is the root element in a request to delete an attachment from the Exchange store.</span></span> 
  
```xml
<DeleteAttachment>
   <AttachmentIds/>
</DeleteAttachment>
```

<span data-ttu-id="933a1-105">**DeleteAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="933a1-105">**DeleteAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="933a1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="933a1-106">Attributes and elements</span></span>

<span data-ttu-id="933a1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="933a1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="933a1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="933a1-108">Attributes</span></span>

<span data-ttu-id="933a1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="933a1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="933a1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="933a1-110">Child elements</span></span>

|<span data-ttu-id="933a1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="933a1-111">**Element**</span></span>|<span data-ttu-id="933a1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="933a1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="933a1-113">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="933a1-113">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="933a1-114">Contient un tableau d’identificateurs de pièce jointe qui sont utilisées pour supprimer les pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="933a1-114">Contains an array of attachment identifiers that are used to delete the attachments.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="933a1-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="933a1-115">Parent elements</span></span>

<span data-ttu-id="933a1-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="933a1-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="933a1-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="933a1-117">Remarks</span></span>

<span data-ttu-id="933a1-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="933a1-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="933a1-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="933a1-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="933a1-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="933a1-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="933a1-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="933a1-121">Schema Name</span></span>  <br/> |<span data-ttu-id="933a1-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="933a1-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="933a1-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="933a1-123">Validation File</span></span>  <br/> |<span data-ttu-id="933a1-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="933a1-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="933a1-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="933a1-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="933a1-126">False</span><span class="sxs-lookup"><span data-stu-id="933a1-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="933a1-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="933a1-127">See also</span></span>

- [<span data-ttu-id="933a1-128">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="933a1-128">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

