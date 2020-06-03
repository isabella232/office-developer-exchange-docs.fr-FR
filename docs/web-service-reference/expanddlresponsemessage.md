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
description: L’élément ExpandDLResponseMessage contient l’État et le résultat d’une seule demande d’opération ExpandDL.
ms.openlocfilehash: e186c4e14cbb9c922a4d262c85c130b9c33ff939
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460637"
---
# <a name="expanddlresponsemessage"></a><span data-ttu-id="38599-103">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="38599-103">ExpandDLResponseMessage</span></span>

<span data-ttu-id="38599-104">L’élément **ExpandDLResponseMessage** contient l’État et le résultat d’une seule demande d' [opération ExpandDL](expanddl-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="38599-104">The **ExpandDLResponseMessage** element contains the status and result of a single [ExpandDL operation](expanddl-operation.md) request.</span></span> 
  
- [<span data-ttu-id="38599-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="38599-105">ExpandDLResponse</span></span>](expanddlresponse.md)  
- [<span data-ttu-id="38599-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="38599-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="38599-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="38599-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

<span data-ttu-id="38599-108">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="38599-108">**ExpandDLResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="38599-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="38599-109">Attributes and elements</span></span>

<span data-ttu-id="38599-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="38599-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38599-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="38599-111">Attributes</span></span>

|<span data-ttu-id="38599-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="38599-112">**Attribute**</span></span>|<span data-ttu-id="38599-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="38599-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="38599-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="38599-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="38599-115">Décrit l’état d’une réponse d' [opération ExpandDL](expanddl-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="38599-115">Describes the status of an [ExpandDL operation](expanddl-operation.md) response.</span></span><br/><br/><span data-ttu-id="38599-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="38599-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="38599-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="38599-117">-  Success</span></span>  <br/><span data-ttu-id="38599-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="38599-118">-  Warning</span></span>  <br/><span data-ttu-id="38599-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="38599-119">-  Error</span></span>  <br/> |
|<span data-ttu-id="38599-120">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="38599-120">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="38599-121">Représente l’index suivant qui doit être utilisé pour la prochaine requête lorsqu’une vue de pagination indexée est utilisée.</span><span class="sxs-lookup"><span data-stu-id="38599-121">Represents the next index that should be used for the next request when an indexed paging view is used.</span></span>  <br/> |
|<span data-ttu-id="38599-122">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="38599-122">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="38599-123">Représente la nouvelle valeur de numérateur à utiliser pour la requête suivante lorsque les vues de fraction de page sont utilisées.</span><span class="sxs-lookup"><span data-stu-id="38599-123">Represents the new numerator value to use for the next request when fraction page views are used.</span></span>  <br/> |
|<span data-ttu-id="38599-124">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="38599-124">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="38599-125">Représente le dénominateur suivant à utiliser pour la requête suivante lors de la pagination fractionnée.</span><span class="sxs-lookup"><span data-stu-id="38599-125">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="38599-126">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="38599-126">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="38599-127">Indique que la pagination supplémentaire n’est pas nécessaire.</span><span class="sxs-lookup"><span data-stu-id="38599-127">Indicates that additional paging is not needed.</span></span> <span data-ttu-id="38599-128">Cet attribut est true si les résultats actuels contiennent le dernier élément de la requête.</span><span class="sxs-lookup"><span data-stu-id="38599-128">This attribute will be true if the current results contain the last item in the query.</span></span>  <br/> |
|<span data-ttu-id="38599-129">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="38599-129">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="38599-130">Représente le nombre total d’éléments qui ont passé la restriction.</span><span class="sxs-lookup"><span data-stu-id="38599-130">Represents the total number of items that pass the restriction.</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="38599-131">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="38599-131">ResponseClass attribute values</span></span>

|<span data-ttu-id="38599-132">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="38599-132">**Value**</span></span>|<span data-ttu-id="38599-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="38599-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="38599-134">**Success**</span><span class="sxs-lookup"><span data-stu-id="38599-134">**Success**</span></span> <br/> |<span data-ttu-id="38599-135">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="38599-135">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="38599-136">**Warning**</span><span class="sxs-lookup"><span data-stu-id="38599-136">**Warning**</span></span> <br/> | <span data-ttu-id="38599-137">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="38599-137">Describes a request that was not processed.</span></span> <span data-ttu-id="38599-138">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="38599-138">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="38599-139">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="38599-139">The following are examples of sources of warnings:</span></span><br/>  <br/><span data-ttu-id="38599-140">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="38599-140">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="38599-141">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="38599-141">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="38599-142">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="38599-142">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="38599-143">-La base de données de boîtes aux lettres (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="38599-143">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="38599-144">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="38599-144">-  A password is expired.</span></span>  <br/><span data-ttu-id="38599-145">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="38599-145">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="38599-146">**Error**</span><span class="sxs-lookup"><span data-stu-id="38599-146">**Error**</span></span> <br/> | <span data-ttu-id="38599-147">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="38599-147">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="38599-148">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="38599-148">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="38599-149">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="38599-149">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="38599-150">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="38599-150">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="38599-151">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="38599-151">-  An unknown tag</span></span>  <br/><span data-ttu-id="38599-152">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="38599-152">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="38599-153">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="38599-153">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="38599-154">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="38599-154">-  A server-side failure in response to a valid client-side call</span></span> <br/> <br/>  <span data-ttu-id="38599-155">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="38599-155">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="38599-156">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="38599-156">Child elements</span></span>

|<span data-ttu-id="38599-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="38599-157">**Element**</span></span>|<span data-ttu-id="38599-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="38599-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38599-159">MessageText</span><span class="sxs-lookup"><span data-stu-id="38599-159">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="38599-160">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="38599-160">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="38599-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="38599-161">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="38599-162">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="38599-162">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="38599-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="38599-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="38599-164">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="38599-164">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="38599-165">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="38599-165">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="38599-166">MessageXml</span><span class="sxs-lookup"><span data-stu-id="38599-166">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="38599-167">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="38599-167">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="38599-168">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="38599-168">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="38599-169">Contient un tableau de boîtes aux lettres contenues dans une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="38599-169">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="38599-170">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="38599-170">Parent elements</span></span>

|<span data-ttu-id="38599-171">**Élément**</span><span class="sxs-lookup"><span data-stu-id="38599-171">**Element**</span></span>|<span data-ttu-id="38599-172">**Description**</span><span class="sxs-lookup"><span data-stu-id="38599-172">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38599-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="38599-173">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="38599-174">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="38599-174">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="38599-175">Remarques</span><span class="sxs-lookup"><span data-stu-id="38599-175">Remarks</span></span>

<span data-ttu-id="38599-176">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="38599-176">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38599-177">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="38599-177">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38599-178">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="38599-178">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38599-179">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="38599-179">Schema Name</span></span>  <br/> |<span data-ttu-id="38599-180">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="38599-180">Types schema</span></span>  <br/> |
|<span data-ttu-id="38599-181">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="38599-181">Validation File</span></span>  <br/> |<span data-ttu-id="38599-182">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="38599-182">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="38599-183">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="38599-183">Can be Empty</span></span>  <br/> |<span data-ttu-id="38599-184">False</span><span class="sxs-lookup"><span data-stu-id="38599-184">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38599-185">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="38599-185">See also</span></span>

- [<span data-ttu-id="38599-186">Opération ExpandDL</span><span class="sxs-lookup"><span data-stu-id="38599-186">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="38599-187">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="38599-187">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="38599-188">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38599-188">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

