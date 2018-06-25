---
title: CreateItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItemResponseMessage
api_type:
- schema
ms.assetid: 595d36c2-f87a-4d50-8e8b-f58d7641564b
description: L’élément CreateItemResponseMessage contient l’état et les résultats d’une demande d’opération CreateItem unique.
ms.openlocfilehash: 099dc799bedb527472bbe7d34cad0dbc8e98bec5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755733"
---
# <a name="createitemresponsemessage"></a><span data-ttu-id="c057e-103">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c057e-103">CreateItemResponseMessage</span></span>

<span data-ttu-id="c057e-104">L’élément **CreateItemResponseMessage** contient l’état et les résultats d’une seule demande [CreateItem operation](createitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c057e-104">The **CreateItemResponseMessage** element contains the status and result of a single [CreateItem operation](createitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="c057e-105">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="c057e-105">CreateItemResponse</span></span>](createitemresponse.md)  
- [<span data-ttu-id="c057e-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c057e-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="c057e-107">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c057e-107">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
  
```xml
<CreateItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CreateItemResponseMessage>
```

 <span data-ttu-id="c057e-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c057e-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c057e-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c057e-109">Attributes and elements</span></span>

<span data-ttu-id="c057e-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c057e-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c057e-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="c057e-111">Attributes</span></span>

|<span data-ttu-id="c057e-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="c057e-112">**Attribute**</span></span>|<span data-ttu-id="c057e-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="c057e-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c057e-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="c057e-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="c057e-115">Décrit l’état d’une réponse de [l’opération CreateItem](createitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c057e-115">Describes the status of a [CreateItem operation](createitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="c057e-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="c057e-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="c057e-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="c057e-117">-  Success</span></span>  <br/><span data-ttu-id="c057e-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="c057e-118">-  Warning</span></span>  <br/><span data-ttu-id="c057e-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="c057e-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="c057e-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c057e-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="c057e-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="c057e-121">**Value**</span></span>|<span data-ttu-id="c057e-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="c057e-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c057e-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="c057e-123">**Success**</span></span> <br/> |<span data-ttu-id="c057e-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="c057e-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="c057e-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="c057e-125">**Warning**</span></span> <br/> | <span data-ttu-id="c057e-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="c057e-126">Describes a request that was not processed.</span></span> <span data-ttu-id="c057e-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="c057e-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="c057e-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="c057e-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="c057e-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="c057e-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="c057e-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="c057e-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="c057e-131">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="c057e-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="c057e-132">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="c057e-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="c057e-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="c057e-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="c057e-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="c057e-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="c057e-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="c057e-135">**Error**</span></span> <br/> | <span data-ttu-id="c057e-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="c057e-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="c057e-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="c057e-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="c057e-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="c057e-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="c057e-139">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="c057e-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="c057e-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="c057e-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="c057e-141">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="c057e-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="c057e-142">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="c057e-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="c057e-143">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="c057e-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="c057e-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="c057e-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c057e-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c057e-145">Child elements</span></span>

|<span data-ttu-id="c057e-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c057e-146">**Element**</span></span>|<span data-ttu-id="c057e-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="c057e-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c057e-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="c057e-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c057e-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="c057e-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c057e-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c057e-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c057e-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="c057e-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="c057e-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c057e-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c057e-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="c057e-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="c057e-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="c057e-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c057e-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c057e-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c057e-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="c057e-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c057e-157">Items</span><span class="sxs-lookup"><span data-stu-id="c057e-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="c057e-158">Contient un tableau d’éléments créés.</span><span class="sxs-lookup"><span data-stu-id="c057e-158">Contains an array of created items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c057e-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c057e-159">Parent elements</span></span>

|<span data-ttu-id="c057e-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c057e-160">**Element**</span></span>|<span data-ttu-id="c057e-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="c057e-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c057e-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c057e-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c057e-163">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c057e-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c057e-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="c057e-164">Remarks</span></span>

<span data-ttu-id="c057e-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="c057e-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c057e-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c057e-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c057e-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c057e-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c057e-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c057e-168">Schema Name</span></span>  <br/> |<span data-ttu-id="c057e-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c057e-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c057e-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c057e-170">Validation File</span></span>  <br/> |<span data-ttu-id="c057e-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c057e-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c057e-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c057e-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="c057e-173">False</span><span class="sxs-lookup"><span data-stu-id="c057e-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c057e-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c057e-174">See also</span></span>

- [<span data-ttu-id="c057e-175">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="c057e-175">CreateItem operation</span></span>](createitem-operation.md)
- [<span data-ttu-id="c057e-176">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="c057e-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="c057e-177">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c057e-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

