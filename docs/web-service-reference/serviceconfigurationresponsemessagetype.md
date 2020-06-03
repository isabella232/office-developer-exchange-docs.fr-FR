---
title: ServiceConfigurationResponseMessageType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServiceConfigurationResponseMessageType
api_type:
- schema
ms.assetid: ccfb0578-c648-44c2-ac4d-7620d881363e
description: L’élément ServiceConfigurationResponseMessageType contient les paramètres de configuration du service.
ms.openlocfilehash: 4c84a49b2403343a1defd00696858489497d6214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44439104"
---
# <a name="serviceconfigurationresponsemessagetype"></a><span data-ttu-id="5835e-103">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="5835e-103">ServiceConfigurationResponseMessageType</span></span>

<span data-ttu-id="5835e-104">L’élément **ServiceConfigurationResponseMessageType** contient les paramètres de configuration du service.</span><span class="sxs-lookup"><span data-stu-id="5835e-104">The **ServiceConfigurationResponseMessageType** element contains service configuration settings.</span></span> 
  
```XML
<ServiceConfigurationResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTipsConfiguration/>
   <UnifiedMessagingConfiguration/>
   <ProtectionRulesConfiguration/>
</ServiceConfigurationResponseMessageType>
```

 <span data-ttu-id="5835e-105">**ServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5835e-105">**ServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5835e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5835e-106">Attributes and elements</span></span>

<span data-ttu-id="5835e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5835e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5835e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5835e-108">Attributes</span></span>

|<span data-ttu-id="5835e-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="5835e-109">**Attribute**</span></span>|<span data-ttu-id="5835e-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="5835e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5835e-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="5835e-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="5835e-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="5835e-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="5835e-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="5835e-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="5835e-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="5835e-114">-  Success</span></span>  <br/><span data-ttu-id="5835e-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="5835e-115">-  Warning</span></span>  <br/><span data-ttu-id="5835e-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="5835e-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="5835e-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="5835e-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="5835e-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="5835e-118">**Value**</span></span>|<span data-ttu-id="5835e-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="5835e-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5835e-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="5835e-120">**Success**</span></span> <br/> |<span data-ttu-id="5835e-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="5835e-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="5835e-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="5835e-122">**Warning**</span></span> <br/> | <span data-ttu-id="5835e-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="5835e-123">Describes a request that was not processed.</span></span> <span data-ttu-id="5835e-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="5835e-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="5835e-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="5835e-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="5835e-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="5835e-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="5835e-127">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="5835e-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="5835e-128">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="5835e-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="5835e-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="5835e-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="5835e-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="5835e-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="5835e-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="5835e-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="5835e-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="5835e-132">**Error**</span></span> <br/> | <span data-ttu-id="5835e-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="5835e-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="5835e-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="5835e-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="5835e-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="5835e-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="5835e-136">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="5835e-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="5835e-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="5835e-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="5835e-138">-Un attribut ou un élément n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="5835e-138">-  An attribute or element is not valid in the context</span></span>  <br/><span data-ttu-id="5835e-139">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="5835e-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="5835e-140">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="5835e-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="5835e-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="5835e-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5835e-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5835e-142">Child elements</span></span>

|<span data-ttu-id="5835e-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5835e-143">**Element**</span></span>|<span data-ttu-id="5835e-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="5835e-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5835e-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="5835e-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5835e-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="5835e-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5835e-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5835e-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5835e-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="5835e-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5835e-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5835e-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5835e-150">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="5835e-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="5835e-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="5835e-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5835e-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5835e-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5835e-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="5835e-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="5835e-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="5835e-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="5835e-155">Contient les informations de configuration de service pour le service de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="5835e-155">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="5835e-156">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="5835e-156">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="5835e-157">Contient des informations de configuration de service pour le service de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="5835e-157">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
|[<span data-ttu-id="5835e-158">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5835e-158">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="5835e-159">Contient des informations de configuration de service pour le service de règles de protection.</span><span class="sxs-lookup"><span data-stu-id="5835e-159">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5835e-160">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5835e-160">Parent elements</span></span>

|<span data-ttu-id="5835e-161">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5835e-161">**Element**</span></span>|<span data-ttu-id="5835e-162">**Description**</span><span class="sxs-lookup"><span data-stu-id="5835e-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5835e-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="5835e-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="5835e-164">Contient un tableau de messages de réponse de configuration de service.</span><span class="sxs-lookup"><span data-stu-id="5835e-164">Contains an array of service configuration response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5835e-165">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5835e-165">Text value</span></span>

<span data-ttu-id="5835e-166">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5835e-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5835e-167">Remarques</span><span class="sxs-lookup"><span data-stu-id="5835e-167">Remarks</span></span>

<span data-ttu-id="5835e-168">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5835e-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5835e-169">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5835e-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5835e-170">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5835e-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5835e-171">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5835e-171">Schema Name</span></span>  <br/> |<span data-ttu-id="5835e-172">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="5835e-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5835e-173">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5835e-173">Validation File</span></span>  <br/> |<span data-ttu-id="5835e-174">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5835e-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5835e-175">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5835e-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="5835e-176">False</span><span class="sxs-lookup"><span data-stu-id="5835e-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5835e-177">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5835e-177">See also</span></span>

- [<span data-ttu-id="5835e-178">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5835e-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

