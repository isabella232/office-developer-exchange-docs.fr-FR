---
title: ResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessage
api_type:
- schema
ms.assetid: bf57265a-d354-4cd7-bbfc-d93e19cbede6
description: L’élément ResponseMessage fournit des informations descriptives concernant l’état de réponse pour une entité dans une demande unique.
ms.openlocfilehash: 69f1f6f12d10044045b72dd644536e742c479b9e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829191"
---
# <a name="responsemessage"></a><span data-ttu-id="1c163-103">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1c163-103">ResponseMessage</span></span>

<span data-ttu-id="1c163-104">L’élément **ResponseMessage** fournit des informations descriptives concernant l’état de réponse pour une entité dans une demande unique.</span><span class="sxs-lookup"><span data-stu-id="1c163-104">The **ResponseMessage** element provides descriptive information about the response status for a single entity within a request.</span></span> 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 <span data-ttu-id="1c163-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c163-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1c163-106">Attributes and elements</span></span>

<span data-ttu-id="1c163-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1c163-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c163-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1c163-108">Attributes</span></span>

|<span data-ttu-id="1c163-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1c163-109">**Attribute**</span></span>|<span data-ttu-id="1c163-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="1c163-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1c163-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="1c163-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1c163-112">Représente l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="1c163-112">Represents the status of the response.</span></span> <br/><br/><span data-ttu-id="1c163-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="1c163-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="1c163-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="1c163-114">-  Success</span></span>  <br/><span data-ttu-id="1c163-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="1c163-115">-  Warning</span></span>  <br/><span data-ttu-id="1c163-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="1c163-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="1c163-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="1c163-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="1c163-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1c163-118">**Value**</span></span>|<span data-ttu-id="1c163-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="1c163-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1c163-120">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="1c163-120">Success</span></span>  <br/> |<span data-ttu-id="1c163-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="1c163-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1c163-122">Avertissement</span><span class="sxs-lookup"><span data-stu-id="1c163-122">Warning</span></span>  <br/> | <span data-ttu-id="1c163-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="1c163-123">Describes a request that was not processed.</span></span> <span data-ttu-id="1c163-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="1c163-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="1c163-125">Voici quelques causes possibles pour les avertissements :</span><span class="sxs-lookup"><span data-stu-id="1c163-125">The following are some possible causes for warnings:</span></span>  <br/><br/><span data-ttu-id="1c163-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="1c163-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="1c163-127">-Le service d’annuaire Active Directory est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1c163-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="1c163-128">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="1c163-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="1c163-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1c163-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="1c163-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="1c163-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="1c163-131">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="1c163-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="1c163-132">Erreur</span><span class="sxs-lookup"><span data-stu-id="1c163-132">Error</span></span>  <br/> | <span data-ttu-id="1c163-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="1c163-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="1c163-134">Voici quelques causes possibles des erreurs :</span><span class="sxs-lookup"><span data-stu-id="1c163-134">The following are some possible causes for errors:</span></span>  <br/><br/><span data-ttu-id="1c163-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="1c163-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="1c163-136">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="1c163-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="1c163-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="1c163-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="1c163-138">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="1c163-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="1c163-139">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="1c163-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="1c163-140">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="1c163-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="1c163-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="1c163-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1c163-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1c163-142">Child elements</span></span>

|<span data-ttu-id="1c163-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1c163-143">**Element**</span></span>|<span data-ttu-id="1c163-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="1c163-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c163-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="1c163-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1c163-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="1c163-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1c163-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1c163-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1c163-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="1c163-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1c163-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1c163-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1c163-150">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="1c163-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="1c163-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="1c163-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1c163-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1c163-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1c163-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="1c163-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1c163-154">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1c163-154">Parent elements</span></span>

|<span data-ttu-id="1c163-155">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1c163-155">**Element**</span></span>|<span data-ttu-id="1c163-156">**Description**</span><span class="sxs-lookup"><span data-stu-id="1c163-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c163-157">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="1c163-157">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="1c163-158">Contient les informations de disponibilité pour un utilisateur de boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="1c163-158">Contains the free/busy information for a single mailbox user.</span></span> <br/> <br/> <span data-ttu-id="1c163-159">Vous trouverez ci-dessous l’expression XPath 2.0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="1c163-159">The following is the XPath 2.0 expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[<span data-ttu-id="1c163-160">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="1c163-160">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="1c163-161">Contient des données d’informations et suggestion de réponse de demande de suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="1c163-161">Contains response information and suggestion data for requested meeting suggestions.</span></span>  <br/><br/> <span data-ttu-id="1c163-162">Vous trouverez ci-dessous l’expression XPath 2.0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="1c163-162">The following is the XPath 2.0 expression to this element:</span></span><br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[<span data-ttu-id="1c163-163">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="1c163-163">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="1c163-164">Contient les résultats de la réponse et les paramètres d’absence du bureau pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1c163-164">Contains the response results and the OOF settings for a user.</span></span>  <br/><br/> <span data-ttu-id="1c163-165">Vous trouverez ci-dessous l’expression XPath 2.0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="1c163-165">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[<span data-ttu-id="1c163-166">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="1c163-166">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md) <br/> |<span data-ttu-id="1c163-167">Contient le résultat d’un message [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) a été lancée.</span><span class="sxs-lookup"><span data-stu-id="1c163-167">Contains the result of an attempted [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message.</span></span> <br/> <br/> <span data-ttu-id="1c163-168">Vous trouverez ci-dessous l’expression XPath 2.0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="1c163-168">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1c163-169">Remarques</span><span class="sxs-lookup"><span data-stu-id="1c163-169">Remarks</span></span>

<span data-ttu-id="1c163-170">Le type de **ResponseMessageType** est commun à toutes les réponses des Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c163-170">The **ResponseMessageType** type is common to all Exchange Web Services responses.</span></span> <span data-ttu-id="1c163-171">Le type **ResponseMessageType** est étendu par les types complexes suivants :</span><span class="sxs-lookup"><span data-stu-id="1c163-171">The **ResponseMessageType** type is extended by the following complex types:</span></span> 
  
- <span data-ttu-id="1c163-172">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-172">**ApplyConversationActionResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-173">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-173">**AttachmentInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-174">**DeleteAttachmentResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-174">**DeleteAttachmentResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-175">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-175">**DeleteItemResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-176">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-176">**ExpandDLResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-177">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-177">**FindFolderResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-178">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-178">**FindItemResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-179">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-179">**FolderInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-180">**GetEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-180">**GetEventsResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-181">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-181">**ItemInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-182">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-182">**ResolveNamesResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-183">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-183">**SubscribeResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-184">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-184">**SendNotificationResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-185">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-185">**SyncFolderHierarchyResponseMessageType**</span></span>
    
- <span data-ttu-id="1c163-186">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1c163-186">**SyncFolderItemsResponseMessageType**</span></span>
    
<span data-ttu-id="1c163-187">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1c163-187">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="1c163-188">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="1c163-188">Version differences</span></span>

<span data-ttu-id="1c163-189">Les types **ApplyConversationActionResponseMessage** et **DeleteItemResponseMessageType** ont été introduites dans Exchange version 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="1c163-189">The **ApplyConversationActionResponseMessage** and **DeleteItemResponseMessageType** types were introduced in Exchange build 15.00.0986.00.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="1c163-190">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1c163-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c163-191">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1c163-191">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1c163-192">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1c163-192">Schema Name</span></span>  <br/> |<span data-ttu-id="1c163-193">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1c163-193">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1c163-194">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1c163-194">Validation File</span></span>  <br/> |<span data-ttu-id="1c163-195">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1c163-195">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1c163-196">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1c163-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="1c163-197">False</span><span class="sxs-lookup"><span data-stu-id="1c163-197">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c163-198">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1c163-198">See also</span></span>

- [<span data-ttu-id="1c163-199">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="1c163-199">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="1c163-200">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="1c163-200">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="1c163-201">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="1c163-201">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="1c163-202">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="1c163-202">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
