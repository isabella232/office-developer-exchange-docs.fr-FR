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
ms.openlocfilehash: d84064ab777fe13ded7727381842ddd1ee9d047d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756657"
---
# <a name="getinboxrulesresponse"></a><span data-ttu-id="92094-103">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="92094-103">GetInboxRulesResponse</span></span>

<span data-ttu-id="92094-104">L’élément **GetInboxRulesResponse** définit une réponse à une demande [d’opération GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="92094-104">The **GetInboxRulesResponse** element defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="92094-105">**GetInboxRulesResponseType**</span><span class="sxs-lookup"><span data-stu-id="92094-105">**GetInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92094-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="92094-106">Attributes and elements</span></span>

<span data-ttu-id="92094-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="92094-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92094-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="92094-108">Attributes</span></span>

|<span data-ttu-id="92094-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="92094-109">**Attribute**</span></span>|<span data-ttu-id="92094-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="92094-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="92094-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="92094-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="92094-112">Décrit l’état d’une réponse de [l’opération GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="92094-112">Describes the status of a [GetInboxRules operation](getinboxrules-operation.md) response.</span></span> <br/><br/><span data-ttu-id="92094-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="92094-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="92094-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="92094-114">-  Success</span></span>  <br/><span data-ttu-id="92094-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="92094-115">-  Warning</span></span>  <br/><span data-ttu-id="92094-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="92094-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="92094-117">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="92094-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="92094-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="92094-118">**Value**</span></span>|<span data-ttu-id="92094-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="92094-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="92094-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="92094-120">**Success**</span></span> <br/> |<span data-ttu-id="92094-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="92094-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="92094-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="92094-122">**Warning**</span></span> <br/> | <span data-ttu-id="92094-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="92094-123">Describes a request that was not processed.</span></span> <span data-ttu-id="92094-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="92094-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="92094-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="92094-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="92094-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="92094-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="92094-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="92094-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="92094-128">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="92094-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="92094-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="92094-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="92094-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="92094-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="92094-131">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="92094-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="92094-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="92094-132">**Error**</span></span> <br/> | <span data-ttu-id="92094-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="92094-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="92094-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="92094-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="92094-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="92094-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="92094-136">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="92094-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="92094-137">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="92094-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="92094-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="92094-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="92094-139">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="92094-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="92094-140">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="92094-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="92094-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="92094-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="92094-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="92094-142">Child elements</span></span>

|<span data-ttu-id="92094-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="92094-143">**Element**</span></span>|<span data-ttu-id="92094-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="92094-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92094-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="92094-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="92094-146">Fournit le texte de description de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="92094-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="92094-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="92094-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="92094-148">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="92094-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="92094-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="92094-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="92094-150">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="92094-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="92094-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="92094-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="92094-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="92094-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="92094-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="92094-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="92094-154">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="92094-154">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md) <br/> |<span data-ttu-id="92094-155">Indique si un objet blob règle de Microsoft Outlook existe dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="92094-155">Indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="92094-156">InboxRules</span><span class="sxs-lookup"><span data-stu-id="92094-156">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="92094-157">Représente un tableau des règles de boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="92094-157">Represents an array of the rules in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92094-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="92094-158">Parent elements</span></span>

<span data-ttu-id="92094-159">Aucun.</span><span class="sxs-lookup"><span data-stu-id="92094-159">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="92094-160">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="92094-160">Text value</span></span>

<span data-ttu-id="92094-161">Aucun.</span><span class="sxs-lookup"><span data-stu-id="92094-161">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="92094-162">Remarques</span><span class="sxs-lookup"><span data-stu-id="92094-162">Remarks</span></span>

<span data-ttu-id="92094-163">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="92094-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92094-164">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="92094-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92094-165">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="92094-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="92094-166">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="92094-166">Schema name</span></span>  <br/> |<span data-ttu-id="92094-167">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="92094-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="92094-168">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="92094-168">Validation file</span></span>  <br/> |<span data-ttu-id="92094-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="92094-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="92094-170">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="92094-170">Can be empty</span></span>  <br/> |<span data-ttu-id="92094-171">False</span><span class="sxs-lookup"><span data-stu-id="92094-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92094-172">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="92094-172">See also</span></span>

- [<span data-ttu-id="92094-173">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="92094-173">GetInboxRules</span></span>](getinboxrules.md)
- [<span data-ttu-id="92094-174">Opération de GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="92094-174">GetInboxRules operation</span></span>](getinboxrules-operation.md)

