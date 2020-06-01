---
title: MailTipsResponseMessageType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsResponseMessageType
api_type:
- schema
ms.assetid: 532cb9d9-1232-4e88-80aa-4cf163eb05da
description: L’élément MailTipsResponseMessageType représente les paramètres des conseils de messagerie.
ms.openlocfilehash: 5244f26ef927a817a9087c299fd1124acb828aa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454035"
---
# <a name="mailtipsresponsemessagetype"></a><span data-ttu-id="20116-103">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="20116-103">MailTipsResponseMessageType</span></span>

<span data-ttu-id="20116-104">L’élément **MailTipsResponseMessageType** représente les paramètres des conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="20116-104">The **MailTipsResponseMessageType** element represents mail tips settings.</span></span> 
  
```XML
<MailTipsResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTips/>
</MailTipsResponseMessageType>
```

 <span data-ttu-id="20116-105">**MailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="20116-105">**MailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20116-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="20116-106">Attributes and elements</span></span>

<span data-ttu-id="20116-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="20116-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20116-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="20116-108">Attributes</span></span>

|<span data-ttu-id="20116-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="20116-109">**Attribute**</span></span>|<span data-ttu-id="20116-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="20116-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="20116-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="20116-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="20116-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="20116-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="20116-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="20116-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="20116-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="20116-114">-  Success</span></span>  <br/><span data-ttu-id="20116-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="20116-115">-  Warning</span></span>  <br/><span data-ttu-id="20116-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="20116-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="20116-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="20116-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="20116-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="20116-118">**Value**</span></span>|<span data-ttu-id="20116-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="20116-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="20116-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="20116-120">**Success**</span></span> <br/> |<span data-ttu-id="20116-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="20116-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="20116-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="20116-122">**Warning**</span></span> <br/> | <span data-ttu-id="20116-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="20116-123">Describes a request that was not processed.</span></span> <span data-ttu-id="20116-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="20116-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="20116-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="20116-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="20116-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="20116-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="20116-127">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="20116-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="20116-128">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="20116-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="20116-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="20116-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="20116-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="20116-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="20116-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="20116-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="20116-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="20116-132">**Error**</span></span> <br/> | <span data-ttu-id="20116-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="20116-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="20116-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="20116-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="20116-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="20116-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="20116-136">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="20116-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="20116-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="20116-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="20116-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="20116-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="20116-139">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="20116-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="20116-140">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="20116-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="20116-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="20116-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="20116-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="20116-142">Child elements</span></span>

|<span data-ttu-id="20116-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20116-143">**Element**</span></span>|<span data-ttu-id="20116-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="20116-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20116-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="20116-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="20116-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="20116-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="20116-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="20116-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="20116-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="20116-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="20116-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="20116-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="20116-150">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="20116-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="20116-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="20116-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="20116-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="20116-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="20116-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="20116-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="20116-154">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="20116-154">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="20116-155">Représente les valeurs de différents types de conseils de courrier.</span><span class="sxs-lookup"><span data-stu-id="20116-155">Represents values for various types of mail tips.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="20116-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="20116-156">Parent elements</span></span>

|<span data-ttu-id="20116-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20116-157">**Element**</span></span>|<span data-ttu-id="20116-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="20116-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20116-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="20116-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="20116-160">Représente une liste de messages de réponse à des conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="20116-160">Represents a list of mail tips response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20116-161">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="20116-161">Text value</span></span>

<span data-ttu-id="20116-162">Aucun.</span><span class="sxs-lookup"><span data-stu-id="20116-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="20116-163">Remarques</span><span class="sxs-lookup"><span data-stu-id="20116-163">Remarks</span></span>

<span data-ttu-id="20116-164">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="20116-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20116-165">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="20116-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20116-166">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="20116-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="20116-167">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="20116-167">Schema Name</span></span>  <br/> |<span data-ttu-id="20116-168">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="20116-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="20116-169">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="20116-169">Validation File</span></span>  <br/> |<span data-ttu-id="20116-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="20116-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="20116-171">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="20116-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="20116-172">False</span><span class="sxs-lookup"><span data-stu-id="20116-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20116-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="20116-173">See also</span></span>

- [<span data-ttu-id="20116-174">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="20116-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

