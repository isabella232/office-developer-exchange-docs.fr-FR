---
title: GetRoomsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomsResponse
api_type:
- schema
ms.assetid: a8c85f65-bb63-4e7a-b0ca-7c9a04560a58
description: L’élément GetRoomsResponse définit une réponse à une demande d’opération GetRooms.
ms.openlocfilehash: 661e143a9edd30f12ab83fb0666e2832422e280a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458585"
---
# <a name="getroomsresponse"></a><span data-ttu-id="4cd14-103">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="4cd14-103">GetRoomsResponse</span></span>

<span data-ttu-id="4cd14-104">L’élément **GetRoomsResponse** définit une réponse à une demande d' [opération GetRooms](getrooms-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4cd14-104">The **GetRoomsResponse** element defines a response to a [GetRooms operation](getrooms-operation.md) request.</span></span> 
  
- [<span data-ttu-id="4cd14-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4cd14-105">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="4cd14-106">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="4cd14-106">GetRoomsResponse</span></span>](getroomsresponse.md)
  
```XML
<GetRoomsResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Rooms/>
</GetRoomsResponse>
```

 <span data-ttu-id="4cd14-107">**GetRoomsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4cd14-107">**GetRoomsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4cd14-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4cd14-108">Attributes and elements</span></span>

<span data-ttu-id="4cd14-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4cd14-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4cd14-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="4cd14-110">Attributes</span></span>

|<span data-ttu-id="4cd14-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4cd14-111">**Attribute**</span></span>|<span data-ttu-id="4cd14-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4cd14-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4cd14-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="4cd14-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4cd14-114">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="4cd14-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="4cd14-115">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="4cd14-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="4cd14-116">-Réussite</span><span class="sxs-lookup"><span data-stu-id="4cd14-116">-  Success</span></span>  <br/><span data-ttu-id="4cd14-117">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="4cd14-117">-  Warning</span></span>  <br/><span data-ttu-id="4cd14-118">-Erreur</span><span class="sxs-lookup"><span data-stu-id="4cd14-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4cd14-119">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="4cd14-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="4cd14-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4cd14-120">**Value**</span></span>|<span data-ttu-id="4cd14-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="4cd14-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4cd14-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="4cd14-122">**Success**</span></span> <br/> |<span data-ttu-id="4cd14-123">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="4cd14-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4cd14-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="4cd14-124">**Warning**</span></span> <br/> | <span data-ttu-id="4cd14-125">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="4cd14-125">Describes a request that was not processed.</span></span> <span data-ttu-id="4cd14-126">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="4cd14-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="4cd14-127">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="4cd14-127">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="4cd14-128">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="4cd14-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="4cd14-129">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="4cd14-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="4cd14-130">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="4cd14-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="4cd14-131">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="4cd14-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="4cd14-132">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="4cd14-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="4cd14-133">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="4cd14-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="4cd14-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="4cd14-134">**Error**</span></span> <br/> | <span data-ttu-id="4cd14-135">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="4cd14-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4cd14-136">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="4cd14-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="4cd14-137">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="4cd14-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4cd14-138">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="4cd14-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="4cd14-139">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="4cd14-139">-  An unknown tag</span></span>  <br/><span data-ttu-id="4cd14-140">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="4cd14-140">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="4cd14-141">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="4cd14-141">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4cd14-142">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="4cd14-142">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="4cd14-143">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="4cd14-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4cd14-144">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4cd14-144">Child elements</span></span>

|<span data-ttu-id="4cd14-145">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4cd14-145">**Element**</span></span>|<span data-ttu-id="4cd14-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="4cd14-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cd14-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="4cd14-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4cd14-148">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="4cd14-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4cd14-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4cd14-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4cd14-150">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="4cd14-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4cd14-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4cd14-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4cd14-152">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="4cd14-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="4cd14-153">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="4cd14-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4cd14-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4cd14-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4cd14-155">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="4cd14-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4cd14-156">Salons</span><span class="sxs-lookup"><span data-stu-id="4cd14-156">Rooms</span></span>](rooms.md) <br/> |<span data-ttu-id="4cd14-157">Fournit la liste des adresses de messagerie et des noms d’affichage qui représentent les salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="4cd14-157">Provides a list of email addresses and display names that represent meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4cd14-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4cd14-158">Parent elements</span></span>

|<span data-ttu-id="4cd14-159">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4cd14-159">**Element**</span></span>|<span data-ttu-id="4cd14-160">**Description**</span><span class="sxs-lookup"><span data-stu-id="4cd14-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cd14-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4cd14-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4cd14-162">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4cd14-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4cd14-163">Remarques</span><span class="sxs-lookup"><span data-stu-id="4cd14-163">Remarks</span></span>

<span data-ttu-id="4cd14-164">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4cd14-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4cd14-165">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4cd14-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4cd14-166">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4cd14-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4cd14-167">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4cd14-167">Schema Name</span></span>  <br/> |<span data-ttu-id="4cd14-168">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4cd14-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4cd14-169">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4cd14-169">Validation File</span></span>  <br/> |<span data-ttu-id="4cd14-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4cd14-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4cd14-171">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4cd14-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="4cd14-172">False</span><span class="sxs-lookup"><span data-stu-id="4cd14-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4cd14-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4cd14-173">See also</span></span>

- [<span data-ttu-id="4cd14-174">Opération GetRooms</span><span class="sxs-lookup"><span data-stu-id="4cd14-174">GetRooms operation</span></span>](getrooms-operation.md)
- [<span data-ttu-id="4cd14-175">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4cd14-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

