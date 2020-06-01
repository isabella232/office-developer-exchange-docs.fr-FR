---
title: UpdateUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: 27728e57-5a9b-4314-ad64-df7869098f62
description: L’élément UpdateUserConfigurationResponseMessage contient l’État et le résultat d’une seule demande d’opération UpdateUserConfiguration.
ms.openlocfilehash: 9c885c87f4b48df16e4097b9c4eafd7e9278c7b8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468522"
---
# <a name="updateuserconfigurationresponsemessage"></a><span data-ttu-id="fd0cf-103">UpdateUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fd0cf-103">UpdateUserConfigurationResponseMessage</span></span>

<span data-ttu-id="fd0cf-104">L’élément **UpdateUserConfigurationResponseMessage** contient l’État et le résultat d’une seule demande d’opération UpdateUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-104">The **UpdateUserConfigurationResponseMessage** element contains the status and result of a single UpdateUserConfiguration operation request.</span></span> 
  
```xml
<UpdateUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateUserConfigurationResponseMessage>
```

 <span data-ttu-id="fd0cf-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd0cf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fd0cf-106">Attributes and elements</span></span>

<span data-ttu-id="fd0cf-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd0cf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fd0cf-108">Attributes</span></span>

|<span data-ttu-id="fd0cf-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-109">**Attribute**</span></span>|<span data-ttu-id="fd0cf-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fd0cf-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="fd0cf-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="fd0cf-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="fd0cf-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="fd0cf-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="fd0cf-114">-  Success</span></span>  <br/><span data-ttu-id="fd0cf-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="fd0cf-115">-  Warning</span></span>  <br/><span data-ttu-id="fd0cf-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="fd0cf-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="fd0cf-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fd0cf-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="fd0cf-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-118">**Value**</span></span>|<span data-ttu-id="fd0cf-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fd0cf-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-120">**Success**</span></span> <br/> |<span data-ttu-id="fd0cf-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="fd0cf-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-122">**Warning**</span></span> <br/> | <span data-ttu-id="fd0cf-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-123">Describes a request that was not processed.</span></span> <span data-ttu-id="fd0cf-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="fd0cf-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="fd0cf-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="fd0cf-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="fd0cf-127">-Le service d’annuaire Active Directory est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="fd0cf-128">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="fd0cf-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="fd0cf-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="fd0cf-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="fd0cf-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-132">**Error**</span></span> <br/> | <span data-ttu-id="fd0cf-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="fd0cf-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="fd0cf-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="fd0cf-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="fd0cf-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="fd0cf-136">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="fd0cf-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="fd0cf-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="fd0cf-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="fd0cf-138">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="fd0cf-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="fd0cf-139">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="fd0cf-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="fd0cf-140">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="fd0cf-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="fd0cf-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="fd0cf-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fd0cf-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fd0cf-142">Child elements</span></span>

|<span data-ttu-id="fd0cf-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-143">**Element**</span></span>|<span data-ttu-id="fd0cf-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd0cf-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="fd0cf-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="fd0cf-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="fd0cf-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fd0cf-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="fd0cf-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="fd0cf-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="fd0cf-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="fd0cf-150">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="fd0cf-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="fd0cf-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="fd0cf-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="fd0cf-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fd0cf-154">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fd0cf-154">Parent elements</span></span>

|<span data-ttu-id="fd0cf-155">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-155">**Element**</span></span>|<span data-ttu-id="fd0cf-156">**Description**</span><span class="sxs-lookup"><span data-stu-id="fd0cf-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd0cf-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fd0cf-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fd0cf-158">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fd0cf-159">Remarques</span><span class="sxs-lookup"><span data-stu-id="fd0cf-159">Remarks</span></span>

<span data-ttu-id="fd0cf-160">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fd0cf-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd0cf-161">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fd0cf-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd0cf-162">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fd0cf-162">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fd0cf-163">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fd0cf-163">Schema Name</span></span>  <br/> |<span data-ttu-id="fd0cf-164">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="fd0cf-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fd0cf-165">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fd0cf-165">Validation File</span></span>  <br/> |<span data-ttu-id="fd0cf-166">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fd0cf-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fd0cf-167">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fd0cf-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd0cf-168">False</span><span class="sxs-lookup"><span data-stu-id="fd0cf-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd0cf-169">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fd0cf-169">See also</span></span>

- [<span data-ttu-id="fd0cf-170">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fd0cf-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

