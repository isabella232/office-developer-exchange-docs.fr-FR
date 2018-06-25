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
description: L’élément ServiceConfigurationResponseMessageType contient les paramètres de configuration de service.
ms.openlocfilehash: fb7841f346083017319cece4479fea8bbfb6de17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829393"
---
# <a name="serviceconfigurationresponsemessagetype"></a><span data-ttu-id="63468-103">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="63468-103">ServiceConfigurationResponseMessageType</span></span>

<span data-ttu-id="63468-104">L’élément **ServiceConfigurationResponseMessageType** contient les paramètres de configuration de service.</span><span class="sxs-lookup"><span data-stu-id="63468-104">The **ServiceConfigurationResponseMessageType** element contains service configuration settings.</span></span> 
  
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

 <span data-ttu-id="63468-105">**ServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="63468-105">**ServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63468-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="63468-106">Attributes and elements</span></span>

<span data-ttu-id="63468-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="63468-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63468-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="63468-108">Attributes</span></span>

|<span data-ttu-id="63468-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="63468-109">**Attribute**</span></span>|<span data-ttu-id="63468-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="63468-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63468-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="63468-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="63468-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="63468-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="63468-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="63468-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="63468-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="63468-114">-  Success</span></span>  <br/><span data-ttu-id="63468-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="63468-115">-  Warning</span></span>  <br/><span data-ttu-id="63468-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="63468-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="63468-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="63468-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="63468-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="63468-118">**Value**</span></span>|<span data-ttu-id="63468-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="63468-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63468-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="63468-120">**Success**</span></span> <br/> |<span data-ttu-id="63468-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="63468-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="63468-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="63468-122">**Warning**</span></span> <br/> | <span data-ttu-id="63468-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="63468-123">Describes a request that was not processed.</span></span> <span data-ttu-id="63468-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="63468-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="63468-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="63468-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="63468-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="63468-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="63468-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="63468-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="63468-128">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="63468-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="63468-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="63468-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="63468-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="63468-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="63468-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="63468-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="63468-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="63468-132">**Error**</span></span> <br/> | <span data-ttu-id="63468-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="63468-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="63468-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="63468-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="63468-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="63468-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="63468-136">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="63468-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="63468-137">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="63468-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="63468-138">-Un attribut ou un élément n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="63468-138">-  An attribute or element is not valid in the context</span></span>  <br/><span data-ttu-id="63468-139">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="63468-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="63468-140">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="63468-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="63468-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="63468-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="63468-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="63468-142">Child elements</span></span>

|<span data-ttu-id="63468-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="63468-143">**Element**</span></span>|<span data-ttu-id="63468-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="63468-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63468-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="63468-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="63468-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="63468-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="63468-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="63468-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="63468-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="63468-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="63468-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="63468-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="63468-150">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="63468-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="63468-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="63468-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="63468-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="63468-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="63468-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="63468-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="63468-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="63468-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="63468-155">Contient des informations de configuration de service pour le service de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="63468-155">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="63468-156">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="63468-156">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="63468-157">Contient des informations de configuration de service pour le service de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="63468-157">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
|[<span data-ttu-id="63468-158">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="63468-158">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="63468-159">Contient des informations de configuration de service pour le service de règles de protection.</span><span class="sxs-lookup"><span data-stu-id="63468-159">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63468-160">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="63468-160">Parent elements</span></span>

|<span data-ttu-id="63468-161">**Élément**</span><span class="sxs-lookup"><span data-stu-id="63468-161">**Element**</span></span>|<span data-ttu-id="63468-162">**Description**</span><span class="sxs-lookup"><span data-stu-id="63468-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63468-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="63468-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="63468-164">Contient un tableau de messages de réponse de configuration de service.</span><span class="sxs-lookup"><span data-stu-id="63468-164">Contains an array of service configuration response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63468-165">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="63468-165">Text value</span></span>

<span data-ttu-id="63468-166">Aucun.</span><span class="sxs-lookup"><span data-stu-id="63468-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63468-167">Remarques</span><span class="sxs-lookup"><span data-stu-id="63468-167">Remarks</span></span>

<span data-ttu-id="63468-168">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="63468-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63468-169">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="63468-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63468-170">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="63468-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="63468-171">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="63468-171">Schema Name</span></span>  <br/> |<span data-ttu-id="63468-172">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="63468-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="63468-173">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="63468-173">Validation File</span></span>  <br/> |<span data-ttu-id="63468-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="63468-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="63468-175">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="63468-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="63468-176">False</span><span class="sxs-lookup"><span data-stu-id="63468-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63468-177">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="63468-177">See also</span></span>

- [<span data-ttu-id="63468-178">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="63468-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

