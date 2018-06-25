---
title: RefreshSharingFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolderResponse
api_type:
- schema
ms.assetid: 951ab681-f2d5-4f10-933e-ff199685ff8e
description: L’élément RefreshSharingFolderResponse définit une réponse à une demande d’opération RefreshSharingFolder.
ms.openlocfilehash: 4ef7a63b2153c6106dae988439f499046689c2b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829048"
---
# <a name="refreshsharingfolderresponse"></a><span data-ttu-id="a6c17-103">RefreshSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="a6c17-103">RefreshSharingFolderResponse</span></span>

<span data-ttu-id="a6c17-104">L’élément **RefreshSharingFolderResponse** définit une réponse à une demande [d’opération RefreshSharingFolder](refreshsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a6c17-104">The **RefreshSharingFolderResponse** element defines a response to a [RefreshSharingFolder operation](refreshsharingfolder-operation.md) request.</span></span> 
  
```xml
<RefreshSharingFolderResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponse>
```

 <span data-ttu-id="a6c17-105">**RefreshSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a6c17-105">**RefreshSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a6c17-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a6c17-106">Attributes and elements</span></span>

<span data-ttu-id="a6c17-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a6c17-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6c17-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a6c17-108">Attributes</span></span>

|<span data-ttu-id="a6c17-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a6c17-109">**Attribute**</span></span>|<span data-ttu-id="a6c17-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="a6c17-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a6c17-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="a6c17-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a6c17-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="a6c17-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="a6c17-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="a6c17-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="a6c17-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="a6c17-114">-  Success</span></span>  <br/><span data-ttu-id="a6c17-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="a6c17-115">-  Warning</span></span>  <br/><span data-ttu-id="a6c17-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="a6c17-116">-  Error</span></span>  <br/>- |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="a6c17-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a6c17-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="a6c17-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a6c17-118">**Value**</span></span>|<span data-ttu-id="a6c17-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="a6c17-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a6c17-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="a6c17-120">**Success**</span></span> <br/> |<span data-ttu-id="a6c17-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="a6c17-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a6c17-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="a6c17-122">**Warning**</span></span> <br/> | <span data-ttu-id="a6c17-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="a6c17-123">Describes a request that was not processed.</span></span> <span data-ttu-id="a6c17-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="a6c17-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="a6c17-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="a6c17-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="a6c17-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="a6c17-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="a6c17-127">-Le service d’annuaire Active Directory est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="a6c17-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="a6c17-128">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="a6c17-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="a6c17-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="a6c17-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="a6c17-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="a6c17-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="a6c17-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="a6c17-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="a6c17-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="a6c17-132">**Error**</span></span> <br/> | <span data-ttu-id="a6c17-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="a6c17-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="a6c17-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="a6c17-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="a6c17-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="a6c17-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="a6c17-136">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="a6c17-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="a6c17-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="a6c17-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="a6c17-138">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="a6c17-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="a6c17-139">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="a6c17-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="a6c17-140">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="a6c17-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="a6c17-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="a6c17-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a6c17-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a6c17-142">Child elements</span></span>

|<span data-ttu-id="a6c17-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a6c17-143">**Element**</span></span>|<span data-ttu-id="a6c17-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="a6c17-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6c17-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="a6c17-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a6c17-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="a6c17-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a6c17-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a6c17-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a6c17-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="a6c17-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="a6c17-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a6c17-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a6c17-150">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="a6c17-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="a6c17-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="a6c17-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a6c17-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a6c17-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a6c17-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="a6c17-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a6c17-154">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a6c17-154">Parent elements</span></span>

<span data-ttu-id="a6c17-155">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a6c17-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a6c17-156">Remarques</span><span class="sxs-lookup"><span data-stu-id="a6c17-156">Remarks</span></span>

<span data-ttu-id="a6c17-157">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="a6c17-157">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6c17-158">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a6c17-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6c17-159">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a6c17-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a6c17-160">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a6c17-160">Schema Name</span></span>  <br/> |<span data-ttu-id="a6c17-161">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a6c17-161">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a6c17-162">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a6c17-162">Validation File</span></span>  <br/> |<span data-ttu-id="a6c17-163">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a6c17-163">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a6c17-164">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a6c17-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="a6c17-165">False</span><span class="sxs-lookup"><span data-stu-id="a6c17-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a6c17-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a6c17-166">See also</span></span>

- [<span data-ttu-id="a6c17-167">Opération RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="a6c17-167">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md)
- [<span data-ttu-id="a6c17-168">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a6c17-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

