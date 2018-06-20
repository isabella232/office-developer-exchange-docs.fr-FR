---
title: DeleteItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemResponseMessage
api_type:
- schema
ms.assetid: c3d34c4d-8d83-4612-aa9e-66f9cc7314df
description: L’élément DeleteItemResponseMessage contient l’état et les résultats d’une demande d’opération DeleteItem unique.
ms.openlocfilehash: 1f0cc3d49bfa5fba6da32cf65df6b6718ccfbded
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755881"
---
# <a name="deleteitemresponsemessage"></a><span data-ttu-id="31fa2-103">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="31fa2-103">DeleteItemResponseMessage</span></span>

<span data-ttu-id="31fa2-104">L’élément **DeleteItemResponseMessage** contient l’état et les résultats d’une seule demande [d’opération DeleteItem](deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="31fa2-104">The **DeleteItemResponseMessage** element contains the status and result of a single [DeleteItem operation](deleteitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="31fa2-105">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="31fa2-105">DeleteItemResponse</span></span>](deleteitemresponse.md) 
- [<span data-ttu-id="31fa2-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="31fa2-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="31fa2-107">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="31fa2-107">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
  
```xml
<DeleteItemResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteItemResponseMessage>
```

 <span data-ttu-id="31fa2-108">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="31fa2-108">**DeleteItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31fa2-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="31fa2-109">Attributes and elements</span></span>

<span data-ttu-id="31fa2-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="31fa2-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31fa2-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="31fa2-111">Attributes</span></span>

|<span data-ttu-id="31fa2-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="31fa2-112">**Attribute**</span></span>|<span data-ttu-id="31fa2-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="31fa2-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="31fa2-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="31fa2-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="31fa2-115">Décrit l’état d’une réponse de [l’opération DeleteItem](deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="31fa2-115">Describes the status of a [DeleteItem operation](deleteitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="31fa2-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="31fa2-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="31fa2-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="31fa2-117">- Success</span></span>  <br/><span data-ttu-id="31fa2-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="31fa2-118">-  Warning</span></span>  <br/><span data-ttu-id="31fa2-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="31fa2-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="31fa2-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="31fa2-120">ResponseClass attribute</span></span>

|<span data-ttu-id="31fa2-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="31fa2-121">**Value**</span></span>|<span data-ttu-id="31fa2-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="31fa2-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="31fa2-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="31fa2-123">**Success**</span></span> <br/> |<span data-ttu-id="31fa2-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="31fa2-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="31fa2-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="31fa2-125">**Warning**</span></span> <br/> | <span data-ttu-id="31fa2-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="31fa2-126">Describes a request that was not processed.</span></span> <span data-ttu-id="31fa2-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="31fa2-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="31fa2-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="31fa2-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="31fa2-129">-La banque d’informations Exchange est déconnecté pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="31fa2-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="31fa2-130">-Services de domaine actives Directory (AD DS) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="31fa2-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="31fa2-131">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="31fa2-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="31fa2-132">-La base de données de message (MDB) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="31fa2-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="31fa2-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="31fa2-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="31fa2-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="31fa2-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="31fa2-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="31fa2-135">**Error**</span></span> <br/> | <span data-ttu-id="31fa2-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="31fa2-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="31fa2-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="31fa2-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="31fa2-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="31fa2-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="31fa2-139">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="31fa2-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="31fa2-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="31fa2-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="31fa2-141">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="31fa2-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="31fa2-142">-Un client tentez de définir le niveau de journalisation erreur au-dessus du niveau maximal qui est autorisé par l’administrateur</span><span class="sxs-lookup"><span data-stu-id="31fa2-142">-  A client attempt to set the error logging level above the maximum level that is permitted by the administrator</span></span>  <br/><span data-ttu-id="31fa2-143">-Une tentative de client pour définir le niveau d’échec de gravité au-dessous du niveau par défaut qui est spécifié par l’administrateur</span><span class="sxs-lookup"><span data-stu-id="31fa2-143">-  A client attempt to set the severity failure level below the default level that is specified by the administrator</span></span>  <br/><span data-ttu-id="31fa2-144">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="31fa2-144">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="31fa2-145">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="31fa2-145">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="31fa2-146">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="31fa2-146">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="31fa2-147">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="31fa2-147">Child elements</span></span>

|<span data-ttu-id="31fa2-148">**Élément**</span><span class="sxs-lookup"><span data-stu-id="31fa2-148">**Element**</span></span>|<span data-ttu-id="31fa2-149">**Description**</span><span class="sxs-lookup"><span data-stu-id="31fa2-149">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31fa2-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="31fa2-150">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="31fa2-151">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="31fa2-151">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="31fa2-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="31fa2-152">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="31fa2-153">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="31fa2-153">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="31fa2-154">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="31fa2-154">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="31fa2-155">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="31fa2-155">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="31fa2-156">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="31fa2-156">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="31fa2-157">MessageXml</span><span class="sxs-lookup"><span data-stu-id="31fa2-157">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="31fa2-158">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="31fa2-158">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="31fa2-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="31fa2-159">Parent elements</span></span>

|<span data-ttu-id="31fa2-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="31fa2-160">**Element**</span></span>|<span data-ttu-id="31fa2-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="31fa2-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31fa2-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="31fa2-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="31fa2-163">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="31fa2-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="31fa2-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="31fa2-164">Remarks</span></span>

<span data-ttu-id="31fa2-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="31fa2-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="31fa2-166">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="31fa2-166">Version differences</span></span>

<span data-ttu-id="31fa2-167">Dans les versions d’Exchange commençant par version 15.00.0986.00, l’élément **DeleteItemResponseMessage** est de type **DeleteItemResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="31fa2-167">In versions of Exchange starting with build 15.00.0986.00, the **DeleteItemResponseMessage** element is of type **DeleteItemResponseMessageType**.</span></span> <span data-ttu-id="31fa2-168">Dans les versions précédentes, l’élément est de type **ResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="31fa2-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31fa2-169">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="31fa2-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31fa2-170">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="31fa2-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="31fa2-171">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="31fa2-171">Schema Name</span></span>  <br/> |<span data-ttu-id="31fa2-172">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="31fa2-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="31fa2-173">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="31fa2-173">Validation File</span></span>  <br/> |<span data-ttu-id="31fa2-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="31fa2-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="31fa2-175">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="31fa2-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="31fa2-176">False</span><span class="sxs-lookup"><span data-stu-id="31fa2-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31fa2-177">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="31fa2-177">See also</span></span>

- [<span data-ttu-id="31fa2-178">Opération DeleteItem</span><span class="sxs-lookup"><span data-stu-id="31fa2-178">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="31fa2-179">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="31fa2-179">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="31fa2-180">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="31fa2-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="31fa2-181">Suppression d’éléments (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="31fa2-181">Deleting Items (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

