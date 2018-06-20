---
title: GetItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItemResponseMessage
api_type:
- schema
ms.assetid: cc583723-54d1-4a17-8c1f-6586f70fdefd
description: L’élément GetItemResponseMessage contient l’état et les résultats d’une demande d’opération GetItem unique.
ms.openlocfilehash: 0c8527258d4637ede053e189dfb918b910c859d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756668"
---
# <a name="getitemresponsemessage"></a><span data-ttu-id="4d2ef-103">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4d2ef-103">GetItemResponseMessage</span></span>

<span data-ttu-id="4d2ef-104">L’élément **GetItemResponseMessage** contient l’état et les résultats d’une seule demande [GetItem operation](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4d2ef-104">The **GetItemResponseMessage** element contains the status and result of a single [GetItem operation](getitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="4d2ef-105">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="4d2ef-105">GetItemResponse</span></span>](getitemresponse.md) 
- [<span data-ttu-id="4d2ef-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4d2ef-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="4d2ef-107">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4d2ef-107">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

<span data-ttu-id="4d2ef-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-108">**ItemInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4d2ef-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4d2ef-109">Attributes and elements</span></span>

<span data-ttu-id="4d2ef-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d2ef-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="4d2ef-111">Attributes</span></span>

|<span data-ttu-id="4d2ef-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-112">**Attribute**</span></span>|<span data-ttu-id="4d2ef-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4d2ef-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4d2ef-115">Décrit l’état d’une réponse [GetItem operation](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4d2ef-115">Describes the status of a [GetItem operation](getitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="4d2ef-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="4d2ef-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="4d2ef-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="4d2ef-117">- Success</span></span><br/><span data-ttu-id="4d2ef-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="4d2ef-118">- Warning</span></span><br/><span data-ttu-id="4d2ef-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="4d2ef-119">- Error</span></span> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4d2ef-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="4d2ef-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="4d2ef-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-121">**Value**</span></span>|<span data-ttu-id="4d2ef-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4d2ef-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-123">**Success**</span></span> <br/> |<span data-ttu-id="4d2ef-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4d2ef-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-125">**Warning**</span></span> <br/> | <span data-ttu-id="4d2ef-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-126">Describes a request that was not processed.</span></span> <span data-ttu-id="4d2ef-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant un élément dans la demande a été traité et les éléments suivants n’ont pas peuvent être traitées.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="4d2ef-128">Voici des exemples de sources pour les avertissements :</span><span class="sxs-lookup"><span data-stu-id="4d2ef-128">The following are examples of sources for warnings:</span></span><br/><br/><span data-ttu-id="4d2ef-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-129">- The Exchange store is offline during the batch.</span></span><br/><span data-ttu-id="4d2ef-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-130">- Active Directory Domain Services (AD DS) is offline.</span></span><br/><span data-ttu-id="4d2ef-131">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="4d2ef-132">-MDB est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-132">- MDB is offline.</span></span><br/><span data-ttu-id="4d2ef-133">-Le mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-133">- Password is expired.</span></span>  <br/><span data-ttu-id="4d2ef-134">-Quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-134">- Quota is exceeded.</span></span> |
|<span data-ttu-id="4d2ef-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-135">**Error**</span></span> <br/> | <span data-ttu-id="4d2ef-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="4d2ef-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="4d2ef-137">The following are examples of sources for errors:</span></span><br/><br/><span data-ttu-id="4d2ef-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="4d2ef-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="4d2ef-139">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="4d2ef-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="4d2ef-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="4d2ef-140">- Unknown tag</span></span><br/><span data-ttu-id="4d2ef-141">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="4d2ef-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="4d2ef-142">-Accès non autorisé a tenté par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="4d2ef-142">- Unauthorized access attempted by any client</span></span><br/><span data-ttu-id="4d2ef-143">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="4d2ef-143">- Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="4d2ef-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="4d2ef-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="4d2ef-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4d2ef-145">Child elements</span></span>

|<span data-ttu-id="4d2ef-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-146">**Element**</span></span>|<span data-ttu-id="4d2ef-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d2ef-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="4d2ef-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4d2ef-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4d2ef-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4d2ef-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4d2ef-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4d2ef-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4d2ef-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4d2ef-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4d2ef-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4d2ef-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4d2ef-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4d2ef-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4d2ef-157">Items</span><span class="sxs-lookup"><span data-stu-id="4d2ef-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="4d2ef-158">Contient un tableau d’éléments renvoyés.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-158">Contains an array of returned items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d2ef-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4d2ef-159">Parent elements</span></span>

|<span data-ttu-id="4d2ef-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-160">**Element**</span></span>|<span data-ttu-id="4d2ef-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d2ef-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d2ef-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4d2ef-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4d2ef-163">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d2ef-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="4d2ef-164">Remarks</span></span>

<span data-ttu-id="4d2ef-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="4d2ef-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d2ef-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4d2ef-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d2ef-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4d2ef-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4d2ef-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4d2ef-168">Schema Name</span></span>  <br/> |<span data-ttu-id="4d2ef-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4d2ef-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4d2ef-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4d2ef-170">Validation File</span></span>  <br/> |<span data-ttu-id="4d2ef-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4d2ef-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4d2ef-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4d2ef-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d2ef-173">False</span><span class="sxs-lookup"><span data-stu-id="4d2ef-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d2ef-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4d2ef-174">See also</span></span>

- [<span data-ttu-id="4d2ef-175">GetItem</span><span class="sxs-lookup"><span data-stu-id="4d2ef-175">GetItem</span></span>](getitem.md)
- [<span data-ttu-id="4d2ef-176">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="4d2ef-176">GetItem operation</span></span>](getitem-operation.md)
