---
title: GetMessageTrackingReportResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReportResponse
api_type:
- schema
ms.assetid: 41177894-2008-44a6-86f8-bc34c0a48e36
description: L’élément GetMessageTrackingReportResponse contient la réponse pour l’opération GetMessageTrackingReport.
ms.openlocfilehash: 15e1f5c91c07dbaad224fb0cd3bc89f444a18087
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460567"
---
# <a name="getmessagetrackingreportresponse"></a><span data-ttu-id="8dfa1-103">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="8dfa1-103">GetMessageTrackingReportResponse</span></span>

<span data-ttu-id="8dfa1-104">L’élément **GetMessageTrackingReportResponse** contient la réponse pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="8dfa1-104">The **GetMessageTrackingReportResponse** element contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
```xml
<GetMessageTrackingReportResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MessageTrackingReport/>
   <Diagnostics/>
   <Errors/>
   <Properties/>
</GetMessageTrackingReportResponse>
```

 <span data-ttu-id="8dfa1-105">**GetMessageTrackingReportResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8dfa1-105">**GetMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8dfa1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8dfa1-106">Attributes and elements</span></span>

<span data-ttu-id="8dfa1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8dfa1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8dfa1-108">Attributes</span></span>

|<span data-ttu-id="8dfa1-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="8dfa1-109">**Attribute**</span></span>|<span data-ttu-id="8dfa1-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="8dfa1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8dfa1-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="8dfa1-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="8dfa1-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="8dfa1-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="8dfa1-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="8dfa1-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="8dfa1-114">-  Success</span></span>  <br/><span data-ttu-id="8dfa1-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="8dfa1-115">-  Warning</span></span>  <br/><span data-ttu-id="8dfa1-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="8dfa1-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="8dfa1-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="8dfa1-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="8dfa1-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="8dfa1-118">**Value**</span></span>|<span data-ttu-id="8dfa1-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="8dfa1-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8dfa1-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="8dfa1-120">**Success**</span></span> <br/> |<span data-ttu-id="8dfa1-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="8dfa1-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="8dfa1-122">**Warning**</span></span> <br/> | <span data-ttu-id="8dfa1-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-123">Describes a request that was not processed.</span></span> <span data-ttu-id="8dfa1-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="8dfa1-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="8dfa1-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="8dfa1-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="8dfa1-127">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-127">-  Active Directory Domain Serves (AD DS) is offline.</span></span>  <br/><span data-ttu-id="8dfa1-128">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="8dfa1-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="8dfa1-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="8dfa1-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="8dfa1-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="8dfa1-132">**Error**</span></span> <br/> | <span data-ttu-id="8dfa1-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="8dfa1-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="8dfa1-134">The following are examples of sources of errors:</span></span>  <br/>  <span data-ttu-id="8dfa1-135">Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="8dfa1-135">Invalid attributes or elements</span></span>  <br/><br/><span data-ttu-id="8dfa1-136">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="8dfa1-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="8dfa1-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="8dfa1-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="8dfa1-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="8dfa1-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="8dfa1-139">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="8dfa1-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="8dfa1-140">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="8dfa1-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="8dfa1-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="8dfa1-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8dfa1-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8dfa1-142">Child elements</span></span>

|<span data-ttu-id="8dfa1-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8dfa1-143">**Element**</span></span>|<span data-ttu-id="8dfa1-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="8dfa1-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8dfa1-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="8dfa1-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="8dfa1-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="8dfa1-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8dfa1-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="8dfa1-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="8dfa1-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8dfa1-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="8dfa1-150">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="8dfa1-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="8dfa1-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="8dfa1-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="8dfa1-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="8dfa1-154">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="8dfa1-154">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="8dfa1-155">Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="8dfa1-155">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="8dfa1-156">Diagnostics</span><span class="sxs-lookup"><span data-stu-id="8dfa1-156">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="8dfa1-157">Fournit des informations sur le temps et les performances utilisées pour la création de rapports dans un centre de données.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-157">Provides timing and performance information that is used for reporting in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="8dfa1-158">Erreurs</span><span class="sxs-lookup"><span data-stu-id="8dfa1-158">Errors</span></span>](errors-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8dfa1-159">Contient un conteneur de propriétés permettant de stocker les erreurs renvoyées via le service Web.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-159">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="8dfa1-160">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="8dfa1-160">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="8dfa1-161">Contient une liste d’une ou plusieurs propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-161">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8dfa1-162">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8dfa1-162">Parent elements</span></span>

<span data-ttu-id="8dfa1-163">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-163">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="8dfa1-164">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8dfa1-164">Text value</span></span>

<span data-ttu-id="8dfa1-165">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8dfa1-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="8dfa1-166">Remarks</span></span>

<span data-ttu-id="8dfa1-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8dfa1-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8dfa1-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8dfa1-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8dfa1-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8dfa1-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8dfa1-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8dfa1-170">Schema Name</span></span>  <br/> |<span data-ttu-id="8dfa1-171">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="8dfa1-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8dfa1-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8dfa1-172">Validation File</span></span>  <br/> |<span data-ttu-id="8dfa1-173">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8dfa1-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8dfa1-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8dfa1-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="8dfa1-175">False</span><span class="sxs-lookup"><span data-stu-id="8dfa1-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8dfa1-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8dfa1-176">See also</span></span>

- [<span data-ttu-id="8dfa1-177">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="8dfa1-177">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="8dfa1-178">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8dfa1-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

