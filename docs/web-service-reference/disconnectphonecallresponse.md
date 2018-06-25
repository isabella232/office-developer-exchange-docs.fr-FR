---
title: DisconnectPhoneCallResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisconnectPhoneCallResponse
api_type:
- schema
ms.assetid: 05041799-5b81-4b87-ada8-ce6c506ffe01
description: L’élément DisconnectPhoneCallResponse contient l’état et les résultats d’une requête DisconnectPhoneCall.
ms.openlocfilehash: 06471ea342424298a4e1d5a0562f8ed9866e26d3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755964"
---
# <a name="disconnectphonecallresponse"></a><span data-ttu-id="96190-103">DisconnectPhoneCallResponse</span><span class="sxs-lookup"><span data-stu-id="96190-103">DisconnectPhoneCallResponse</span></span>

<span data-ttu-id="96190-104">L’élément **DisconnectPhoneCallResponse** contient l’état et les résultats d’une requête **DisconnectPhoneCall** .</span><span class="sxs-lookup"><span data-stu-id="96190-104">The **DisconnectPhoneCallResponse** element contains the status and result of a single **DisconnectPhoneCall** request.</span></span> 
  
```xml
<DisconnectPhoneCallResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DisconnectPhoneCallResponse>
```

 <span data-ttu-id="96190-105">**DisconnectPhoneCallResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="96190-105">**DisconnectPhoneCallResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96190-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="96190-106">Attributes and elements</span></span>

<span data-ttu-id="96190-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="96190-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96190-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="96190-108">Attributes</span></span>

|<span data-ttu-id="96190-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="96190-109">**Attribute**</span></span>|<span data-ttu-id="96190-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="96190-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="96190-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="96190-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="96190-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="96190-112">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="96190-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="96190-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="96190-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="96190-114">-  Success</span></span>  <br/><span data-ttu-id="96190-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="96190-115">-  Warning</span></span>  <br/><span data-ttu-id="96190-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="96190-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="96190-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="96190-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="96190-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="96190-118">**Value**</span></span>|<span data-ttu-id="96190-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="96190-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="96190-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="96190-120">**Success**</span></span> <br/> |<span data-ttu-id="96190-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="96190-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="96190-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="96190-122">**Warning**</span></span> <br/> | <span data-ttu-id="96190-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="96190-123">Describes a request that was not processed.</span></span> <span data-ttu-id="96190-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="96190-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="96190-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="96190-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="96190-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="96190-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="96190-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="96190-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="96190-128">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="96190-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="96190-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="96190-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="96190-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="96190-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="96190-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="96190-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="96190-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="96190-132">**Error**</span></span> <br/> | <span data-ttu-id="96190-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="96190-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="96190-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="96190-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="96190-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="96190-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="96190-136">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="96190-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="96190-137">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="96190-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="96190-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="96190-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="96190-139">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="96190-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="96190-140">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="96190-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="96190-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="96190-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="96190-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="96190-142">Child elements</span></span>

|<span data-ttu-id="96190-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="96190-143">**Element**</span></span>|<span data-ttu-id="96190-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="96190-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96190-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="96190-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="96190-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="96190-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="96190-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="96190-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="96190-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="96190-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="96190-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="96190-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="96190-150">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="96190-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="96190-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="96190-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="96190-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="96190-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="96190-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="96190-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96190-154">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="96190-154">Parent elements</span></span>

<span data-ttu-id="96190-155">Aucun.</span><span class="sxs-lookup"><span data-stu-id="96190-155">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="96190-156">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="96190-156">Text value</span></span>

<span data-ttu-id="96190-157">Aucun.</span><span class="sxs-lookup"><span data-stu-id="96190-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96190-158">Remarques</span><span class="sxs-lookup"><span data-stu-id="96190-158">Remarks</span></span>

<span data-ttu-id="96190-159">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="96190-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96190-160">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="96190-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96190-161">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="96190-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96190-162">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="96190-162">Schema Name</span></span>  <br/> |<span data-ttu-id="96190-163">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="96190-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="96190-164">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="96190-164">Validation File</span></span>  <br/> |<span data-ttu-id="96190-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="96190-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96190-166">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="96190-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="96190-167">False</span><span class="sxs-lookup"><span data-stu-id="96190-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96190-168">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="96190-168">See also</span></span>

- [<span data-ttu-id="96190-169">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="96190-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

