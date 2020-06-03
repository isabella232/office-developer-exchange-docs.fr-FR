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
description: L’élément ConvertIdResponseMessage contient l’État et le résultat d’une demande d’opération ConvertId.
ms.openlocfilehash: cd0154f87390be3516ced4be53f5371d4a348c49
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456219"
---
# <a name="convertidresponsemessage"></a><span data-ttu-id="0331f-103">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0331f-103">ConvertIdResponseMessage</span></span>

<span data-ttu-id="0331f-104">L’élément **ConvertIdResponseMessage** contient l’État et le résultat d’une demande d' [opération ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0331f-104">The **ConvertIdResponseMessage** element contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span> 
  
- [<span data-ttu-id="0331f-105">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="0331f-105">ConvertIdResponse</span></span>](convertidresponse.md) 
- [<span data-ttu-id="0331f-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0331f-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="0331f-107">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0331f-107">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 <span data-ttu-id="0331f-108">**ConvertIdResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0331f-108">**ConvertIdResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0331f-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0331f-109">Attributes and elements</span></span>

<span data-ttu-id="0331f-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0331f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0331f-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="0331f-111">Attributes</span></span>

|<span data-ttu-id="0331f-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="0331f-112">**Attribute**</span></span>|<span data-ttu-id="0331f-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="0331f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0331f-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0331f-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0331f-115">Décrit l’état d’une réponse d' [opération ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0331f-115">Describes the status of a [ConvertId operation](convertid-operation.md) response.</span></span><br/><br/><span data-ttu-id="0331f-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="0331f-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="0331f-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="0331f-117">- Success</span></span>  <br/><span data-ttu-id="0331f-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="0331f-118">-  Warning</span></span>  <br/><span data-ttu-id="0331f-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="0331f-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="0331f-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0331f-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="0331f-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="0331f-121">**Value**</span></span>|<span data-ttu-id="0331f-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="0331f-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0331f-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="0331f-123">**Success**</span></span> <br/> |<span data-ttu-id="0331f-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="0331f-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0331f-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="0331f-125">**Warning**</span></span> <br/> | <span data-ttu-id="0331f-126">Décrit une demande qui n’a pas été entièrement traitée ou pour laquelle un résultat inattendu s’est produit.</span><span class="sxs-lookup"><span data-stu-id="0331f-126">Describes a request that was not fully processed or for which an unintended result occurred.</span></span>  <br/> |
|<span data-ttu-id="0331f-127">**Error**</span><span class="sxs-lookup"><span data-stu-id="0331f-127">**Error**</span></span> <br/> | <span data-ttu-id="0331f-128">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="0331f-128">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="0331f-129">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="0331f-129">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0331f-130">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="0331f-130">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="0331f-131">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="0331f-131">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="0331f-132">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="0331f-132">-  An unknown tag</span></span>  <br/><span data-ttu-id="0331f-133">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="0331f-133">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="0331f-134">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="0331f-134">- An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="0331f-135">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="0331f-135">-  A server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="0331f-136">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="0331f-136">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0331f-137">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0331f-137">Child elements</span></span>

|<span data-ttu-id="0331f-138">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0331f-138">**Element**</span></span>|<span data-ttu-id="0331f-139">**Description**</span><span class="sxs-lookup"><span data-stu-id="0331f-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0331f-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="0331f-140">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0331f-141">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="0331f-141">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0331f-142">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0331f-142">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0331f-143">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="0331f-143">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0331f-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0331f-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0331f-145">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="0331f-145">Currently unused and reserved for future use.</span></span> <span data-ttu-id="0331f-146">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="0331f-146">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0331f-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0331f-147">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0331f-148">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="0331f-148">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0331f-149">AlternateId</span><span class="sxs-lookup"><span data-stu-id="0331f-149">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="0331f-150">Décrit un identificateur converti dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="0331f-150">Describes a converted identifier in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0331f-151">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0331f-151">Parent elements</span></span>

|<span data-ttu-id="0331f-152">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0331f-152">**Element**</span></span>|<span data-ttu-id="0331f-153">**Description**</span><span class="sxs-lookup"><span data-stu-id="0331f-153">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0331f-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0331f-154">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0331f-155">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0331f-155">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0331f-156">Remarques</span><span class="sxs-lookup"><span data-stu-id="0331f-156">Remarks</span></span>

<span data-ttu-id="0331f-157">Un message de réponse par identificateur converti est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="0331f-157">One response message per converted identifier is returned.</span></span> <span data-ttu-id="0331f-158">L’élément [AlternateId](alternateid.md) sera absent de la réponse si un code de réponse d’erreur est renvoyé,</span><span class="sxs-lookup"><span data-stu-id="0331f-158">The [AlternateId](alternateid.md) element will be missing from the response if an error response code is returned,</span></span> 
  
<span data-ttu-id="0331f-159">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange 2010 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0331f-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0331f-160">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0331f-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0331f-161">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0331f-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0331f-162">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0331f-162">Schema Name</span></span>  <br/> |<span data-ttu-id="0331f-163">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0331f-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0331f-164">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0331f-164">Validation File</span></span>  <br/> |<span data-ttu-id="0331f-165">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0331f-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0331f-166">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0331f-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="0331f-167">False</span><span class="sxs-lookup"><span data-stu-id="0331f-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0331f-168">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0331f-168">See also</span></span>

- [<span data-ttu-id="0331f-169">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="0331f-169">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="0331f-170">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0331f-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

