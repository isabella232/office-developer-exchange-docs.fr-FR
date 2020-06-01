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
description: L’élément UnsubscribeResponseMessage contient l’État et le résultat d’une demande d’opération de désinscription unique.
ms.openlocfilehash: e5b42404d09e6367c134934409ec2a45351e135e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467164"
---
# <a name="unsubscriberesponsemessage"></a><span data-ttu-id="4b3ce-103">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4b3ce-103">UnsubscribeResponseMessage</span></span>

<span data-ttu-id="4b3ce-104">L’élément **UnsubscribeResponseMessage** contient l’État et le résultat d’une demande d' [opération de désinscription](unsubscribe-operation.md) unique.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-104">The **UnsubscribeResponseMessage** element contains the status and result of a single [Unsubscribe operation](unsubscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="4b3ce-105">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="4b3ce-105">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
- [<span data-ttu-id="4b3ce-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4b3ce-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="4b3ce-107">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4b3ce-107">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
  
```xml
<UnsubscribeResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UnsubscribeResponseMessage>
```

 <span data-ttu-id="4b3ce-108">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b3ce-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4b3ce-109">Attributes and elements</span></span>

<span data-ttu-id="4b3ce-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b3ce-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="4b3ce-111">Attributes</span></span>

|<span data-ttu-id="4b3ce-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-112">**Attribute**</span></span>|<span data-ttu-id="4b3ce-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4b3ce-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4b3ce-115">Décrit l’état d’une réponse d' [opération de résiliation](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4b3ce-115">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="4b3ce-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="4b3ce-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="4b3ce-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="4b3ce-117">-  Success</span></span>  <br/><span data-ttu-id="4b3ce-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="4b3ce-118">-  Warning</span></span>  <br/><span data-ttu-id="4b3ce-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="4b3ce-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4b3ce-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="4b3ce-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="4b3ce-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-121">**Value**</span></span>|<span data-ttu-id="4b3ce-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4b3ce-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-123">**Success**</span></span> <br/> |<span data-ttu-id="4b3ce-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4b3ce-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-125">**Warning**</span></span> <br/> | <span data-ttu-id="4b3ce-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-126">Describes a request that was not processed.</span></span> <span data-ttu-id="4b3ce-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="4b3ce-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="4b3ce-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="4b3ce-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="4b3ce-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="4b3ce-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="4b3ce-132">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="4b3ce-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="4b3ce-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="4b3ce-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-135">**Error**</span></span> <br/> | <span data-ttu-id="4b3ce-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4b3ce-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="4b3ce-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="4b3ce-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="4b3ce-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4b3ce-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="4b3ce-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="4b3ce-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="4b3ce-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="4b3ce-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="4b3ce-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="4b3ce-142">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="4b3ce-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4b3ce-143">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="4b3ce-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="4b3ce-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="4b3ce-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4b3ce-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4b3ce-145">Child elements</span></span>

|<span data-ttu-id="4b3ce-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-146">**Element**</span></span>|<span data-ttu-id="4b3ce-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b3ce-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="4b3ce-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4b3ce-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4b3ce-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4b3ce-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4b3ce-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4b3ce-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4b3ce-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4b3ce-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4b3ce-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4b3ce-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4b3ce-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4b3ce-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b3ce-157">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4b3ce-157">Parent elements</span></span>

|<span data-ttu-id="4b3ce-158">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-158">**Element**</span></span>|<span data-ttu-id="4b3ce-159">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b3ce-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b3ce-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4b3ce-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4b3ce-161">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4b3ce-162">Remarques</span><span class="sxs-lookup"><span data-stu-id="4b3ce-162">Remarks</span></span>

<span data-ttu-id="4b3ce-163">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4b3ce-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b3ce-164">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4b3ce-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b3ce-165">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4b3ce-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4b3ce-166">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4b3ce-166">Schema Name</span></span>  <br/> |<span data-ttu-id="4b3ce-167">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4b3ce-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4b3ce-168">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4b3ce-168">Validation File</span></span>  <br/> |<span data-ttu-id="4b3ce-169">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4b3ce-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4b3ce-170">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4b3ce-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b3ce-171">False</span><span class="sxs-lookup"><span data-stu-id="4b3ce-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b3ce-172">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4b3ce-172">See also</span></span>

- [<span data-ttu-id="4b3ce-173">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="4b3ce-173">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="4b3ce-174">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b3ce-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

