---
title: GetPasswordExpirationDateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: L’élément GetPasswordExpirationDateResponse définit la réponse à une demande d’opération GetPasswordExpirationDate opération.
ms.openlocfilehash: 3754a53da53c12479f11c2e32cd15a08cba665fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756714"
---
# <a name="getpasswordexpirationdateresponse"></a><span data-ttu-id="b0306-103">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="b0306-103">GetPasswordExpirationDateResponse</span></span>

<span data-ttu-id="b0306-104">L’élément **GetPasswordExpirationDateResponse** définit la réponse à une demande d’opération [GetPasswordExpirationDate opération](getpasswordexpirationdate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b0306-104">The **GetPasswordExpirationDateResponse** element defines the response to a [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation request.</span></span> 
  
- [<span data-ttu-id="b0306-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b0306-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="b0306-106">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="b0306-106">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 <span data-ttu-id="b0306-107">**GetPasswordExpirationDateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b0306-107">**GetPasswordExpirationDateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0306-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b0306-108">Attributes and elements</span></span>

<span data-ttu-id="b0306-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b0306-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0306-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="b0306-110">Attributes</span></span>

|<span data-ttu-id="b0306-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b0306-111">**Attribute**</span></span>|<span data-ttu-id="b0306-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0306-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b0306-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b0306-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b0306-114">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="b0306-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="b0306-115">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="b0306-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="b0306-116">-Réussite</span><span class="sxs-lookup"><span data-stu-id="b0306-116">-  Success</span></span>  <br/><span data-ttu-id="b0306-117">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="b0306-117">-  Warning</span></span>  <br/><span data-ttu-id="b0306-118">-Erreur</span><span class="sxs-lookup"><span data-stu-id="b0306-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b0306-119">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b0306-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="b0306-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="b0306-120">**Value**</span></span>|<span data-ttu-id="b0306-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0306-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b0306-122">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="b0306-122">**Success**</span></span> <br/> |<span data-ttu-id="b0306-123">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="b0306-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b0306-124">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="b0306-124">**Warning**</span></span> <br/> | <span data-ttu-id="b0306-125">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="b0306-125">Describes a request that was not processed.</span></span> <span data-ttu-id="b0306-126">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="b0306-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="b0306-127">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="b0306-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="b0306-128">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="b0306-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="b0306-129">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b0306-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="b0306-130">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="b0306-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="b0306-131">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b0306-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="b0306-132">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="b0306-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="b0306-133">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="b0306-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="b0306-134">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="b0306-134">**Error**</span></span> <br/> | <span data-ttu-id="b0306-135">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="b0306-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b0306-136">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="b0306-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b0306-137">-Non valide attributs ou éléments.</span><span class="sxs-lookup"><span data-stu-id="b0306-137">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="b0306-138">-Les attributs ou les éléments qui sont hors de portée.</span><span class="sxs-lookup"><span data-stu-id="b0306-138">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="b0306-139">-Une balise inconnue.</span><span class="sxs-lookup"><span data-stu-id="b0306-139">-  An unknown tag.</span></span>  <br/><span data-ttu-id="b0306-140">-Un attribut ou un élément qui n’est pas valide dans le contexte.</span><span class="sxs-lookup"><span data-stu-id="b0306-140">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="b0306-141">-Une tentative d’accès non autorisé par n’importe quel client.</span><span class="sxs-lookup"><span data-stu-id="b0306-141">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="b0306-142">-Une panne côté serveur en réponse à un appel côté client valid.</span><span class="sxs-lookup"><span data-stu-id="b0306-142">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="b0306-143">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b0306-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b0306-144">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b0306-144">Child elements</span></span>

|<span data-ttu-id="b0306-145">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="b0306-145">**Element name**</span></span>|<span data-ttu-id="b0306-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0306-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0306-147">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="b0306-147">PasswordExpirationDate</span></span>](passwordexpirationdate.md) <br/> |<span data-ttu-id="b0306-148">Fournit la date d’expiration de mot de passe du compte de messagerie spécifiée dans la demande.</span><span class="sxs-lookup"><span data-stu-id="b0306-148">Provides the password expiration date for the email account specified in the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0306-149">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b0306-149">Parent elements</span></span>

|<span data-ttu-id="b0306-150">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="b0306-150">**Element name**</span></span>|<span data-ttu-id="b0306-151">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0306-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0306-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b0306-152">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b0306-153">Contient les messages de réponse pour une demande d’Exchange Web Services (EWS).</span><span class="sxs-lookup"><span data-stu-id="b0306-153">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b0306-154">Remarques</span><span class="sxs-lookup"><span data-stu-id="b0306-154">Remarks</span></span>

<span data-ttu-id="b0306-155">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0306-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="b0306-156">Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="b0306-156">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0306-157">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b0306-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0306-158">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b0306-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b0306-159">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b0306-159">Schema Name</span></span>  <br/> |<span data-ttu-id="b0306-160">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b0306-160">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b0306-161">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b0306-161">Validation File</span></span>  <br/> |<span data-ttu-id="b0306-162">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b0306-162">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b0306-163">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b0306-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0306-164">False</span><span class="sxs-lookup"><span data-stu-id="b0306-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0306-165">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b0306-165">See also</span></span>

- [<span data-ttu-id="b0306-166">Opération GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="b0306-166">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="b0306-167">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b0306-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

