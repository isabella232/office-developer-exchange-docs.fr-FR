---
title: ExpandDLResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDLResponseMessage
api_type:
- schema
ms.assetid: 1140601b-98cf-4cb4-a019-321c7f63d5be
description: L’élément ExpandDLResponseMessage contient l’état et les résultats d’une demande d’opération ExpandDL unique.
ms.openlocfilehash: 62a81574f9c513b905a92876b3d757c635b4f07b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756264"
---
# <a name="expanddlresponsemessage"></a><span data-ttu-id="21ffb-103">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="21ffb-103">ExpandDLResponseMessage</span></span>

<span data-ttu-id="21ffb-104">L’élément **ExpandDLResponseMessage** contient l’état et les résultats d’une seule demande [d’opération ExpandDL](expanddl-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="21ffb-104">The **ExpandDLResponseMessage** element contains the status and result of a single [ExpandDL operation](expanddl-operation.md) request.</span></span> 
  
- [<span data-ttu-id="21ffb-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="21ffb-105">ExpandDLResponse</span></span>](expanddlresponse.md)  
- [<span data-ttu-id="21ffb-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="21ffb-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="21ffb-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="21ffb-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

<span data-ttu-id="21ffb-108">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="21ffb-108">**ExpandDLResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="21ffb-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="21ffb-109">Attributes and elements</span></span>

<span data-ttu-id="21ffb-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="21ffb-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21ffb-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="21ffb-111">Attributes</span></span>

|<span data-ttu-id="21ffb-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="21ffb-112">**Attribute**</span></span>|<span data-ttu-id="21ffb-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="21ffb-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="21ffb-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="21ffb-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="21ffb-115">Décrit l’état d’une réponse de [l’opération ExpandDL](expanddl-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="21ffb-115">Describes the status of an [ExpandDL operation](expanddl-operation.md) response.</span></span><br/><br/><span data-ttu-id="21ffb-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="21ffb-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="21ffb-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="21ffb-117">-  Success</span></span>  <br/><span data-ttu-id="21ffb-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="21ffb-118">-  Warning</span></span>  <br/><span data-ttu-id="21ffb-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="21ffb-119">-  Error</span></span>  <br/> |
|<span data-ttu-id="21ffb-120">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="21ffb-120">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="21ffb-121">Représente l’index suivant doit être utilisé pour la requête suivante lorsqu’une vue indexée de pagination est utilisée.</span><span class="sxs-lookup"><span data-stu-id="21ffb-121">Represents the next index that should be used for the next request when an indexed paging view is used.</span></span>  <br/> |
|<span data-ttu-id="21ffb-122">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="21ffb-122">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="21ffb-123">Représente la nouvelle valeur numérateur à utiliser pour la requête suivante lors de la fraction les vues de page sont utilisées.</span><span class="sxs-lookup"><span data-stu-id="21ffb-123">Represents the new numerator value to use for the next request when fraction page views are used.</span></span>  <br/> |
|<span data-ttu-id="21ffb-124">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="21ffb-124">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="21ffb-125">Représente le dénominateur suivant à utiliser pour la requête suivante lors de la pagination en fraction.</span><span class="sxs-lookup"><span data-stu-id="21ffb-125">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="21ffb-126">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="21ffb-126">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="21ffb-127">Indique que le fichier d’échange supplémentaire n’est pas nécessaire.</span><span class="sxs-lookup"><span data-stu-id="21ffb-127">Indicates that additional paging is not needed.</span></span> <span data-ttu-id="21ffb-128">Cet attribut aura la valeur true si le résultat actuel contient le dernier élément dans la requête.</span><span class="sxs-lookup"><span data-stu-id="21ffb-128">This attribute will be true if the current results contain the last item in the query.</span></span>  <br/> |
|<span data-ttu-id="21ffb-129">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="21ffb-129">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="21ffb-130">Représente le nombre total d’éléments qui transmet la restriction.</span><span class="sxs-lookup"><span data-stu-id="21ffb-130">Represents the total number of items that pass the restriction.</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="21ffb-131">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="21ffb-131">ResponseClass attribute values</span></span>

|<span data-ttu-id="21ffb-132">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="21ffb-132">**Value**</span></span>|<span data-ttu-id="21ffb-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="21ffb-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="21ffb-134">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="21ffb-134">**Success**</span></span> <br/> |<span data-ttu-id="21ffb-135">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="21ffb-135">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="21ffb-136">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="21ffb-136">**Warning**</span></span> <br/> | <span data-ttu-id="21ffb-137">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="21ffb-137">Describes a request that was not processed.</span></span> <span data-ttu-id="21ffb-138">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="21ffb-138">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="21ffb-139">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="21ffb-139">The following are examples of sources of warnings:</span></span><br/>  <br/><span data-ttu-id="21ffb-140">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="21ffb-140">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="21ffb-141">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="21ffb-141">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="21ffb-142">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="21ffb-142">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="21ffb-143">-La base de données de boîtes aux lettres (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="21ffb-143">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="21ffb-144">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="21ffb-144">-  A password is expired.</span></span>  <br/><span data-ttu-id="21ffb-145">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="21ffb-145">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="21ffb-146">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="21ffb-146">**Error**</span></span> <br/> | <span data-ttu-id="21ffb-147">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="21ffb-147">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="21ffb-148">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="21ffb-148">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="21ffb-149">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="21ffb-149">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="21ffb-150">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="21ffb-150">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="21ffb-151">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="21ffb-151">-  An unknown tag</span></span>  <br/><span data-ttu-id="21ffb-152">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="21ffb-152">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="21ffb-153">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="21ffb-153">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="21ffb-154">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="21ffb-154">-  A server-side failure in response to a valid client-side call</span></span> <br/> <br/>  <span data-ttu-id="21ffb-155">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="21ffb-155">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="21ffb-156">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="21ffb-156">Child elements</span></span>

|<span data-ttu-id="21ffb-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="21ffb-157">**Element**</span></span>|<span data-ttu-id="21ffb-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="21ffb-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21ffb-159">MessageText</span><span class="sxs-lookup"><span data-stu-id="21ffb-159">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="21ffb-160">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="21ffb-160">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="21ffb-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="21ffb-161">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="21ffb-162">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="21ffb-162">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="21ffb-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="21ffb-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="21ffb-164">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="21ffb-164">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="21ffb-165">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="21ffb-165">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="21ffb-166">MessageXml</span><span class="sxs-lookup"><span data-stu-id="21ffb-166">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="21ffb-167">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="21ffb-167">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="21ffb-168">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="21ffb-168">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="21ffb-169">Contient un tableau de boîtes aux lettres qui sont contenus dans une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="21ffb-169">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21ffb-170">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="21ffb-170">Parent elements</span></span>

|<span data-ttu-id="21ffb-171">**Élément**</span><span class="sxs-lookup"><span data-stu-id="21ffb-171">**Element**</span></span>|<span data-ttu-id="21ffb-172">**Description**</span><span class="sxs-lookup"><span data-stu-id="21ffb-172">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21ffb-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="21ffb-173">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="21ffb-174">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="21ffb-174">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="21ffb-175">Remarques</span><span class="sxs-lookup"><span data-stu-id="21ffb-175">Remarks</span></span>

<span data-ttu-id="21ffb-176">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="21ffb-176">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21ffb-177">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="21ffb-177">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21ffb-178">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="21ffb-178">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="21ffb-179">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="21ffb-179">Schema Name</span></span>  <br/> |<span data-ttu-id="21ffb-180">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="21ffb-180">Types schema</span></span>  <br/> |
|<span data-ttu-id="21ffb-181">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="21ffb-181">Validation File</span></span>  <br/> |<span data-ttu-id="21ffb-182">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="21ffb-182">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="21ffb-183">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="21ffb-183">Can be Empty</span></span>  <br/> |<span data-ttu-id="21ffb-184">False</span><span class="sxs-lookup"><span data-stu-id="21ffb-184">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21ffb-185">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="21ffb-185">See also</span></span>

- [<span data-ttu-id="21ffb-186">Opération ExpandDL</span><span class="sxs-lookup"><span data-stu-id="21ffb-186">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="21ffb-187">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="21ffb-187">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="21ffb-188">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="21ffb-188">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

