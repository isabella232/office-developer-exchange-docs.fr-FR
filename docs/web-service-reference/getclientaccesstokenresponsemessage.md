---
title: GetClientAccessTokenResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 45ca2500-ceab-4c98-9576-cb9e158e5896
description: L’élément GetClientAccessTokenResponseMessage spécifie le message de réponse pour une demande GetClientAccessToken.
ms.openlocfilehash: e842353dfe91fa7df410203b53e22d5ec53e1e39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526682"
---
# <a name="getclientaccesstokenresponsemessage"></a><span data-ttu-id="31d77-103">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="31d77-103">GetClientAccessTokenResponseMessage</span></span>

<span data-ttu-id="31d77-104">L’élément **GetClientAccessTokenResponseMessage** spécifie le message de réponse pour une demande **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="31d77-104">The **GetClientAccessTokenResponseMessage** element specifies the response message for a **GetClientAccessToken** request.</span></span> 
  
```XML
<GetClientAccessTokenResponseMessage ResponseClass=" Success | Warning | Error ">
    <Token/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetClientAccessTokenResponseMessage>
```

 <span data-ttu-id="31d77-105">**GetClientAccessTokenResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="31d77-105">**GetClientAccessTokenResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31d77-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="31d77-106">Attributes and elements</span></span>

<span data-ttu-id="31d77-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="31d77-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31d77-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="31d77-108">Attributes</span></span>

|<span data-ttu-id="31d77-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="31d77-109">**Attribute**</span></span>|<span data-ttu-id="31d77-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="31d77-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="31d77-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="31d77-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="31d77-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="31d77-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="31d77-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="31d77-113">ResponseClass</span></span>

|<span data-ttu-id="31d77-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="31d77-114">**Value**</span></span>|<span data-ttu-id="31d77-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="31d77-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="31d77-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="31d77-116">Success</span></span>  <br/> |<span data-ttu-id="31d77-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="31d77-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="31d77-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="31d77-118">Warning</span></span>  <br/> |<span data-ttu-id="31d77-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="31d77-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="31d77-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="31d77-120">Error</span></span>  <br/> |<span data-ttu-id="31d77-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="31d77-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="31d77-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="31d77-122">Child elements</span></span>

|<span data-ttu-id="31d77-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="31d77-123">**Element**</span></span>|<span data-ttu-id="31d77-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="31d77-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31d77-125">Jeton (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="31d77-125">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md) <br/> |<span data-ttu-id="31d77-126">Spécifie un jeton d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="31d77-126">Specifies a client access token.</span></span>  <br/> |
|[<span data-ttu-id="31d77-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="31d77-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="31d77-128">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="31d77-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="31d77-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="31d77-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="31d77-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="31d77-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="31d77-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="31d77-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="31d77-132">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="31d77-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="31d77-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="31d77-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="31d77-134">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="31d77-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="31d77-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="31d77-135">Parent elements</span></span>

|<span data-ttu-id="31d77-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="31d77-136">**Element**</span></span>|<span data-ttu-id="31d77-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="31d77-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31d77-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="31d77-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="31d77-139">Contient les messages de réponse pour une demande de services Web Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="31d77-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="31d77-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="31d77-140">Remarks</span></span>

<span data-ttu-id="31d77-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="31d77-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="31d77-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="31d77-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31d77-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="31d77-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31d77-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="31d77-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="31d77-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="31d77-145">Schema Name</span></span>  <br/> |<span data-ttu-id="31d77-146">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="31d77-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="31d77-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="31d77-147">Validation File</span></span>  <br/> |<span data-ttu-id="31d77-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="31d77-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="31d77-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="31d77-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="31d77-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="31d77-150">See also</span></span>



- [<span data-ttu-id="31d77-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="31d77-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

