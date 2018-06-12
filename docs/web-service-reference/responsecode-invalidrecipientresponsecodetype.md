---
title: ResponseCode (InvalidRecipientResponseCodeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: L’élément ResponseCode fournit des informations sur la raison pour laquelle le destinataire n’est pas valide.
ms.openlocfilehash: 3bff99dd1ac6603ce31d5ceb074e73ef48190bb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829186"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a><span data-ttu-id="460b4-103">ResponseCode (InvalidRecipientResponseCodeType)</span><span class="sxs-lookup"><span data-stu-id="460b4-103">ResponseCode (InvalidRecipientResponseCodeType)</span></span>

<span data-ttu-id="460b4-104">L’élément **ResponseCode** fournit des informations sur la raison pour laquelle le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="460b4-104">The **ResponseCode** element provides information about why the recipient is invalid.</span></span> 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 <span data-ttu-id="460b4-105">**InvalidRecipientResponseCodeType**</span><span class="sxs-lookup"><span data-stu-id="460b4-105">**InvalidRecipientResponseCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="460b4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="460b4-106">Attributes and elements</span></span>

<span data-ttu-id="460b4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="460b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="460b4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="460b4-108">Attributes</span></span>

<span data-ttu-id="460b4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="460b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="460b4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="460b4-110">Child elements</span></span>

<span data-ttu-id="460b4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="460b4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="460b4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="460b4-112">Parent elements</span></span>

|<span data-ttu-id="460b4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="460b4-113">**Element**</span></span>|<span data-ttu-id="460b4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="460b4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="460b4-115">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="460b4-115">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="460b4-116">Contient l'adresse SMTP du destinataire non valide et plus d'informations sur la raison pour laquelle le destinataire n'est pas valide.</span><span class="sxs-lookup"><span data-stu-id="460b4-116">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="460b4-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="460b4-117">Text value</span></span>

<span data-ttu-id="460b4-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **ResponseCode** .</span><span class="sxs-lookup"><span data-stu-id="460b4-118">The following table lists the possible values for the **ResponseCode** element.</span></span> 
  
|<span data-ttu-id="460b4-119">**Code**</span><span class="sxs-lookup"><span data-stu-id="460b4-119">**Code**</span></span>|<span data-ttu-id="460b4-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="460b4-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="460b4-121">OtherError</span><span class="sxs-lookup"><span data-stu-id="460b4-121">OtherError</span></span>  <br/> |<span data-ttu-id="460b4-122">Indique que l’erreur n’est pas spécifié par un autre code d’erreur.</span><span class="sxs-lookup"><span data-stu-id="460b4-122">Indicates that the error is not specified by another error response code.</span></span>  <br/> |
|<span data-ttu-id="460b4-123">RecipientOrganizationNotFederated</span><span class="sxs-lookup"><span data-stu-id="460b4-123">RecipientOrganizationNotFederated</span></span>  <br/> |<span data-ttu-id="460b4-124">Indique qu’une relation de partage n’est pas disponible avec l’organisation spécifiée dans l’adresse de messagerie SMTP du destinataire.</span><span class="sxs-lookup"><span data-stu-id="460b4-124">Indicates that a sharing relationship is not available with the organization specified in the recipient's SMTP e-mail address.</span></span>  <br/> |
|<span data-ttu-id="460b4-125">CannotObtainTokenFromSTS</span><span class="sxs-lookup"><span data-stu-id="460b4-125">CannotObtainTokenFromSTS</span></span>  <br/> |<span data-ttu-id="460b4-126">Indique qu’il y a un problème d’obtention d’un jeton de sécurité à partir du serveur d’émission de jeton.</span><span class="sxs-lookup"><span data-stu-id="460b4-126">Indicates that there was a problem obtaining a security token from the token server.</span></span>  <br/> |
|<span data-ttu-id="460b4-127">SystemPolicyBlocksSharingWithThisRecipient</span><span class="sxs-lookup"><span data-stu-id="460b4-127">SystemPolicyBlocksSharingWithThisRecipient</span></span>  <br/> |<span data-ttu-id="460b4-128">Indique que l’administrateur système a défini une stratégie système qui bloque le partage avec le destinataire spécifié.</span><span class="sxs-lookup"><span data-stu-id="460b4-128">Indicates that the system administrator has set a system policy that blocks sharing with the specified recipient.</span></span>  <br/> |
|<span data-ttu-id="460b4-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span><span class="sxs-lookup"><span data-stu-id="460b4-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span></span>  <br/> |<span data-ttu-id="460b4-130">Indique que le service de jeton de sécurité utilisé par le destinataire spécifié est inconnu.</span><span class="sxs-lookup"><span data-stu-id="460b4-130">Indicates that the secure token service that is used by the specified recipient is unknown.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="460b4-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="460b4-131">Remarks</span></span>

<span data-ttu-id="460b4-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="460b4-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="460b4-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="460b4-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="460b4-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="460b4-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="460b4-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="460b4-135">Schema Name</span></span>  <br/> |<span data-ttu-id="460b4-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="460b4-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="460b4-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="460b4-137">Validation File</span></span>  <br/> |<span data-ttu-id="460b4-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="460b4-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="460b4-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="460b4-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="460b4-140">False</span><span class="sxs-lookup"><span data-stu-id="460b4-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="460b4-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="460b4-141">See also</span></span>



[<span data-ttu-id="460b4-142">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="460b4-142">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="460b4-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="460b4-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

