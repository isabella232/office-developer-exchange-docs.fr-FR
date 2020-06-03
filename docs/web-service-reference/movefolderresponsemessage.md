---
title: MoveFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolderResponseMessage
api_type:
- schema
ms.assetid: 54917251-96af-44c2-ae90-d545f0a16e2e
description: L’élément MoveFolderResponseMessage contient l’État et le résultat d’une seule demande d’opération MoveFolder.
ms.openlocfilehash: 634fec89445b49d1c8c42541f2fc50d07b5a1acd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467472"
---
# <a name="movefolderresponsemessage"></a><span data-ttu-id="24dde-103">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="24dde-103">MoveFolderResponseMessage</span></span>

<span data-ttu-id="24dde-104">L’élément **MoveFolderResponseMessage** contient l’État et le résultat d’une seule demande d' [opération MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="24dde-104">The **MoveFolderResponseMessage** element contains the status and result of a single [MoveFolder operation](movefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="24dde-105">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="24dde-105">MoveFolderResponse</span></span>](movefolderresponse.md)
- [<span data-ttu-id="24dde-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="24dde-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="24dde-107">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="24dde-107">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
  
```xml
<MoveFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</MoveFolderResponseMessage>
```

 <span data-ttu-id="24dde-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="24dde-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24dde-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="24dde-109">Attributes and elements</span></span>

<span data-ttu-id="24dde-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="24dde-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24dde-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="24dde-111">Attributes</span></span>

|<span data-ttu-id="24dde-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="24dde-112">**Attribute**</span></span>|<span data-ttu-id="24dde-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="24dde-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="24dde-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="24dde-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="24dde-115">Décrit l’état d’une réponse d' [opération MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="24dde-115">Describes the status of a [MoveFolder operation](movefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="24dde-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="24dde-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="24dde-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="24dde-117">-  Success</span></span>  <br/><span data-ttu-id="24dde-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="24dde-118">-  Warning</span></span>  <br/><span data-ttu-id="24dde-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="24dde-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="24dde-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="24dde-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="24dde-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="24dde-121">**Value**</span></span>|<span data-ttu-id="24dde-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="24dde-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="24dde-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="24dde-123">**Success**</span></span> <br/> |<span data-ttu-id="24dde-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="24dde-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="24dde-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="24dde-125">**Warning**</span></span> <br/> | <span data-ttu-id="24dde-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="24dde-126">Describes a request that was not processed.</span></span> <span data-ttu-id="24dde-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="24dde-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="24dde-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="24dde-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="24dde-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="24dde-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="24dde-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="24dde-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="24dde-131">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="24dde-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="24dde-132">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="24dde-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="24dde-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="24dde-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="24dde-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="24dde-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="24dde-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="24dde-135">**Error**</span></span> <br/> | <span data-ttu-id="24dde-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="24dde-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="24dde-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="24dde-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="24dde-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="24dde-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="24dde-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="24dde-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="24dde-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="24dde-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="24dde-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="24dde-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="24dde-142">-Toute tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="24dde-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="24dde-143">-Tout échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="24dde-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="24dde-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="24dde-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="24dde-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="24dde-145">Child elements</span></span>

|<span data-ttu-id="24dde-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="24dde-146">**Element**</span></span>|<span data-ttu-id="24dde-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="24dde-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24dde-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="24dde-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="24dde-149">Texte décrivant l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="24dde-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="24dde-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="24dde-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="24dde-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="24dde-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="24dde-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="24dde-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="24dde-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="24dde-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="24dde-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="24dde-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="24dde-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="24dde-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="24dde-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="24dde-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="24dde-157">Dossiers</span><span class="sxs-lookup"><span data-stu-id="24dde-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="24dde-158">Contient un tableau de dossiers déplacés.</span><span class="sxs-lookup"><span data-stu-id="24dde-158">Contains an array of moved folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24dde-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="24dde-159">Parent elements</span></span>

|<span data-ttu-id="24dde-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="24dde-160">**Element**</span></span>|<span data-ttu-id="24dde-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="24dde-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24dde-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="24dde-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="24dde-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="24dde-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="24dde-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="24dde-164">Remarks</span></span>

<span data-ttu-id="24dde-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="24dde-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24dde-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="24dde-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24dde-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="24dde-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="24dde-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="24dde-168">Schema Name</span></span>  <br/> |<span data-ttu-id="24dde-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="24dde-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="24dde-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="24dde-170">Validation File</span></span>  <br/> |<span data-ttu-id="24dde-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="24dde-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="24dde-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="24dde-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="24dde-173">False</span><span class="sxs-lookup"><span data-stu-id="24dde-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24dde-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="24dde-174">See also</span></span>

- [<span data-ttu-id="24dde-175">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="24dde-175">MoveFolder</span></span>](movefolder.md)
- [<span data-ttu-id="24dde-176">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="24dde-176">MoveFolder operation</span></span>](movefolder-operation.md)

