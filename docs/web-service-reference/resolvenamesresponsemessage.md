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
description: L’élément ResolveNamesResponseMessage contient l’État et le résultat d’une demande d’opération ResolveNames.
ms.openlocfilehash: 12f32008dbbc603fca7adf26057f1f1904d3cfb2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455596"
---
# <a name="resolvenamesresponsemessage"></a><span data-ttu-id="42b66-103">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="42b66-103">ResolveNamesResponseMessage</span></span>

<span data-ttu-id="42b66-104">L’élément **ResolveNamesResponseMessage** contient l’État et le résultat d’une demande d' [opération ResolveNames](resolvenames-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="42b66-104">The **ResolveNamesResponseMessage** element contains the status and result of a [ResolveNames operation](resolvenames-operation.md) request.</span></span> 
  
- [<span data-ttu-id="42b66-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="42b66-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md) 
- [<span data-ttu-id="42b66-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="42b66-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="42b66-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="42b66-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 <span data-ttu-id="42b66-108">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="42b66-108">**ResolveNamesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42b66-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="42b66-109">Attributes and elements</span></span>

<span data-ttu-id="42b66-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="42b66-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42b66-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="42b66-111">Attributes</span></span>

|<span data-ttu-id="42b66-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="42b66-112">**Attribute**</span></span>|<span data-ttu-id="42b66-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="42b66-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="42b66-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="42b66-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="42b66-115">Décrit l’état d’une réponse d' [opération ResolveNames](resolvenames-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="42b66-115">Describes the status of a [ResolveNames operation](resolvenames-operation.md) response.</span></span> <br/><br/><span data-ttu-id="42b66-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="42b66-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="42b66-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="42b66-117">-  Success</span></span>  <br/><span data-ttu-id="42b66-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="42b66-118">-  Warning</span></span>  <br/><span data-ttu-id="42b66-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="42b66-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="42b66-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="42b66-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="42b66-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="42b66-121">**Value**</span></span>|<span data-ttu-id="42b66-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="42b66-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="42b66-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="42b66-123">**Success**</span></span> <br/> |<span data-ttu-id="42b66-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="42b66-124">Describes a request that is fulfilled.</span></span> <span data-ttu-id="42b66-125">Cela se produit lorsque le nom demandé n’est pas ambigu et que la réponse contient un seul destinataire.</span><span class="sxs-lookup"><span data-stu-id="42b66-125">This occurs when the requested name is unambiguous and the response contains a single recipient.</span></span>  <br/> |
|<span data-ttu-id="42b66-126">**Warning**</span><span class="sxs-lookup"><span data-stu-id="42b66-126">**Warning**</span></span> <br/> | <span data-ttu-id="42b66-127">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="42b66-127">Describes a request that was not processed.</span></span> <span data-ttu-id="42b66-128">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="42b66-128">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="42b66-129">Voici un exemple de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="42b66-129">The following are example of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="42b66-130">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="42b66-130">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="42b66-131">-Les services de domaine Active Directory (AD DS) sont en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="42b66-131">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="42b66-132">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="42b66-132">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="42b66-133">-La base de données de boîtes aux lettres (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="42b66-133">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="42b66-134">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="42b66-134">-  A password is expired.</span></span>  <br/><span data-ttu-id="42b66-135">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="42b66-135">-  A quota is exceeded.</span></span>  <br/><span data-ttu-id="42b66-136">-Le nom demandé est ambigu et la réponse contient plusieurs destinataires.</span><span class="sxs-lookup"><span data-stu-id="42b66-136">-  The requested name is ambiguous and the response contains multiple recipients.</span></span>  <br/> |
|<span data-ttu-id="42b66-137">**Error**</span><span class="sxs-lookup"><span data-stu-id="42b66-137">**Error**</span></span> <br/> | <span data-ttu-id="42b66-138">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="42b66-138">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="42b66-139">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="42b66-139">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="42b66-140">-Le nom demandé n’a pas pu être résolu.</span><span class="sxs-lookup"><span data-stu-id="42b66-140">-  The requested name could not be resolved.</span></span>  <br/><span data-ttu-id="42b66-141">-Les attributs ou les éléments ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="42b66-141">-  Attributes or elements are invalid.</span></span>  <br/><span data-ttu-id="42b66-142">-Les attributs ou les éléments sont en dehors de la plage.</span><span class="sxs-lookup"><span data-stu-id="42b66-142">-  Attributes or elements are out of range.</span></span>  <br/><span data-ttu-id="42b66-143">-Une balise est inconnue.</span><span class="sxs-lookup"><span data-stu-id="42b66-143">-  A tag is unknown.</span></span>  <br/><span data-ttu-id="42b66-144">-Un attribut ou un élément n’est pas valide dans le contexte.</span><span class="sxs-lookup"><span data-stu-id="42b66-144">-  An attribute or element is not valid in the context.</span></span>  <br/><span data-ttu-id="42b66-145">-Une tentative d’accès non autorisée par un client s’est produite.</span><span class="sxs-lookup"><span data-stu-id="42b66-145">-  An unauthorized access attempt by any client occurred.</span></span>  <br/><span data-ttu-id="42b66-146">-Une erreur côté serveur s’est produite en réponse à un appel côté client valide.</span><span class="sxs-lookup"><span data-stu-id="42b66-146">-  A server-side failure occurred in response to a valid client-side call.</span></span>  <br/>  <br/><span data-ttu-id="42b66-147">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="42b66-147">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="42b66-148">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="42b66-148">Child elements</span></span>

|<span data-ttu-id="42b66-149">**Élément**</span><span class="sxs-lookup"><span data-stu-id="42b66-149">**Element**</span></span>|<span data-ttu-id="42b66-150">**Description**</span><span class="sxs-lookup"><span data-stu-id="42b66-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42b66-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="42b66-151">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="42b66-152">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="42b66-152">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="42b66-153">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="42b66-153">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="42b66-154">Fournit des informations d’erreur sur la demande.</span><span class="sxs-lookup"><span data-stu-id="42b66-154">Provides error information about the request.</span></span>  <br/> |
|[<span data-ttu-id="42b66-155">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="42b66-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="42b66-156">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="42b66-156">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="42b66-157">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="42b66-157">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="42b66-158">MessageXml</span><span class="sxs-lookup"><span data-stu-id="42b66-158">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="42b66-159">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="42b66-159">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="42b66-160">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="42b66-160">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="42b66-161">Contient un tableau de résolutions pour un nom ambigu.</span><span class="sxs-lookup"><span data-stu-id="42b66-161">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="42b66-162">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="42b66-162">Parent elements</span></span>

|<span data-ttu-id="42b66-163">**Élément**</span><span class="sxs-lookup"><span data-stu-id="42b66-163">**Element**</span></span>|<span data-ttu-id="42b66-164">**Description**</span><span class="sxs-lookup"><span data-stu-id="42b66-164">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42b66-165">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="42b66-165">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="42b66-166">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="42b66-166">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="42b66-167">Remarques</span><span class="sxs-lookup"><span data-stu-id="42b66-167">Remarks</span></span>

<span data-ttu-id="42b66-168">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="42b66-168">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42b66-169">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="42b66-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42b66-170">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="42b66-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="42b66-171">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="42b66-171">Schema name</span></span>  <br/> |<span data-ttu-id="42b66-172">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="42b66-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="42b66-173">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="42b66-173">Validation file</span></span>  <br/> |<span data-ttu-id="42b66-174">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="42b66-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="42b66-175">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="42b66-175">Can be empty</span></span>  <br/> |<span data-ttu-id="42b66-176">False</span><span class="sxs-lookup"><span data-stu-id="42b66-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="42b66-177">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="42b66-177">See also</span></span>

- [<span data-ttu-id="42b66-178">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="42b66-178">ResolveNames</span></span>](resolvenames.md)
- [<span data-ttu-id="42b66-179">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="42b66-179">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
- [<span data-ttu-id="42b66-180">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="42b66-180">ResolveNames operation</span></span>](resolvenames-operation.md)

