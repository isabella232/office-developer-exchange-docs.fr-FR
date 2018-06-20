---
title: UpdateInboxRulesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRulesResponse
api_type:
- schema
ms.assetid: 0947b6aa-0d95-421b-aebb-d03021ecc110
description: L’élément UpdateInboxRulesResponse définit une réponse à une demande de UpdateInboxRules.
ms.openlocfilehash: cd64e4546f8d9bf573062d9c982477be3fa4d925
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838882"
---
# <a name="updateinboxrulesresponse"></a><span data-ttu-id="87ffb-103">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="87ffb-103">UpdateInboxRulesResponse</span></span>

<span data-ttu-id="87ffb-104">L’élément **UpdateInboxRulesResponse** définit une réponse à une demande de UpdateInboxRules.</span><span class="sxs-lookup"><span data-stu-id="87ffb-104">The **UpdateInboxRulesResponse** element defines a response to an UpdateInboxRules request.</span></span> 
  
```XML
<UpdateInboxRulesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RuleOperationErrors/>
</UpdateInboxRulesResponse>
```

 <span data-ttu-id="87ffb-105">**UpdateInboxRulesResponseType**</span><span class="sxs-lookup"><span data-stu-id="87ffb-105">**UpdateInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87ffb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="87ffb-106">Attributes and elements</span></span>

<span data-ttu-id="87ffb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="87ffb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87ffb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="87ffb-108">Attributes</span></span>

|<span data-ttu-id="87ffb-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="87ffb-109">**Attribute**</span></span>|<span data-ttu-id="87ffb-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="87ffb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="87ffb-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="87ffb-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="87ffb-112">Décrit l’état d’une réponse de [l’opération d’annulation d’abonnement](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="87ffb-112">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span><br/><br/> <span data-ttu-id="87ffb-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="87ffb-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="87ffb-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="87ffb-114">-  Success</span></span>  <br/><span data-ttu-id="87ffb-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="87ffb-115">-  Warning</span></span>  <br/><span data-ttu-id="87ffb-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="87ffb-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="87ffb-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="87ffb-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="87ffb-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="87ffb-118">**Value**</span></span>|<span data-ttu-id="87ffb-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="87ffb-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="87ffb-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="87ffb-120">**Success**</span></span> <br/> |<span data-ttu-id="87ffb-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="87ffb-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="87ffb-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="87ffb-122">**Warning**</span></span> <br/> | <span data-ttu-id="87ffb-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="87ffb-123">Describes a request that was not processed.</span></span> <span data-ttu-id="87ffb-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="87ffb-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="87ffb-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="87ffb-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="87ffb-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="87ffb-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="87ffb-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="87ffb-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="87ffb-128">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="87ffb-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="87ffb-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="87ffb-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="87ffb-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="87ffb-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="87ffb-131">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="87ffb-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="87ffb-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="87ffb-132">**Error**</span></span> <br/> | <span data-ttu-id="87ffb-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="87ffb-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="87ffb-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="87ffb-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="87ffb-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="87ffb-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="87ffb-136">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="87ffb-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="87ffb-137">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="87ffb-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="87ffb-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="87ffb-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="87ffb-139">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="87ffb-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="87ffb-140">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="87ffb-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="87ffb-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="87ffb-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="87ffb-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="87ffb-142">Child elements</span></span>

|<span data-ttu-id="87ffb-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="87ffb-143">**Element**</span></span>|<span data-ttu-id="87ffb-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="87ffb-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87ffb-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="87ffb-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="87ffb-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="87ffb-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="87ffb-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="87ffb-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="87ffb-148">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="87ffb-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="87ffb-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="87ffb-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="87ffb-150">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="87ffb-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="87ffb-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="87ffb-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="87ffb-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="87ffb-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="87ffb-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="87ffb-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="87ffb-154">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="87ffb-154">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="87ffb-155">Représente un tableau règle des erreurs de validation sur chaque champ de règle qui comporte une erreur.</span><span class="sxs-lookup"><span data-stu-id="87ffb-155">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="87ffb-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="87ffb-156">Parent elements</span></span>

<span data-ttu-id="87ffb-157">Aucun.</span><span class="sxs-lookup"><span data-stu-id="87ffb-157">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="87ffb-158">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="87ffb-158">Text value</span></span>

<span data-ttu-id="87ffb-159">Aucun.</span><span class="sxs-lookup"><span data-stu-id="87ffb-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="87ffb-160">Remarques</span><span class="sxs-lookup"><span data-stu-id="87ffb-160">Remarks</span></span>

<span data-ttu-id="87ffb-161">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="87ffb-161">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87ffb-162">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="87ffb-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87ffb-163">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="87ffb-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="87ffb-164">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="87ffb-164">Schema name</span></span>  <br/> |<span data-ttu-id="87ffb-165">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="87ffb-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="87ffb-166">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="87ffb-166">Validation file</span></span>  <br/> |<span data-ttu-id="87ffb-167">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="87ffb-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="87ffb-168">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="87ffb-168">Can be empty</span></span>  <br/> |<span data-ttu-id="87ffb-169">False</span><span class="sxs-lookup"><span data-stu-id="87ffb-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87ffb-170">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="87ffb-170">See also</span></span>

- [<span data-ttu-id="87ffb-171">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="87ffb-171">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="87ffb-172">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="87ffb-172">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="87ffb-173">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="87ffb-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

