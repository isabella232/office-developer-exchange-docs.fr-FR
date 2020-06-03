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
description: L’élément ResponseMessage fournit des informations descriptives sur l’état de réponse d’une entité unique dans une demande.
ms.openlocfilehash: a7f4240b1e988cb69d67118c6db58db0d7babba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467157"
---
# <a name="responsemessage"></a><span data-ttu-id="40dae-103">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="40dae-103">ResponseMessage</span></span>

<span data-ttu-id="40dae-104">L’élément **ResponseMessage** fournit des informations descriptives sur l’état de réponse d’une entité unique dans une demande.</span><span class="sxs-lookup"><span data-stu-id="40dae-104">The **ResponseMessage** element provides descriptive information about the response status for a single entity within a request.</span></span> 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 <span data-ttu-id="40dae-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40dae-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="40dae-106">Attributes and elements</span></span>

<span data-ttu-id="40dae-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="40dae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40dae-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="40dae-108">Attributes</span></span>

|<span data-ttu-id="40dae-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="40dae-109">**Attribute**</span></span>|<span data-ttu-id="40dae-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="40dae-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="40dae-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="40dae-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="40dae-112">Représente l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="40dae-112">Represents the status of the response.</span></span> <br/><br/><span data-ttu-id="40dae-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="40dae-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="40dae-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="40dae-114">-  Success</span></span>  <br/><span data-ttu-id="40dae-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="40dae-115">-  Warning</span></span>  <br/><span data-ttu-id="40dae-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="40dae-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="40dae-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="40dae-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="40dae-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="40dae-118">**Value**</span></span>|<span data-ttu-id="40dae-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="40dae-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="40dae-120">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="40dae-120">Success</span></span>  <br/> |<span data-ttu-id="40dae-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="40dae-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="40dae-122">Avertissement</span><span class="sxs-lookup"><span data-stu-id="40dae-122">Warning</span></span>  <br/> | <span data-ttu-id="40dae-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="40dae-123">Describes a request that was not processed.</span></span> <span data-ttu-id="40dae-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="40dae-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="40dae-125">Voici quelques causes possibles des avertissements :</span><span class="sxs-lookup"><span data-stu-id="40dae-125">The following are some possible causes for warnings:</span></span>  <br/><br/><span data-ttu-id="40dae-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="40dae-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="40dae-127">-Le service d’annuaire Active Directory est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="40dae-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="40dae-128">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="40dae-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="40dae-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="40dae-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="40dae-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="40dae-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="40dae-131">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="40dae-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="40dae-132">Erreur</span><span class="sxs-lookup"><span data-stu-id="40dae-132">Error</span></span>  <br/> | <span data-ttu-id="40dae-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="40dae-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="40dae-134">Voici quelques causes possibles des erreurs :</span><span class="sxs-lookup"><span data-stu-id="40dae-134">The following are some possible causes for errors:</span></span>  <br/><br/><span data-ttu-id="40dae-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="40dae-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="40dae-136">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="40dae-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="40dae-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="40dae-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="40dae-138">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="40dae-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="40dae-139">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="40dae-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="40dae-140">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="40dae-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="40dae-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="40dae-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="40dae-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="40dae-142">Child elements</span></span>

|<span data-ttu-id="40dae-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="40dae-143">**Element**</span></span>|<span data-ttu-id="40dae-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="40dae-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40dae-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="40dae-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="40dae-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="40dae-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="40dae-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="40dae-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="40dae-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="40dae-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="40dae-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="40dae-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="40dae-150">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="40dae-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="40dae-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="40dae-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="40dae-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="40dae-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="40dae-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="40dae-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="40dae-154">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="40dae-154">Parent elements</span></span>

|<span data-ttu-id="40dae-155">**Élément**</span><span class="sxs-lookup"><span data-stu-id="40dae-155">**Element**</span></span>|<span data-ttu-id="40dae-156">**Description**</span><span class="sxs-lookup"><span data-stu-id="40dae-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40dae-157">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="40dae-157">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="40dae-158">Contient les informations de disponibilité pour un utilisateur de boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="40dae-158">Contains the free/busy information for a single mailbox user.</span></span> <br/> <br/> <span data-ttu-id="40dae-159">Voici l’expression XPath 2,0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="40dae-159">The following is the XPath 2.0 expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[<span data-ttu-id="40dae-160">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="40dae-160">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="40dae-161">Contient des informations de réponse et des suggestions de données pour les suggestions de réunion demandées.</span><span class="sxs-lookup"><span data-stu-id="40dae-161">Contains response information and suggestion data for requested meeting suggestions.</span></span>  <br/><br/> <span data-ttu-id="40dae-162">Voici l’expression XPath 2,0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="40dae-162">The following is the XPath 2.0 expression to this element:</span></span><br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[<span data-ttu-id="40dae-163">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="40dae-163">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="40dae-164">Contient les résultats de la réponse et les paramètres OOF d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="40dae-164">Contains the response results and the OOF settings for a user.</span></span>  <br/><br/> <span data-ttu-id="40dae-165">Voici l’expression XPath 2,0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="40dae-165">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[<span data-ttu-id="40dae-166">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="40dae-166">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md) <br/> |<span data-ttu-id="40dae-167">Contient le résultat d’un message de tentative de [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="40dae-167">Contains the result of an attempted [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message.</span></span> <br/> <br/> <span data-ttu-id="40dae-168">Voici l’expression XPath 2,0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="40dae-168">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="40dae-169">Remarques</span><span class="sxs-lookup"><span data-stu-id="40dae-169">Remarks</span></span>

<span data-ttu-id="40dae-170">Le type **ResponseMessageType** est commun à toutes les réponses des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="40dae-170">The **ResponseMessageType** type is common to all Exchange Web Services responses.</span></span> <span data-ttu-id="40dae-171">Le type **ResponseMessageType** est étendu par les types complexes suivants :</span><span class="sxs-lookup"><span data-stu-id="40dae-171">The **ResponseMessageType** type is extended by the following complex types:</span></span> 
  
- <span data-ttu-id="40dae-172">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-172">**ApplyConversationActionResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-173">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-173">**AttachmentInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-174">**DeleteAttachmentResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-174">**DeleteAttachmentResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-175">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-175">**DeleteItemResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-176">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-176">**ExpandDLResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-177">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-177">**FindFolderResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-178">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-178">**FindItemResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-179">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-179">**FolderInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-180">**GetEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-180">**GetEventsResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-181">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-181">**ItemInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-182">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-182">**ResolveNamesResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-183">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-183">**SubscribeResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-184">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-184">**SendNotificationResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-185">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-185">**SyncFolderHierarchyResponseMessageType**</span></span>
    
- <span data-ttu-id="40dae-186">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="40dae-186">**SyncFolderItemsResponseMessageType**</span></span>
    
<span data-ttu-id="40dae-187">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="40dae-187">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="40dae-188">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="40dae-188">Version differences</span></span>

<span data-ttu-id="40dae-189">Les types **ApplyConversationActionResponseMessage** et **DeleteItemResponseMessageType** ont été introduits dans Exchange Build 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="40dae-189">The **ApplyConversationActionResponseMessage** and **DeleteItemResponseMessageType** types were introduced in Exchange build 15.00.0986.00.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="40dae-190">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="40dae-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40dae-191">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="40dae-191">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="40dae-192">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="40dae-192">Schema Name</span></span>  <br/> |<span data-ttu-id="40dae-193">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="40dae-193">Messages schema</span></span>  <br/> |
|<span data-ttu-id="40dae-194">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="40dae-194">Validation File</span></span>  <br/> |<span data-ttu-id="40dae-195">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="40dae-195">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="40dae-196">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="40dae-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="40dae-197">False</span><span class="sxs-lookup"><span data-stu-id="40dae-197">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40dae-198">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="40dae-198">See also</span></span>

- [<span data-ttu-id="40dae-199">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="40dae-199">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="40dae-200">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="40dae-200">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="40dae-201">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="40dae-201">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="40dae-202">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="40dae-202">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

