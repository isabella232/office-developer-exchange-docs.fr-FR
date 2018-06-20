---
title: GetServerTimeZonesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZonesResponseMessage
api_type:
- schema
ms.assetid: eb2592b2-144f-4c33-8df7-8e70dce7ab55
description: L’élément GetServerTimeZonesResponseMessage contient l’état et les résultats d’une demande d’opération GetServerTimeZones unique.
ms.openlocfilehash: 594b194f7c73e8880b83db6e20bb447e682a525c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827665"
---
# <a name="getservertimezonesresponsemessage"></a><span data-ttu-id="19ebc-103">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="19ebc-103">GetServerTimeZonesResponseMessage</span></span>

<span data-ttu-id="19ebc-104">L’élément **GetServerTimeZonesResponseMessage** contient l’état et les résultats d’une seule demande [d’opération GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="19ebc-104">The **GetServerTimeZonesResponseMessage** element contains the status and result of a single [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span> 
  
```XML
<GetServerTimeZonesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <TimeZoneDefinitions/>
</GetServerTimeZonesResponseMessage>
```

 <span data-ttu-id="19ebc-105">**GetServerTimeZonesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="19ebc-105">**GetServerTimeZonesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19ebc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="19ebc-106">Attributes and elements</span></span>

<span data-ttu-id="19ebc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="19ebc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19ebc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="19ebc-108">Attributes</span></span>

|<span data-ttu-id="19ebc-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="19ebc-109">**Attribute**</span></span>|<span data-ttu-id="19ebc-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="19ebc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="19ebc-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="19ebc-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="19ebc-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="19ebc-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="19ebc-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="19ebc-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="19ebc-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="19ebc-114">-  Success</span></span>  <br/><span data-ttu-id="19ebc-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="19ebc-115">-  Warning</span></span>  <br/><span data-ttu-id="19ebc-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="19ebc-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="19ebc-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="19ebc-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="19ebc-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="19ebc-118">**Value**</span></span>|<span data-ttu-id="19ebc-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="19ebc-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="19ebc-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="19ebc-120">**Success**</span></span> <br/> |<span data-ttu-id="19ebc-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="19ebc-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="19ebc-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="19ebc-122">**Warning**</span></span> <br/> | <span data-ttu-id="19ebc-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="19ebc-123">Describes a request that was not processed.</span></span> <span data-ttu-id="19ebc-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="19ebc-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="19ebc-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="19ebc-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="19ebc-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="19ebc-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="19ebc-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="19ebc-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="19ebc-128">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="19ebc-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="19ebc-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="19ebc-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="19ebc-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="19ebc-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="19ebc-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="19ebc-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="19ebc-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="19ebc-132">**Error**</span></span> <br/> | <span data-ttu-id="19ebc-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="19ebc-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="19ebc-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="19ebc-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="19ebc-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="19ebc-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="19ebc-136">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="19ebc-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="19ebc-137">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="19ebc-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="19ebc-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="19ebc-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="19ebc-139">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="19ebc-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="19ebc-140">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="19ebc-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="19ebc-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="19ebc-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="19ebc-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="19ebc-142">Child elements</span></span>

|<span data-ttu-id="19ebc-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="19ebc-143">**Element**</span></span>|<span data-ttu-id="19ebc-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="19ebc-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19ebc-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="19ebc-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="19ebc-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="19ebc-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="19ebc-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="19ebc-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="19ebc-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="19ebc-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="19ebc-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="19ebc-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="19ebc-150">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="19ebc-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="19ebc-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="19ebc-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="19ebc-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="19ebc-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="19ebc-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="19ebc-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="19ebc-154">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="19ebc-154">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="19ebc-155">Contient un tableau des définitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="19ebc-155">Contains an array of time zone definitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="19ebc-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="19ebc-156">Parent elements</span></span>

|<span data-ttu-id="19ebc-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="19ebc-157">**Element**</span></span>|<span data-ttu-id="19ebc-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="19ebc-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19ebc-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="19ebc-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="19ebc-160">Contient les messages de réponse pour une demande d’Exchange Web Services (EWS).</span><span class="sxs-lookup"><span data-stu-id="19ebc-160">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="19ebc-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="19ebc-161">Remarks</span></span>

<span data-ttu-id="19ebc-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="19ebc-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19ebc-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="19ebc-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19ebc-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="19ebc-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="19ebc-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="19ebc-165">Schema Name</span></span>  <br/> |<span data-ttu-id="19ebc-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="19ebc-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="19ebc-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="19ebc-167">Validation File</span></span>  <br/> |<span data-ttu-id="19ebc-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="19ebc-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="19ebc-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="19ebc-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="19ebc-170">False</span><span class="sxs-lookup"><span data-stu-id="19ebc-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19ebc-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="19ebc-171">See also</span></span>

- [<span data-ttu-id="19ebc-172">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="19ebc-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
