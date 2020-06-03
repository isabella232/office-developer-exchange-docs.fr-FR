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
description: L’élément AttachmentIds contient un tableau d’identificateurs de pièces jointes.
ms.openlocfilehash: cff1cb5658690fd6dd2c6a7812e1f600a4c80e29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464251"
---
# <a name="attachmentids"></a><span data-ttu-id="ac9dd-103">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="ac9dd-103">AttachmentIds</span></span>

<span data-ttu-id="ac9dd-104">L’élément **AttachmentIds** contient un tableau d’identificateurs de pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="ac9dd-104">The **AttachmentIds** element contains an array of attachment identifiers.</span></span> 
  
```xml
<AttachmentIds>
   <AttachmentId Id=""/>
</AttachmentIds>
```

 <span data-ttu-id="ac9dd-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span><span class="sxs-lookup"><span data-stu-id="ac9dd-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac9dd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ac9dd-106">Attributes and elements</span></span>

<span data-ttu-id="ac9dd-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ac9dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac9dd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ac9dd-108">Attributes</span></span>

<span data-ttu-id="ac9dd-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ac9dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac9dd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ac9dd-110">Child elements</span></span>

|<span data-ttu-id="ac9dd-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ac9dd-111">**Element**</span></span>|<span data-ttu-id="ac9dd-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ac9dd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac9dd-113">AttachmentId (GetAttachment et DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="ac9dd-113">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md) <br/> |<span data-ttu-id="ac9dd-114">Élément qui identifie une pièce jointe unique.</span><span class="sxs-lookup"><span data-stu-id="ac9dd-114">The element that identifies a single attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ac9dd-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ac9dd-115">Parent elements</span></span>

|<span data-ttu-id="ac9dd-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ac9dd-116">**Element**</span></span>|<span data-ttu-id="ac9dd-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ac9dd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac9dd-118">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="ac9dd-118">DeleteAttachment</span></span>](deleteattachment.md) <br/> |<span data-ttu-id="ac9dd-119">Élément qui définit une demande de suppression d’une pièce jointe de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac9dd-119">The element that defines a request to delete an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="ac9dd-120">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="ac9dd-120">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteAttachment` <br/> |
|[<span data-ttu-id="ac9dd-121">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ac9dd-121">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="ac9dd-122">Élément qui définit une demande d’obtention d’une pièce jointe à partir de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac9dd-122">The element that defines a request to get an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="ac9dd-123">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="ac9dd-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ac9dd-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="ac9dd-124">Remarks</span></span>

<span data-ttu-id="ac9dd-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ac9dd-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac9dd-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ac9dd-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac9dd-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ac9dd-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ac9dd-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ac9dd-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ac9dd-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ac9dd-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ac9dd-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ac9dd-130">Validation File</span></span>  <br/> |<span data-ttu-id="ac9dd-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ac9dd-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ac9dd-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ac9dd-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ac9dd-133">False</span><span class="sxs-lookup"><span data-stu-id="ac9dd-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac9dd-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ac9dd-134">See also</span></span>

- [<span data-ttu-id="ac9dd-135">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="ac9dd-135">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="ac9dd-136">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ac9dd-136">GetAttachment operation</span></span>](getattachment-operation.md)

