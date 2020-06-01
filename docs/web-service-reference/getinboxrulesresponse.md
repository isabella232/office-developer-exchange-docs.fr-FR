---
title: GetInboxRulesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRulesResponse
api_type:
- schema
ms.assetid: 6d6c1950-c328-489a-94bf-a250fdbd5cd9
description: L’élément GetInboxRulesResponse définit une réponse à une demande d’opération GetInboxRules.
ms.openlocfilehash: 0d67d7eaf6ffbeeb790249190a98f252dbdb9c87
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458284"
---
# <a name="getinboxrulesresponse"></a><span data-ttu-id="b66b9-103">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="b66b9-103">GetInboxRulesResponse</span></span>

<span data-ttu-id="b66b9-104">L’élément **GetInboxRulesResponse** définit une réponse à une demande d' [opération GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b66b9-104">The **GetInboxRulesResponse** element defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span> 
  
```XML
<GetInboxRulesResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <OutlookRuleBlobExists/>
   <InboxRules/>
</GetInboxRulesResponse>
```

 <span data-ttu-id="b66b9-105">**GetInboxRulesResponseType**</span><span class="sxs-lookup"><span data-stu-id="b66b9-105">**GetInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b66b9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b66b9-106">Attributes and elements</span></span>

<span data-ttu-id="b66b9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b66b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b66b9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b66b9-108">Attributes</span></span>

|<span data-ttu-id="b66b9-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b66b9-109">**Attribute**</span></span>|<span data-ttu-id="b66b9-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="b66b9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b66b9-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b66b9-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b66b9-112">Décrit l’état d’une réponse d' [opération GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b66b9-112">Describes the status of a [GetInboxRules operation](getinboxrules-operation.md) response.</span></span> <br/><br/><span data-ttu-id="b66b9-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="b66b9-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="b66b9-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="b66b9-114">-  Success</span></span>  <br/><span data-ttu-id="b66b9-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="b66b9-115">-  Warning</span></span>  <br/><span data-ttu-id="b66b9-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="b66b9-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="b66b9-117">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b66b9-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="b66b9-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="b66b9-118">**Value**</span></span>|<span data-ttu-id="b66b9-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="b66b9-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b66b9-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="b66b9-120">**Success**</span></span> <br/> |<span data-ttu-id="b66b9-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="b66b9-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b66b9-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="b66b9-122">**Warning**</span></span> <br/> | <span data-ttu-id="b66b9-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="b66b9-123">Describes a request that was not processed.</span></span> <span data-ttu-id="b66b9-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="b66b9-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="b66b9-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="b66b9-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="b66b9-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="b66b9-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="b66b9-127">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b66b9-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="b66b9-128">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="b66b9-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="b66b9-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b66b9-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="b66b9-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="b66b9-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="b66b9-131">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="b66b9-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="b66b9-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="b66b9-132">**Error**</span></span> <br/> | <span data-ttu-id="b66b9-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="b66b9-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b66b9-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="b66b9-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b66b9-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="b66b9-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b66b9-136">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="b66b9-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="b66b9-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="b66b9-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="b66b9-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="b66b9-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="b66b9-139">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="b66b9-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b66b9-140">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="b66b9-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="b66b9-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b66b9-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b66b9-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b66b9-142">Child elements</span></span>

|<span data-ttu-id="b66b9-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b66b9-143">**Element**</span></span>|<span data-ttu-id="b66b9-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="b66b9-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b66b9-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="b66b9-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b66b9-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="b66b9-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b66b9-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b66b9-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b66b9-148">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="b66b9-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="b66b9-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b66b9-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b66b9-150">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="b66b9-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="b66b9-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="b66b9-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b66b9-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b66b9-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b66b9-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="b66b9-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b66b9-154">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="b66b9-154">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md) <br/> |<span data-ttu-id="b66b9-155">Indique si un objet blob de règle Microsoft Outlook existe dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b66b9-155">Indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b66b9-156">InboxRules</span><span class="sxs-lookup"><span data-stu-id="b66b9-156">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="b66b9-157">Représente un tableau des règles dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b66b9-157">Represents an array of the rules in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b66b9-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b66b9-158">Parent elements</span></span>

<span data-ttu-id="b66b9-159">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b66b9-159">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b66b9-160">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b66b9-160">Text value</span></span>

<span data-ttu-id="b66b9-161">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b66b9-161">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b66b9-162">Remarques</span><span class="sxs-lookup"><span data-stu-id="b66b9-162">Remarks</span></span>

<span data-ttu-id="b66b9-163">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b66b9-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b66b9-164">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b66b9-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b66b9-165">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b66b9-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b66b9-166">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b66b9-166">Schema name</span></span>  <br/> |<span data-ttu-id="b66b9-167">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b66b9-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b66b9-168">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b66b9-168">Validation file</span></span>  <br/> |<span data-ttu-id="b66b9-169">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b66b9-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b66b9-170">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b66b9-170">Can be empty</span></span>  <br/> |<span data-ttu-id="b66b9-171">False</span><span class="sxs-lookup"><span data-stu-id="b66b9-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b66b9-172">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b66b9-172">See also</span></span>

- [<span data-ttu-id="b66b9-173">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="b66b9-173">GetInboxRules</span></span>](getinboxrules.md)
- [<span data-ttu-id="b66b9-174">Opération de GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="b66b9-174">GetInboxRules operation</span></span>](getinboxrules-operation.md)

