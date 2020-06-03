---
title: EmptyFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 678dd5ce-8d9e-4939-bf1b-a8e148f4f449
description: L’élément EmptyFolderResponseMessage contient l’État et le résultat d’une seule requête EmptyFolder.
ms.openlocfilehash: fd69df45d7e1d6538a977b79711baa769413ea66
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526213"
---
# <a name="emptyfolderresponsemessage"></a><span data-ttu-id="b55d3-103">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b55d3-103">EmptyFolderResponseMessage</span></span>

<span data-ttu-id="b55d3-104">L’élément **EmptyFolderResponseMessage** contient l’État et le résultat d’une seule requête [EmptyFolder](emptyfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="b55d3-104">The **EmptyFolderResponseMessage** element contains the status and result of a single [EmptyFolder](emptyfolder.md) request.</span></span> 
  
```XML
<EmptyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</EmptyFolderResponseMessage>
```

 <span data-ttu-id="b55d3-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b55d3-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b55d3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b55d3-106">Attributes and elements</span></span>

<span data-ttu-id="b55d3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b55d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b55d3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b55d3-108">Attributes</span></span>

|<span data-ttu-id="b55d3-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b55d3-109">**Attribute**</span></span>|<span data-ttu-id="b55d3-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="b55d3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b55d3-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b55d3-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b55d3-112">Décrit l’état d’une réponse d' [opération EmptyFolder](emptyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b55d3-112">Describes the status of an [EmptyFolder operation](emptyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="b55d3-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="b55d3-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="b55d3-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="b55d3-114">-  Success</span></span>  <br/><span data-ttu-id="b55d3-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="b55d3-115">-  Warning</span></span>  <br/><span data-ttu-id="b55d3-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="b55d3-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b55d3-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b55d3-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="b55d3-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="b55d3-118">**Value**</span></span>|<span data-ttu-id="b55d3-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="b55d3-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b55d3-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="b55d3-120">**Success**</span></span> <br/> |<span data-ttu-id="b55d3-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="b55d3-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b55d3-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="b55d3-122">**Warning**</span></span> <br/> | <span data-ttu-id="b55d3-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="b55d3-123">Describes a request that was not processed.</span></span> <span data-ttu-id="b55d3-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="b55d3-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="b55d3-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="b55d3-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="b55d3-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="b55d3-126">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="b55d3-127">-Les services de domaine Active Directory (AD DS) sont en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b55d3-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="b55d3-128">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="b55d3-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="b55d3-129">-La base de données de messages (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b55d3-129">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="b55d3-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="b55d3-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="b55d3-131">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="b55d3-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="b55d3-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="b55d3-132">**Error**</span></span> <br/> | <span data-ttu-id="b55d3-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="b55d3-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="b55d3-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="b55d3-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b55d3-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="b55d3-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b55d3-136">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="b55d3-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="b55d3-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="b55d3-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="b55d3-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="b55d3-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="b55d3-139">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="b55d3-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b55d3-140">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="b55d3-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="b55d3-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b55d3-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b55d3-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b55d3-142">Child elements</span></span>

|<span data-ttu-id="b55d3-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b55d3-143">**Element**</span></span>|<span data-ttu-id="b55d3-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="b55d3-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b55d3-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="b55d3-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b55d3-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="b55d3-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b55d3-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b55d3-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b55d3-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="b55d3-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b55d3-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b55d3-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b55d3-150">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="b55d3-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="b55d3-151">Il contient la valeur 0.</span><span class="sxs-lookup"><span data-stu-id="b55d3-151">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b55d3-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b55d3-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b55d3-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="b55d3-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b55d3-154">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b55d3-154">Parent elements</span></span>

|<span data-ttu-id="b55d3-155">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b55d3-155">**Element**</span></span>|<span data-ttu-id="b55d3-156">**Description**</span><span class="sxs-lookup"><span data-stu-id="b55d3-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b55d3-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b55d3-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b55d3-158">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b55d3-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b55d3-159">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b55d3-159">Text value</span></span>

<span data-ttu-id="b55d3-160">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b55d3-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b55d3-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="b55d3-161">Remarks</span></span>

<span data-ttu-id="b55d3-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b55d3-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b55d3-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b55d3-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b55d3-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b55d3-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b55d3-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b55d3-165">Schema Name</span></span>  <br/> |<span data-ttu-id="b55d3-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b55d3-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b55d3-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b55d3-167">Validation File</span></span>  <br/> |<span data-ttu-id="b55d3-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b55d3-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b55d3-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b55d3-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="b55d3-170">False</span><span class="sxs-lookup"><span data-stu-id="b55d3-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b55d3-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b55d3-171">See also</span></span>

- [<span data-ttu-id="b55d3-172">Opération EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="b55d3-172">EmptyFolder operation</span></span>](emptyfolder-operation.md)
- [<span data-ttu-id="b55d3-173">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b55d3-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="b55d3-174">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b55d3-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

