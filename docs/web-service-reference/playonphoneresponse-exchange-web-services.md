---
title: PlayOnPhoneResponse (Exchange Web Services)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 578b70d1-dc9d-4bce-b859-0109b2d2bcec
description: L’élément PlayOnPhoneResponse spécifie la réponse à une demande de lire un message vocal sur le téléphone.
ms.openlocfilehash: 203309bdd6d17b1c78054e673f8a340c2f069b38
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828831"
---
# <a name="playonphoneresponse-exchange-web-services"></a><span data-ttu-id="27ce9-103">PlayOnPhoneResponse (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="27ce9-103">PlayOnPhoneResponse (Exchange Web Services)</span></span>

<span data-ttu-id="27ce9-104">L’élément **PlayOnPhoneResponse** spécifie la réponse à une demande de lire un message vocal sur le téléphone.</span><span class="sxs-lookup"><span data-stu-id="27ce9-104">The **PlayOnPhoneResponse** element specifies the response to a request to play a voice mail over the telephone.</span></span> 
  
```xml
<PlayOnPhoneResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <PhoneCallId/>
</PlayOnPhoneResponse>
```

 <span data-ttu-id="27ce9-105">**PlayOnPhoneResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="27ce9-105">**PlayOnPhoneResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27ce9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="27ce9-106">Attributes and elements</span></span>

<span data-ttu-id="27ce9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="27ce9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27ce9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="27ce9-108">Attributes</span></span>

|<span data-ttu-id="27ce9-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="27ce9-109">**Attribute**</span></span>|<span data-ttu-id="27ce9-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="27ce9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="27ce9-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="27ce9-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="27ce9-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="27ce9-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="27ce9-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="27ce9-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="27ce9-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="27ce9-114">-  Success</span></span>  <br/><span data-ttu-id="27ce9-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="27ce9-115">-  Warning</span></span>  <br/><span data-ttu-id="27ce9-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="27ce9-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="27ce9-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="27ce9-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="27ce9-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="27ce9-118">**Value**</span></span>|<span data-ttu-id="27ce9-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="27ce9-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="27ce9-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="27ce9-120">**Success**</span></span> <br/> |<span data-ttu-id="27ce9-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="27ce9-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="27ce9-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="27ce9-122">**Warning**</span></span> <br/> | <span data-ttu-id="27ce9-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="27ce9-123">Describes a request that was not processed.</span></span> <span data-ttu-id="27ce9-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="27ce9-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="27ce9-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="27ce9-125">The following are examples of sources of warnings:</span></span> <br/><br/><span data-ttu-id="27ce9-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="27ce9-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="27ce9-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="27ce9-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="27ce9-128">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="27ce9-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="27ce9-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="27ce9-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="27ce9-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="27ce9-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="27ce9-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="27ce9-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="27ce9-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="27ce9-132">**Error**</span></span> <br/> | <span data-ttu-id="27ce9-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="27ce9-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="27ce9-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="27ce9-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="27ce9-135">-Non valide attributs ou éléments.</span><span class="sxs-lookup"><span data-stu-id="27ce9-135">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="27ce9-136">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="27ce9-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="27ce9-137">-Une balise inconnue.</span><span class="sxs-lookup"><span data-stu-id="27ce9-137">-  An unknown tag.</span></span>  <br/><span data-ttu-id="27ce9-138">-Un attribut ou un élément qui n’est pas valide dans le contexte.</span><span class="sxs-lookup"><span data-stu-id="27ce9-138">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="27ce9-139">-Une tentative d’accès non autorisé par n’importe quel client.</span><span class="sxs-lookup"><span data-stu-id="27ce9-139">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="27ce9-140">-Une panne côté serveur en réponse à un appel côté client valid.</span><span class="sxs-lookup"><span data-stu-id="27ce9-140">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="27ce9-141">Vous trouverez plus d’informations sur l’erreur dans les rubriques d’éléments [MessageText](messagetext.md) [ResponseCode](responsecode.md) .</span><span class="sxs-lookup"><span data-stu-id="27ce9-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) element topics.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="27ce9-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="27ce9-142">Child elements</span></span>

|<span data-ttu-id="27ce9-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="27ce9-143">**Element**</span></span>|<span data-ttu-id="27ce9-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="27ce9-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27ce9-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="27ce9-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="27ce9-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="27ce9-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="27ce9-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="27ce9-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="27ce9-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="27ce9-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="27ce9-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="27ce9-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="27ce9-150">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="27ce9-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="27ce9-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="27ce9-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="27ce9-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="27ce9-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="27ce9-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="27ce9-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="27ce9-154">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="27ce9-154">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="27ce9-155">Spécifie l’identificateur de l’appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="27ce9-155">Specifies the telephone call identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27ce9-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="27ce9-156">Parent elements</span></span>

<span data-ttu-id="27ce9-157">Aucun.</span><span class="sxs-lookup"><span data-stu-id="27ce9-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="27ce9-158">Remarques</span><span class="sxs-lookup"><span data-stu-id="27ce9-158">Remarks</span></span>

<span data-ttu-id="27ce9-159">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="27ce9-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27ce9-160">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="27ce9-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27ce9-161">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="27ce9-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27ce9-162">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="27ce9-162">Schema Name</span></span>  <br/> |<span data-ttu-id="27ce9-163">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="27ce9-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="27ce9-164">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="27ce9-164">Validation File</span></span>  <br/> |<span data-ttu-id="27ce9-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="27ce9-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27ce9-166">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="27ce9-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="27ce9-167">False</span><span class="sxs-lookup"><span data-stu-id="27ce9-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27ce9-168">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="27ce9-168">See also</span></span>

- [<span data-ttu-id="27ce9-169">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="27ce9-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

