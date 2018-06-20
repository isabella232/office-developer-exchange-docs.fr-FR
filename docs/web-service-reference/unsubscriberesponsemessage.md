---
title: UnsubscribeResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnsubscribeResponseMessage
api_type:
- schema
ms.assetid: 92c53b13-0ca1-4b44-b925-b23682e9417c
description: L’élément UnsubscribeResponseMessage contient l’état et les résultats d’une seule demande d’opération Annuler l’abonnement.
ms.openlocfilehash: 09475b8c858ddcd0e404819b6b9a281cbf7cfcbb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838850"
---
# <a name="unsubscriberesponsemessage"></a><span data-ttu-id="b799d-103">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b799d-103">UnsubscribeResponseMessage</span></span>

<span data-ttu-id="b799d-104">L’élément **UnsubscribeResponseMessage** contient l’état et les résultats d’une seule demande [d’opération Annuler l’abonnement](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b799d-104">The **UnsubscribeResponseMessage** element contains the status and result of a single [Unsubscribe operation](unsubscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="b799d-105">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="b799d-105">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
- [<span data-ttu-id="b799d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b799d-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="b799d-107">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b799d-107">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
  
```xml
<UnsubscribeResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UnsubscribeResponseMessage>
```

 <span data-ttu-id="b799d-108">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b799d-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b799d-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b799d-109">Attributes and elements</span></span>

<span data-ttu-id="b799d-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b799d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b799d-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="b799d-111">Attributes</span></span>

|<span data-ttu-id="b799d-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b799d-112">**Attribute**</span></span>|<span data-ttu-id="b799d-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="b799d-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b799d-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b799d-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b799d-115">Décrit l’état d’une réponse de [l’opération d’annulation d’abonnement](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b799d-115">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="b799d-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="b799d-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="b799d-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="b799d-117">-  Success</span></span>  <br/><span data-ttu-id="b799d-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="b799d-118">-  Warning</span></span>  <br/><span data-ttu-id="b799d-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="b799d-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b799d-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b799d-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="b799d-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="b799d-121">**Value**</span></span>|<span data-ttu-id="b799d-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="b799d-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b799d-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="b799d-123">**Success**</span></span> <br/> |<span data-ttu-id="b799d-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="b799d-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b799d-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="b799d-125">**Warning**</span></span> <br/> | <span data-ttu-id="b799d-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="b799d-126">Describes a request that was not processed.</span></span> <span data-ttu-id="b799d-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="b799d-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="b799d-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="b799d-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="b799d-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="b799d-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="b799d-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b799d-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="b799d-131">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="b799d-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="b799d-132">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b799d-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="b799d-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="b799d-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="b799d-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="b799d-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="b799d-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="b799d-135">**Error**</span></span> <br/> | <span data-ttu-id="b799d-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="b799d-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b799d-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="b799d-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b799d-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="b799d-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b799d-139">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="b799d-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="b799d-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="b799d-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="b799d-141">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="b799d-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="b799d-142">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="b799d-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b799d-143">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="b799d-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="b799d-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b799d-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b799d-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b799d-145">Child elements</span></span>

|<span data-ttu-id="b799d-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b799d-146">**Element**</span></span>|<span data-ttu-id="b799d-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="b799d-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b799d-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="b799d-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b799d-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="b799d-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b799d-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b799d-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b799d-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="b799d-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b799d-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b799d-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b799d-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="b799d-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="b799d-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="b799d-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b799d-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b799d-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b799d-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="b799d-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b799d-157">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b799d-157">Parent elements</span></span>

|<span data-ttu-id="b799d-158">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b799d-158">**Element**</span></span>|<span data-ttu-id="b799d-159">**Description**</span><span class="sxs-lookup"><span data-stu-id="b799d-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b799d-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b799d-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b799d-161">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b799d-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b799d-162">Remarques</span><span class="sxs-lookup"><span data-stu-id="b799d-162">Remarks</span></span>

<span data-ttu-id="b799d-163">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="b799d-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b799d-164">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b799d-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b799d-165">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b799d-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b799d-166">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b799d-166">Schema Name</span></span>  <br/> |<span data-ttu-id="b799d-167">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b799d-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b799d-168">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b799d-168">Validation File</span></span>  <br/> |<span data-ttu-id="b799d-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b799d-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b799d-170">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b799d-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="b799d-171">False</span><span class="sxs-lookup"><span data-stu-id="b799d-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b799d-172">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b799d-172">See also</span></span>

- [<span data-ttu-id="b799d-173">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="b799d-173">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="b799d-174">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b799d-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
