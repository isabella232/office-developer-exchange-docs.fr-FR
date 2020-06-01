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
description: L’élément UpdateInboxRulesResponse définit une réponse à une demande UpdateInboxRules.
ms.openlocfilehash: 1216a32bdaf2dd5211021add0728844eb62089ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455904"
---
# <a name="updateinboxrulesresponse"></a><span data-ttu-id="7cb37-103">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="7cb37-103">UpdateInboxRulesResponse</span></span>

<span data-ttu-id="7cb37-104">L’élément **UpdateInboxRulesResponse** définit une réponse à une demande UpdateInboxRules.</span><span class="sxs-lookup"><span data-stu-id="7cb37-104">The **UpdateInboxRulesResponse** element defines a response to an UpdateInboxRules request.</span></span> 
  
```XML
<UpdateInboxRulesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RuleOperationErrors/>
</UpdateInboxRulesResponse>
```

 <span data-ttu-id="7cb37-105">**UpdateInboxRulesResponseType**</span><span class="sxs-lookup"><span data-stu-id="7cb37-105">**UpdateInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7cb37-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7cb37-106">Attributes and elements</span></span>

<span data-ttu-id="7cb37-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7cb37-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cb37-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7cb37-108">Attributes</span></span>

|<span data-ttu-id="7cb37-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7cb37-109">**Attribute**</span></span>|<span data-ttu-id="7cb37-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="7cb37-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7cb37-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="7cb37-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="7cb37-112">Décrit l’état d’une réponse d' [opération de résiliation](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7cb37-112">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span><br/><br/> <span data-ttu-id="7cb37-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="7cb37-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="7cb37-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="7cb37-114">-  Success</span></span>  <br/><span data-ttu-id="7cb37-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="7cb37-115">-  Warning</span></span>  <br/><span data-ttu-id="7cb37-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="7cb37-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="7cb37-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7cb37-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="7cb37-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="7cb37-118">**Value**</span></span>|<span data-ttu-id="7cb37-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="7cb37-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7cb37-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="7cb37-120">**Success**</span></span> <br/> |<span data-ttu-id="7cb37-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="7cb37-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="7cb37-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="7cb37-122">**Warning**</span></span> <br/> | <span data-ttu-id="7cb37-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="7cb37-123">Describes a request that was not processed.</span></span> <span data-ttu-id="7cb37-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="7cb37-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="7cb37-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="7cb37-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="7cb37-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="7cb37-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="7cb37-127">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="7cb37-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="7cb37-128">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="7cb37-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="7cb37-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="7cb37-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="7cb37-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="7cb37-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="7cb37-131">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="7cb37-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="7cb37-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="7cb37-132">**Error**</span></span> <br/> | <span data-ttu-id="7cb37-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="7cb37-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="7cb37-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="7cb37-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="7cb37-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="7cb37-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="7cb37-136">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="7cb37-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="7cb37-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="7cb37-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="7cb37-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="7cb37-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="7cb37-139">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="7cb37-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="7cb37-140">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="7cb37-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="7cb37-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="7cb37-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7cb37-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7cb37-142">Child elements</span></span>

|<span data-ttu-id="7cb37-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7cb37-143">**Element**</span></span>|<span data-ttu-id="7cb37-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="7cb37-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cb37-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="7cb37-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7cb37-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="7cb37-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7cb37-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7cb37-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7cb37-148">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="7cb37-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="7cb37-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7cb37-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7cb37-150">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="7cb37-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="7cb37-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="7cb37-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7cb37-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7cb37-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7cb37-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="7cb37-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7cb37-154">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="7cb37-154">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="7cb37-155">Représente un tableau des erreurs de validation de règle sur chaque champ de règle qui comporte une erreur.</span><span class="sxs-lookup"><span data-stu-id="7cb37-155">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7cb37-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7cb37-156">Parent elements</span></span>

<span data-ttu-id="7cb37-157">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7cb37-157">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7cb37-158">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7cb37-158">Text value</span></span>

<span data-ttu-id="7cb37-159">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7cb37-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7cb37-160">Remarques</span><span class="sxs-lookup"><span data-stu-id="7cb37-160">Remarks</span></span>

<span data-ttu-id="7cb37-161">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7cb37-161">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7cb37-162">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7cb37-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cb37-163">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7cb37-163">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7cb37-164">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7cb37-164">Schema name</span></span>  <br/> |<span data-ttu-id="7cb37-165">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7cb37-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7cb37-166">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7cb37-166">Validation file</span></span>  <br/> |<span data-ttu-id="7cb37-167">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7cb37-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7cb37-168">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7cb37-168">Can be empty</span></span>  <br/> |<span data-ttu-id="7cb37-169">False</span><span class="sxs-lookup"><span data-stu-id="7cb37-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cb37-170">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7cb37-170">See also</span></span>

- [<span data-ttu-id="7cb37-171">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7cb37-171">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="7cb37-172">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7cb37-172">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="7cb37-173">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7cb37-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

