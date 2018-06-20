---
title: ResolveNamesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNamesResponseMessage
api_type:
- schema
ms.assetid: edcdaf58-ef63-412e-8c58-409213e6ab0d
description: L’élément ResolveNamesResponseMessage contient l’état et les résultats d’une demande d’opération ResolveNames.
ms.openlocfilehash: 953a1f0b19c078d969ffe175c22df02b58c5e939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829170"
---
# <a name="resolvenamesresponsemessage"></a><span data-ttu-id="29386-103">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="29386-103">ResolveNamesResponseMessage</span></span>

<span data-ttu-id="29386-104">L’élément **ResolveNamesResponseMessage** contient l’état et les résultats d’une demande [d’opération ResolveNames](resolvenames-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="29386-104">The **ResolveNamesResponseMessage** element contains the status and result of a [ResolveNames operation](resolvenames-operation.md) request.</span></span> 
  
- [<span data-ttu-id="29386-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="29386-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md) 
- [<span data-ttu-id="29386-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="29386-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="29386-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="29386-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 <span data-ttu-id="29386-108">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="29386-108">**ResolveNamesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29386-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="29386-109">Attributes and elements</span></span>

<span data-ttu-id="29386-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="29386-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29386-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="29386-111">Attributes</span></span>

|<span data-ttu-id="29386-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="29386-112">**Attribute**</span></span>|<span data-ttu-id="29386-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="29386-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="29386-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="29386-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="29386-115">Décrit l’état d’une réponse de [l’opération ResolveNames](resolvenames-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="29386-115">Describes the status of a [ResolveNames operation](resolvenames-operation.md) response.</span></span> <br/><br/><span data-ttu-id="29386-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="29386-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="29386-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="29386-117">-  Success</span></span>  <br/><span data-ttu-id="29386-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="29386-118">-  Warning</span></span>  <br/><span data-ttu-id="29386-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="29386-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="29386-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="29386-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="29386-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="29386-121">**Value**</span></span>|<span data-ttu-id="29386-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="29386-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="29386-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="29386-123">**Success**</span></span> <br/> |<span data-ttu-id="29386-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="29386-124">Describes a request that is fulfilled.</span></span> <span data-ttu-id="29386-125">Cela se produit lorsque le nom demandé est non ambigu et la réponse contient un destinataire unique.</span><span class="sxs-lookup"><span data-stu-id="29386-125">This occurs when the requested name is unambiguous and the response contains a single recipient.</span></span>  <br/> |
|<span data-ttu-id="29386-126">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="29386-126">**Warning**</span></span> <br/> | <span data-ttu-id="29386-127">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="29386-127">Describes a request that was not processed.</span></span> <span data-ttu-id="29386-128">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="29386-128">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="29386-129">Exemple de sources des avertissements sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="29386-129">The following are example of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="29386-130">-La banque d’informations Exchange est déconnecté pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="29386-130">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="29386-131">-Services de domaine actives Directory (AD DS) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="29386-131">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="29386-132">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="29386-132">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="29386-133">-La base de données de boîtes aux lettres (MDB) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="29386-133">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="29386-134">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="29386-134">-  A password is expired.</span></span>  <br/><span data-ttu-id="29386-135">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="29386-135">-  A quota is exceeded.</span></span>  <br/><span data-ttu-id="29386-136">-Le nom demandé est ambigu et la réponse contient plusieurs destinataires.</span><span class="sxs-lookup"><span data-stu-id="29386-136">-  The requested name is ambiguous and the response contains multiple recipients.</span></span>  <br/> |
|<span data-ttu-id="29386-137">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="29386-137">**Error**</span></span> <br/> | <span data-ttu-id="29386-138">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="29386-138">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="29386-139">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="29386-139">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="29386-140">-Le nom demandé n’a pas pu être résolu.</span><span class="sxs-lookup"><span data-stu-id="29386-140">-  The requested name could not be resolved.</span></span>  <br/><span data-ttu-id="29386-141">-Attributs ou éléments ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="29386-141">-  Attributes or elements are invalid.</span></span>  <br/><span data-ttu-id="29386-142">-Attributs ou éléments sont hors de portée.</span><span class="sxs-lookup"><span data-stu-id="29386-142">-  Attributes or elements are out of range.</span></span>  <br/><span data-ttu-id="29386-143">-Une balise est inconnue.</span><span class="sxs-lookup"><span data-stu-id="29386-143">-  A tag is unknown.</span></span>  <br/><span data-ttu-id="29386-144">-Un attribut ou un élément n’est pas valide dans le contexte.</span><span class="sxs-lookup"><span data-stu-id="29386-144">-  An attribute or element is not valid in the context.</span></span>  <br/><span data-ttu-id="29386-145">-Une tentative d’accès non autorisés par n’importe quel client s’est produite.</span><span class="sxs-lookup"><span data-stu-id="29386-145">-  An unauthorized access attempt by any client occurred.</span></span>  <br/><span data-ttu-id="29386-146">-Une défaillance du côté serveur s’est produite en réponse à un appel côté client valid.</span><span class="sxs-lookup"><span data-stu-id="29386-146">-  A server-side failure occurred in response to a valid client-side call.</span></span>  <br/>  <br/><span data-ttu-id="29386-147">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="29386-147">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="29386-148">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="29386-148">Child elements</span></span>

|<span data-ttu-id="29386-149">**Élément**</span><span class="sxs-lookup"><span data-stu-id="29386-149">**Element**</span></span>|<span data-ttu-id="29386-150">**Description**</span><span class="sxs-lookup"><span data-stu-id="29386-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29386-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="29386-151">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="29386-152">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="29386-152">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="29386-153">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="29386-153">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="29386-154">Fournit des informations sur la demande.</span><span class="sxs-lookup"><span data-stu-id="29386-154">Provides error information about the request.</span></span>  <br/> |
|[<span data-ttu-id="29386-155">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="29386-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="29386-156">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="29386-156">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="29386-157">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="29386-157">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="29386-158">MessageXml</span><span class="sxs-lookup"><span data-stu-id="29386-158">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="29386-159">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="29386-159">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="29386-160">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="29386-160">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="29386-161">Contient un tableau des résolutions pour un nom ambigu.</span><span class="sxs-lookup"><span data-stu-id="29386-161">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29386-162">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="29386-162">Parent elements</span></span>

|<span data-ttu-id="29386-163">**Élément**</span><span class="sxs-lookup"><span data-stu-id="29386-163">**Element**</span></span>|<span data-ttu-id="29386-164">**Description**</span><span class="sxs-lookup"><span data-stu-id="29386-164">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29386-165">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="29386-165">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="29386-166">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="29386-166">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="29386-167">Remarques</span><span class="sxs-lookup"><span data-stu-id="29386-167">Remarks</span></span>

<span data-ttu-id="29386-168">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="29386-168">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29386-169">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="29386-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29386-170">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="29386-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="29386-171">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="29386-171">Schema name</span></span>  <br/> |<span data-ttu-id="29386-172">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="29386-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="29386-173">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="29386-173">Validation file</span></span>  <br/> |<span data-ttu-id="29386-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="29386-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="29386-175">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="29386-175">Can be empty</span></span>  <br/> |<span data-ttu-id="29386-176">False</span><span class="sxs-lookup"><span data-stu-id="29386-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29386-177">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="29386-177">See also</span></span>

- [<span data-ttu-id="29386-178">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="29386-178">ResolveNames</span></span>](resolvenames.md)
- [<span data-ttu-id="29386-179">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="29386-179">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
- [<span data-ttu-id="29386-180">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="29386-180">ResolveNames operation</span></span>](resolvenames-operation.md)

