---
title: InvalidRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipients
api_type:
- schema
ms.assetid: e4e7b50e-2fa9-4649-94a6-6002f341ecc4
description: L'élément InvalidRecipients représente les destinataires d'un dossier de demande de partage qui ne sont pas valides.
ms.openlocfilehash: 02ad8935bde347c563875bf5bfb31968b70d81b6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827966"
---
# <a name="invalidrecipients"></a><span data-ttu-id="65dc6-103">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="65dc6-103">InvalidRecipients</span></span>

<span data-ttu-id="65dc6-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **InvalidRecipients** représente les destinataires d'un dossier de demande de partage qui ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="65dc6-104">The **InvalidRecipients** element represents the recipients of a folder sharing request that are invalid.</span></span> 
  
```XML
<InvalidRecipients>
   <InvalidRecipient/>
</InvalidRecipients>
```

 <span data-ttu-id="65dc6-105">**ArrayOfInvalidRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="65dc6-105">**ArrayOfInvalidRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65dc6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="65dc6-106">Attributes and elements</span></span>

<span data-ttu-id="65dc6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="65dc6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65dc6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="65dc6-108">Attributes</span></span>

<span data-ttu-id="65dc6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="65dc6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65dc6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="65dc6-110">Child elements</span></span>

|<span data-ttu-id="65dc6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65dc6-111">**Element**</span></span>|<span data-ttu-id="65dc6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="65dc6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65dc6-113">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="65dc6-113">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="65dc6-114">Contient l'adresse SMTP du destinataire non valide et plus d'informations sur la raison pour laquelle le destinataire n'est pas valide.</span><span class="sxs-lookup"><span data-stu-id="65dc6-114">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65dc6-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="65dc6-115">Parent elements</span></span>

|<span data-ttu-id="65dc6-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65dc6-116">**Element**</span></span>|<span data-ttu-id="65dc6-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="65dc6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65dc6-118">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="65dc6-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="65dc6-119">Définit une réponse à une demande de [Opération de GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="65dc6-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="65dc6-120">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="65dc6-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="65dc6-121">Contient l'état et les résultats d'une demande unique [Opération de GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="65dc6-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="65dc6-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="65dc6-122">Remarks</span></span>

<span data-ttu-id="65dc6-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="65dc6-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65dc6-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="65dc6-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65dc6-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="65dc6-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="65dc6-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="65dc6-126">Schema Name</span></span>  <br/> |<span data-ttu-id="65dc6-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="65dc6-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="65dc6-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="65dc6-128">Validation File</span></span>  <br/> |<span data-ttu-id="65dc6-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="65dc6-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="65dc6-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="65dc6-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="65dc6-131">False</span><span class="sxs-lookup"><span data-stu-id="65dc6-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65dc6-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65dc6-132">See also</span></span>



[<span data-ttu-id="65dc6-133">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="65dc6-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="65dc6-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="65dc6-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

