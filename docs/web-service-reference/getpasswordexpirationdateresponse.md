---
title: GetPasswordExpirationDateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: L’élément GetPasswordExpirationDateResponse définit la réponse à une demande d’opération d’opération GetPasswordExpirationDate.
ms.openlocfilehash: c925b2b37879ba0f8f25b2dd73737ed2f3202555
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530203"
---
# <a name="getpasswordexpirationdateresponse"></a><span data-ttu-id="93230-103">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="93230-103">GetPasswordExpirationDateResponse</span></span>

<span data-ttu-id="93230-104">L’élément **GetPasswordExpirationDateResponse** définit la réponse à une demande d’opération d' [opération GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="93230-104">The **GetPasswordExpirationDateResponse** element defines the response to a [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation request.</span></span> 
  
- [<span data-ttu-id="93230-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="93230-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="93230-106">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="93230-106">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 <span data-ttu-id="93230-107">**GetPasswordExpirationDateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="93230-107">**GetPasswordExpirationDateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93230-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="93230-108">Attributes and elements</span></span>

<span data-ttu-id="93230-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="93230-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93230-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="93230-110">Attributes</span></span>

|<span data-ttu-id="93230-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="93230-111">**Attribute**</span></span>|<span data-ttu-id="93230-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="93230-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93230-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="93230-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="93230-114">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="93230-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="93230-115">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="93230-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="93230-116">-Réussite</span><span class="sxs-lookup"><span data-stu-id="93230-116">-  Success</span></span>  <br/><span data-ttu-id="93230-117">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="93230-117">-  Warning</span></span>  <br/><span data-ttu-id="93230-118">-Erreur</span><span class="sxs-lookup"><span data-stu-id="93230-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="93230-119">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="93230-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="93230-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="93230-120">**Value**</span></span>|<span data-ttu-id="93230-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="93230-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93230-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="93230-122">**Success**</span></span> <br/> |<span data-ttu-id="93230-123">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="93230-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="93230-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="93230-124">**Warning**</span></span> <br/> | <span data-ttu-id="93230-125">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="93230-125">Describes a request that was not processed.</span></span> <span data-ttu-id="93230-126">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="93230-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="93230-127">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="93230-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="93230-128">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="93230-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="93230-129">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="93230-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="93230-130">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="93230-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="93230-131">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="93230-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="93230-132">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="93230-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="93230-133">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="93230-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="93230-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="93230-134">**Error**</span></span> <br/> | <span data-ttu-id="93230-135">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="93230-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="93230-136">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="93230-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="93230-137">-Attributs ou éléments non valides.</span><span class="sxs-lookup"><span data-stu-id="93230-137">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="93230-138">-Les attributs ou les éléments qui sont en dehors de la plage.</span><span class="sxs-lookup"><span data-stu-id="93230-138">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="93230-139">-Balise inconnue.</span><span class="sxs-lookup"><span data-stu-id="93230-139">-  An unknown tag.</span></span>  <br/><span data-ttu-id="93230-140">-Un attribut ou un élément qui n’est pas valide dans le contexte.</span><span class="sxs-lookup"><span data-stu-id="93230-140">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="93230-141">-Une tentative d’accès non autorisée par un client.</span><span class="sxs-lookup"><span data-stu-id="93230-141">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="93230-142">-Un échec côté serveur en réponse à un appel côté client valide.</span><span class="sxs-lookup"><span data-stu-id="93230-142">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="93230-143">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="93230-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="93230-144">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="93230-144">Child elements</span></span>

|<span data-ttu-id="93230-145">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="93230-145">**Element name**</span></span>|<span data-ttu-id="93230-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="93230-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93230-147">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="93230-147">PasswordExpirationDate</span></span>](passwordexpirationdate.md) <br/> |<span data-ttu-id="93230-148">Indique la date d’expiration du mot de passe pour le compte de messagerie spécifié dans la demande.</span><span class="sxs-lookup"><span data-stu-id="93230-148">Provides the password expiration date for the email account specified in the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93230-149">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="93230-149">Parent elements</span></span>

|<span data-ttu-id="93230-150">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="93230-150">**Element name**</span></span>|<span data-ttu-id="93230-151">**Description**</span><span class="sxs-lookup"><span data-stu-id="93230-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93230-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="93230-152">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="93230-153">Contient les messages de réponse pour une demande de services Web Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="93230-153">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="93230-154">Remarques</span><span class="sxs-lookup"><span data-stu-id="93230-154">Remarks</span></span>

<span data-ttu-id="93230-155">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="93230-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="93230-156">Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="93230-156">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93230-157">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="93230-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93230-158">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="93230-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93230-159">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="93230-159">Schema Name</span></span>  <br/> |<span data-ttu-id="93230-160">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="93230-160">Messages schema</span></span>  <br/> |
|<span data-ttu-id="93230-161">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="93230-161">Validation File</span></span>  <br/> |<span data-ttu-id="93230-162">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="93230-162">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93230-163">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="93230-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="93230-164">False</span><span class="sxs-lookup"><span data-stu-id="93230-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93230-165">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="93230-165">See also</span></span>

- [<span data-ttu-id="93230-166">Opération GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="93230-166">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="93230-167">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="93230-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

