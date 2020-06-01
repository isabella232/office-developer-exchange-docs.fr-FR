---
title: GetPhoneCallInformationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetPhoneCallInformationResponse
api_type:
- schema
ms.assetid: 17f79875-46ec-4289-b974-b3c35af429cd
description: L’élément GetPhoneCallInformationResponse définit une réponse à une requête GetPhoneCallInformation unique.
ms.openlocfilehash: 5bc060504ea734ec2d7e01707ef6bbdb0aa665d3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457885"
---
# <a name="getphonecallinformationresponse"></a><span data-ttu-id="bfcd9-103">GetPhoneCallInformationResponse</span><span class="sxs-lookup"><span data-stu-id="bfcd9-103">GetPhoneCallInformationResponse</span></span>

<span data-ttu-id="bfcd9-104">L’élément **GetPhoneCallInformationResponse** définit une réponse à une requête GetPhoneCallInformation unique.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-104">The **GetPhoneCallInformationResponse** element defines a response to a single GetPhoneCallInformation request.</span></span> 
  
```xml
<GetPhoneCallInformationResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <PhoneCallInformation/>
</GetPhoneCallInformationResponse>
```

 <span data-ttu-id="bfcd9-105">**GetPhoneCallInformationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="bfcd9-105">**GetPhoneCallInformationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bfcd9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bfcd9-106">Attributes and elements</span></span>

<span data-ttu-id="bfcd9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bfcd9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bfcd9-108">Attributes</span></span>

|<span data-ttu-id="bfcd9-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bfcd9-109">**Attribute**</span></span>|<span data-ttu-id="bfcd9-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="bfcd9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bfcd9-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="bfcd9-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="bfcd9-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="bfcd9-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="bfcd9-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="bfcd9-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="bfcd9-114">-  Success</span></span>  <br/><span data-ttu-id="bfcd9-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="bfcd9-115">-  Warning</span></span>  <br/><span data-ttu-id="bfcd9-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="bfcd9-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="bfcd9-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="bfcd9-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="bfcd9-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="bfcd9-118">**Value**</span></span>|<span data-ttu-id="bfcd9-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="bfcd9-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bfcd9-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="bfcd9-120">**Success**</span></span> <br/> |<span data-ttu-id="bfcd9-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="bfcd9-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="bfcd9-122">**Warning**</span></span> <br/> | <span data-ttu-id="bfcd9-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-123">Describes a request that was not processed.</span></span> <span data-ttu-id="bfcd9-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="bfcd9-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="bfcd9-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="bfcd9-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="bfcd9-127">-Le service d’annuaire Active Directory est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="bfcd9-128">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="bfcd9-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="bfcd9-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="bfcd9-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="bfcd9-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="bfcd9-132">**Error**</span></span> <br/> | <span data-ttu-id="bfcd9-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="bfcd9-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="bfcd9-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="bfcd9-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="bfcd9-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="bfcd9-136">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="bfcd9-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="bfcd9-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="bfcd9-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="bfcd9-138">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="bfcd9-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="bfcd9-139">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="bfcd9-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="bfcd9-140">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="bfcd9-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="bfcd9-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="bfcd9-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bfcd9-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bfcd9-142">Child elements</span></span>

|<span data-ttu-id="bfcd9-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bfcd9-143">**Element**</span></span>|<span data-ttu-id="bfcd9-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="bfcd9-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfcd9-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="bfcd9-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bfcd9-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bfcd9-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bfcd9-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bfcd9-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bfcd9-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bfcd9-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bfcd9-150">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="bfcd9-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bfcd9-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="bfcd9-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bfcd9-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="bfcd9-154">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="bfcd9-154">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="bfcd9-155">Spécifie les informations d’État pour un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-155">Specifies the state information for a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bfcd9-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bfcd9-156">Parent elements</span></span>

<span data-ttu-id="bfcd9-157">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bfcd9-158">Remarques</span><span class="sxs-lookup"><span data-stu-id="bfcd9-158">Remarks</span></span>

<span data-ttu-id="bfcd9-159">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="bfcd9-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bfcd9-160">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bfcd9-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bfcd9-161">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bfcd9-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bfcd9-162">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bfcd9-162">Schema Name</span></span>  <br/> |<span data-ttu-id="bfcd9-163">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="bfcd9-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bfcd9-164">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bfcd9-164">Validation File</span></span>  <br/> |<span data-ttu-id="bfcd9-165">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bfcd9-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bfcd9-166">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bfcd9-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="bfcd9-167">False</span><span class="sxs-lookup"><span data-stu-id="bfcd9-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bfcd9-168">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bfcd9-168">See also</span></span>

- [<span data-ttu-id="bfcd9-169">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bfcd9-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

