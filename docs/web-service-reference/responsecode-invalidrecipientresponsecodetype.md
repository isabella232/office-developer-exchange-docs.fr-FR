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
ms.openlocfilehash: d78de64de7725007ec51a55dad13d1cc892a25e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529720"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a><span data-ttu-id="a7042-103">ResponseCode (InvalidRecipientResponseCodeType)</span><span class="sxs-lookup"><span data-stu-id="a7042-103">ResponseCode (InvalidRecipientResponseCodeType)</span></span>

<span data-ttu-id="a7042-104">L’élément **ResponseCode** fournit des informations sur la raison pour laquelle le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="a7042-104">The **ResponseCode** element provides information about why the recipient is invalid.</span></span> 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 <span data-ttu-id="a7042-105">**InvalidRecipientResponseCodeType**</span><span class="sxs-lookup"><span data-stu-id="a7042-105">**InvalidRecipientResponseCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7042-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a7042-106">Attributes and elements</span></span>

<span data-ttu-id="a7042-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a7042-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7042-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a7042-108">Attributes</span></span>

<span data-ttu-id="a7042-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a7042-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7042-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a7042-110">Child elements</span></span>

<span data-ttu-id="a7042-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a7042-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a7042-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a7042-112">Parent elements</span></span>

|<span data-ttu-id="a7042-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a7042-113">**Element**</span></span>|<span data-ttu-id="a7042-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7042-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7042-115">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="a7042-115">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="a7042-116">Contient l'adresse SMTP du destinataire non valide et plus d'informations sur la raison pour laquelle le destinataire n'est pas valide.</span><span class="sxs-lookup"><span data-stu-id="a7042-116">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a7042-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a7042-117">Text value</span></span>

<span data-ttu-id="a7042-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **ResponseCode** .</span><span class="sxs-lookup"><span data-stu-id="a7042-118">The following table lists the possible values for the **ResponseCode** element.</span></span> 
  
|<span data-ttu-id="a7042-119">**Code**</span><span class="sxs-lookup"><span data-stu-id="a7042-119">**Code**</span></span>|<span data-ttu-id="a7042-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7042-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7042-121">OtherError</span><span class="sxs-lookup"><span data-stu-id="a7042-121">OtherError</span></span>  <br/> |<span data-ttu-id="a7042-122">Indique que l’erreur n’est pas spécifiée par un autre code de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="a7042-122">Indicates that the error is not specified by another error response code.</span></span>  <br/> |
|<span data-ttu-id="a7042-123">RecipientOrganizationNotFederated</span><span class="sxs-lookup"><span data-stu-id="a7042-123">RecipientOrganizationNotFederated</span></span>  <br/> |<span data-ttu-id="a7042-124">Indique qu’une relation de partage n’est pas disponible pour l’organisation spécifiée dans l’adresse de messagerie SMTP du destinataire.</span><span class="sxs-lookup"><span data-stu-id="a7042-124">Indicates that a sharing relationship is not available with the organization specified in the recipient's SMTP e-mail address.</span></span>  <br/> |
|<span data-ttu-id="a7042-125">CannotObtainTokenFromSTS</span><span class="sxs-lookup"><span data-stu-id="a7042-125">CannotObtainTokenFromSTS</span></span>  <br/> |<span data-ttu-id="a7042-126">Indique qu’un problème est survenu lors de l’obtention d’un jeton de sécurité à partir du serveur de jetons.</span><span class="sxs-lookup"><span data-stu-id="a7042-126">Indicates that there was a problem obtaining a security token from the token server.</span></span>  <br/> |
|<span data-ttu-id="a7042-127">SystemPolicyBlocksSharingWithThisRecipient</span><span class="sxs-lookup"><span data-stu-id="a7042-127">SystemPolicyBlocksSharingWithThisRecipient</span></span>  <br/> |<span data-ttu-id="a7042-128">Indique que l’administrateur système a défini une stratégie système qui bloque le partage avec le destinataire spécifié.</span><span class="sxs-lookup"><span data-stu-id="a7042-128">Indicates that the system administrator has set a system policy that blocks sharing with the specified recipient.</span></span>  <br/> |
|<span data-ttu-id="a7042-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span><span class="sxs-lookup"><span data-stu-id="a7042-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span></span>  <br/> |<span data-ttu-id="a7042-130">Indique que le service d’émission de jeton de sécurité utilisé par le destinataire spécifié est inconnu.</span><span class="sxs-lookup"><span data-stu-id="a7042-130">Indicates that the secure token service that is used by the specified recipient is unknown.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a7042-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="a7042-131">Remarks</span></span>

<span data-ttu-id="a7042-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7042-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7042-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a7042-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7042-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a7042-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7042-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a7042-135">Schema Name</span></span>  <br/> |<span data-ttu-id="a7042-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a7042-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7042-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a7042-137">Validation File</span></span>  <br/> |<span data-ttu-id="a7042-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a7042-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7042-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a7042-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7042-140">False</span><span class="sxs-lookup"><span data-stu-id="a7042-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7042-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a7042-141">See also</span></span>



[<span data-ttu-id="a7042-142">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="a7042-142">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="a7042-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a7042-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

