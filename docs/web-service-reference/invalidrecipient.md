---
title: InvalidRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 9e2d3433-22d7-444b-9883-e5649297d8fe
description: L’élément InvalidRecipient contient l’adresse SMTP du destinataire non valide et plus d’informations sur la raison pour laquelle le destinataire n’est pas valide.
ms.openlocfilehash: 800056666e486e9337dcd1c2786f7e6db1e060bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827961"
---
# <a name="invalidrecipient"></a><span data-ttu-id="91ccb-103">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="91ccb-103">InvalidRecipient</span></span>

<span data-ttu-id="91ccb-104">L’élément **InvalidRecipient** contient l’adresse SMTP du destinataire non valide et plus d’informations sur la raison pour laquelle le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="91ccb-104">The **InvalidRecipient** element contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>
   <SmtpAddress/>
   <ResponseCode/>
   <MessageText/>
</InvalidRecipient>

```

 <span data-ttu-id="91ccb-105">**InvalidRecipientType**</span><span class="sxs-lookup"><span data-stu-id="91ccb-105">**InvalidRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91ccb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="91ccb-106">Attributes and elements</span></span>

<span data-ttu-id="91ccb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="91ccb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91ccb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="91ccb-108">Attributes</span></span>

<span data-ttu-id="91ccb-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="91ccb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91ccb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="91ccb-110">Child elements</span></span>

|<span data-ttu-id="91ccb-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="91ccb-111">**Element**</span></span>|<span data-ttu-id="91ccb-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="91ccb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91ccb-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="91ccb-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="91ccb-114">Contient l’adresse SMTP du destinataire non valide.</span><span class="sxs-lookup"><span data-stu-id="91ccb-114">Contains the SMTP address of the invalid recipient.</span></span> <span data-ttu-id="91ccb-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="91ccb-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="91ccb-116">ResponseCode (InvalidRecipientResponseCodeType)</span><span class="sxs-lookup"><span data-stu-id="91ccb-116">ResponseCode (InvalidRecipientResponseCodeType)</span></span>](responsecode-invalidrecipientresponsecodetype.md) <br/> |<span data-ttu-id="91ccb-117">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="91ccb-117">Provides an error code that identifies the specific error that the request encountered.</span></span> <span data-ttu-id="91ccb-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="91ccb-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="91ccb-119">MessageText</span><span class="sxs-lookup"><span data-stu-id="91ccb-119">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="91ccb-120">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="91ccb-120">Provides a text description of the status of the response.</span></span> <span data-ttu-id="91ccb-121">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="91ccb-121">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="91ccb-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="91ccb-122">Parent elements</span></span>

|<span data-ttu-id="91ccb-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="91ccb-123">**Element**</span></span>|<span data-ttu-id="91ccb-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="91ccb-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91ccb-125">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="91ccb-125">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="91ccb-126">Représente les destinataires d’un dossier de demande de partage qui ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="91ccb-126">Represents the recipients of a folder sharing request that are invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="91ccb-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="91ccb-127">Remarks</span></span>

<span data-ttu-id="91ccb-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="91ccb-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91ccb-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="91ccb-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91ccb-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="91ccb-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91ccb-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="91ccb-131">Schema Name</span></span>  <br/> |<span data-ttu-id="91ccb-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="91ccb-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="91ccb-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="91ccb-133">Validation File</span></span>  <br/> |<span data-ttu-id="91ccb-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91ccb-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91ccb-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="91ccb-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="91ccb-136">False</span><span class="sxs-lookup"><span data-stu-id="91ccb-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91ccb-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="91ccb-137">See also</span></span>



[<span data-ttu-id="91ccb-138">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="91ccb-138">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="91ccb-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="91ccb-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

