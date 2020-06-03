---
title: FindFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolderResponseMessage
api_type:
- schema
ms.assetid: 538d64fe-51ae-41d2-bfab-91698678aa1b
description: L’élément FindFolderResponseMessage contient l’État et le résultat d’une seule demande d’opération FindFolder.
ms.openlocfilehash: 318a09e371043252d43a5197211e9623f34229fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462562"
---
# <a name="findfolderresponsemessage"></a><span data-ttu-id="542f7-103">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="542f7-103">FindFolderResponseMessage</span></span>

<span data-ttu-id="542f7-104">L’élément **FindFolderResponseMessage** contient l’État et le résultat d’une seule demande d' [opération FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="542f7-104">The **FindFolderResponseMessage** element contains the status and result of a single [FindFolder operation](findfolder-operation.md) request.</span></span> 
  
[<span data-ttu-id="542f7-105">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="542f7-105">FindFolderResponse</span></span>](findfolderresponse.md)
  
[<span data-ttu-id="542f7-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="542f7-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="542f7-107">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="542f7-107">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
  
```xml
<FindFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindFolderResponseMessage>
```

 <span data-ttu-id="542f7-108">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="542f7-108">**FindFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="542f7-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="542f7-109">Attributes and elements</span></span>

<span data-ttu-id="542f7-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="542f7-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="542f7-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="542f7-111">Attributes</span></span>

|<span data-ttu-id="542f7-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="542f7-112">**Attribute**</span></span>|<span data-ttu-id="542f7-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="542f7-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="542f7-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="542f7-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="542f7-115">Décrit l’état d’une réponse d' [opération FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="542f7-115">Describes the status of a [FindFolder operation](findfolder-operation.md) response.</span></span><br/><br/> <span data-ttu-id="542f7-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="542f7-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="542f7-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="542f7-117">-  Success</span></span>  <br/><span data-ttu-id="542f7-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="542f7-118">-  Warning</span></span>  <br/><span data-ttu-id="542f7-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="542f7-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="542f7-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="542f7-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="542f7-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="542f7-121">**Value**</span></span>|<span data-ttu-id="542f7-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="542f7-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="542f7-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="542f7-123">**Success**</span></span> <br/> |<span data-ttu-id="542f7-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="542f7-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="542f7-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="542f7-125">**Warning**</span></span> <br/> | <span data-ttu-id="542f7-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="542f7-126">Describes a request that was not processed.</span></span> <span data-ttu-id="542f7-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="542f7-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="542f7-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="542f7-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="542f7-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="542f7-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="542f7-130">-Les services de domaine Active Directory (AD DS) sont en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="542f7-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="542f7-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="542f7-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="542f7-132">-La base de données de messages (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="542f7-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="542f7-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="542f7-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="542f7-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="542f7-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="542f7-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="542f7-135">**Error**</span></span> <br/> | <span data-ttu-id="542f7-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="542f7-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="542f7-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="542f7-137">The following are examples of sources of errors:</span></span>  <br/><span data-ttu-id="542f7-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="542f7-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="542f7-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="542f7-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="542f7-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="542f7-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="542f7-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="542f7-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="542f7-142">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="542f7-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="542f7-143">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="542f7-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="542f7-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="542f7-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="542f7-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="542f7-145">Child elements</span></span>

|<span data-ttu-id="542f7-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="542f7-146">**Element**</span></span>|<span data-ttu-id="542f7-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="542f7-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="542f7-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="542f7-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="542f7-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="542f7-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="542f7-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="542f7-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="542f7-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="542f7-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="542f7-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="542f7-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="542f7-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="542f7-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="542f7-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="542f7-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="542f7-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="542f7-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="542f7-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="542f7-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="542f7-157">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="542f7-157">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="542f7-158">Contient les résultats d’une recherche d’un dossier racine unique pendant une [opération FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="542f7-158">Contains the results from a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="542f7-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="542f7-159">Parent elements</span></span>

|<span data-ttu-id="542f7-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="542f7-160">**Element**</span></span>|<span data-ttu-id="542f7-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="542f7-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="542f7-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="542f7-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="542f7-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="542f7-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="542f7-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="542f7-164">Remarks</span></span>

<span data-ttu-id="542f7-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="542f7-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="542f7-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="542f7-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="542f7-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="542f7-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="542f7-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="542f7-168">Schema name</span></span>  <br/> |<span data-ttu-id="542f7-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="542f7-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="542f7-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="542f7-170">Validation file</span></span>  <br/> |<span data-ttu-id="542f7-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="542f7-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="542f7-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="542f7-172">Can be empty</span></span>  <br/> |<span data-ttu-id="542f7-173">False</span><span class="sxs-lookup"><span data-stu-id="542f7-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="542f7-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="542f7-174">See also</span></span>

- [<span data-ttu-id="542f7-175">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="542f7-175">FindFolder operation</span></span>](findfolder-operation.md)
- [<span data-ttu-id="542f7-176">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="542f7-176">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

