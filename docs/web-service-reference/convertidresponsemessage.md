---
title: ConvertIdResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponseMessage
api_type:
- schema
ms.assetid: 7a439cae-0268-4328-9ded-af56ad642227
description: L’élément ConvertIdResponseMessage contient l’état et les résultats d’une demande d’opération ConvertId.
ms.openlocfilehash: 6668c0b3254191ca628413bae5ff957c3cb95b5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755663"
---
# <a name="convertidresponsemessage"></a><span data-ttu-id="a0dcf-103">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a0dcf-103">ConvertIdResponseMessage</span></span>

<span data-ttu-id="a0dcf-104">L’élément **ConvertIdResponseMessage** contient l’état et les résultats d’une demande [d’opération ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a0dcf-104">The **ConvertIdResponseMessage** element contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span> 
  
- [<span data-ttu-id="a0dcf-105">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="a0dcf-105">ConvertIdResponse</span></span>](convertidresponse.md) 
- [<span data-ttu-id="a0dcf-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a0dcf-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="a0dcf-107">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a0dcf-107">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 <span data-ttu-id="a0dcf-108">**ConvertIdResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-108">**ConvertIdResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0dcf-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a0dcf-109">Attributes and elements</span></span>

<span data-ttu-id="a0dcf-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0dcf-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="a0dcf-111">Attributes</span></span>

|<span data-ttu-id="a0dcf-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-112">**Attribute**</span></span>|<span data-ttu-id="a0dcf-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0dcf-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a0dcf-115">Décrit l’état d’une réponse de [l’opération ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a0dcf-115">Describes the status of a [ConvertId operation](convertid-operation.md) response.</span></span><br/><br/><span data-ttu-id="a0dcf-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="a0dcf-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="a0dcf-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="a0dcf-117">- Success</span></span>  <br/><span data-ttu-id="a0dcf-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="a0dcf-118">-  Warning</span></span>  <br/><span data-ttu-id="a0dcf-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="a0dcf-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="a0dcf-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a0dcf-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="a0dcf-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-121">**Value**</span></span>|<span data-ttu-id="a0dcf-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0dcf-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-123">**Success**</span></span> <br/> |<span data-ttu-id="a0dcf-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a0dcf-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-125">**Warning**</span></span> <br/> | <span data-ttu-id="a0dcf-126">Décrit une demande qui n’a pas été entièrement traité ou pour lesquelles un résultat inattendu s’est produite.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-126">Describes a request that was not fully processed or for which an unintended result occurred.</span></span>  <br/> |
|<span data-ttu-id="a0dcf-127">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-127">**Error**</span></span> <br/> | <span data-ttu-id="a0dcf-128">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-128">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="a0dcf-129">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="a0dcf-129">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="a0dcf-130">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="a0dcf-130">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="a0dcf-131">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="a0dcf-131">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="a0dcf-132">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="a0dcf-132">-  An unknown tag</span></span>  <br/><span data-ttu-id="a0dcf-133">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="a0dcf-133">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="a0dcf-134">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="a0dcf-134">- An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="a0dcf-135">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="a0dcf-135">-  A server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="a0dcf-136">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="a0dcf-136">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a0dcf-137">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a0dcf-137">Child elements</span></span>

|<span data-ttu-id="a0dcf-138">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-138">**Element**</span></span>|<span data-ttu-id="a0dcf-139">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0dcf-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="a0dcf-140">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a0dcf-141">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-141">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a0dcf-142">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a0dcf-142">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a0dcf-143">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-143">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="a0dcf-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a0dcf-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a0dcf-145">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-145">Currently unused and reserved for future use.</span></span> <span data-ttu-id="a0dcf-146">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-146">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a0dcf-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a0dcf-147">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a0dcf-148">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-148">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a0dcf-149">AlternateId</span><span class="sxs-lookup"><span data-stu-id="a0dcf-149">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="a0dcf-150">Décrit un identificateur converti dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-150">Describes a converted identifier in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a0dcf-151">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a0dcf-151">Parent elements</span></span>

|<span data-ttu-id="a0dcf-152">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-152">**Element**</span></span>|<span data-ttu-id="a0dcf-153">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0dcf-153">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0dcf-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a0dcf-154">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a0dcf-155">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-155">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a0dcf-156">Remarques</span><span class="sxs-lookup"><span data-stu-id="a0dcf-156">Remarks</span></span>

<span data-ttu-id="a0dcf-157">Un message de réponse par identificateur converti est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-157">One response message per converted identifier is returned.</span></span> <span data-ttu-id="a0dcf-158">L’élément [AlternateId](alternateid.md) sera absent de la réponse si un code d’erreur est renvoyé,</span><span class="sxs-lookup"><span data-stu-id="a0dcf-158">The [AlternateId](alternateid.md) element will be missing from the response if an error response code is returned,</span></span> 
  
<span data-ttu-id="a0dcf-159">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="a0dcf-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0dcf-160">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a0dcf-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0dcf-161">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a0dcf-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a0dcf-162">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a0dcf-162">Schema Name</span></span>  <br/> |<span data-ttu-id="a0dcf-163">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a0dcf-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a0dcf-164">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a0dcf-164">Validation File</span></span>  <br/> |<span data-ttu-id="a0dcf-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a0dcf-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a0dcf-166">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a0dcf-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0dcf-167">False</span><span class="sxs-lookup"><span data-stu-id="a0dcf-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0dcf-168">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a0dcf-168">See also</span></span>

- [<span data-ttu-id="a0dcf-169">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="a0dcf-169">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="a0dcf-170">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a0dcf-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

