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
description: L’élément GetMessageTrackingReportResponse contient la réponse de l’opération GetMessageTrackingReport.
ms.openlocfilehash: bdb8b97e57f92a32cbdc498d09297920366b58bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756678"
---
# <a name="getmessagetrackingreportresponse"></a><span data-ttu-id="1cb3e-103">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="1cb3e-103">GetMessageTrackingReportResponse</span></span>

<span data-ttu-id="1cb3e-104">L’élément **GetMessageTrackingReportResponse** contient la réponse de l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1cb3e-104">The **GetMessageTrackingReportResponse** element contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
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

 <span data-ttu-id="1cb3e-105">**GetMessageTrackingReportResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1cb3e-105">**GetMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1cb3e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1cb3e-106">Attributes and elements</span></span>

<span data-ttu-id="1cb3e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cb3e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1cb3e-108">Attributes</span></span>

|<span data-ttu-id="1cb3e-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1cb3e-109">**Attribute**</span></span>|<span data-ttu-id="1cb3e-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="1cb3e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1cb3e-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="1cb3e-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1cb3e-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="1cb3e-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="1cb3e-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="1cb3e-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="1cb3e-114">-  Success</span></span>  <br/><span data-ttu-id="1cb3e-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="1cb3e-115">-  Warning</span></span>  <br/><span data-ttu-id="1cb3e-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="1cb3e-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="1cb3e-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="1cb3e-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="1cb3e-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1cb3e-118">**Value**</span></span>|<span data-ttu-id="1cb3e-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="1cb3e-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1cb3e-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="1cb3e-120">**Success**</span></span> <br/> |<span data-ttu-id="1cb3e-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1cb3e-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="1cb3e-122">**Warning**</span></span> <br/> | <span data-ttu-id="1cb3e-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-123">Describes a request that was not processed.</span></span> <span data-ttu-id="1cb3e-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="1cb3e-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="1cb3e-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="1cb3e-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="1cb3e-127">-Active Directory domaine sert (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-127">-  Active Directory Domain Serves (AD DS) is offline.</span></span>  <br/><span data-ttu-id="1cb3e-128">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="1cb3e-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="1cb3e-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="1cb3e-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="1cb3e-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="1cb3e-132">**Error**</span></span> <br/> | <span data-ttu-id="1cb3e-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="1cb3e-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="1cb3e-134">The following are examples of sources of errors:</span></span>  <br/>  <span data-ttu-id="1cb3e-135">Attributs non valides ou des éléments</span><span class="sxs-lookup"><span data-stu-id="1cb3e-135">Invalid attributes or elements</span></span>  <br/><br/><span data-ttu-id="1cb3e-136">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="1cb3e-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="1cb3e-137">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="1cb3e-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="1cb3e-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="1cb3e-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="1cb3e-139">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="1cb3e-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="1cb3e-140">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="1cb3e-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="1cb3e-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="1cb3e-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1cb3e-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1cb3e-142">Child elements</span></span>

|<span data-ttu-id="1cb3e-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1cb3e-143">**Element**</span></span>|<span data-ttu-id="1cb3e-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="1cb3e-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cb3e-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="1cb3e-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1cb3e-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1cb3e-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1cb3e-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1cb3e-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1cb3e-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1cb3e-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1cb3e-150">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="1cb3e-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1cb3e-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1cb3e-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1cb3e-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="1cb3e-154">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="1cb3e-154">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="1cb3e-155">Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1cb3e-155">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="1cb3e-156">Diagnostics</span><span class="sxs-lookup"><span data-stu-id="1cb3e-156">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="1cb3e-157">Fournit des informations de synchronisation et les performances qui sont utilisées pour la création de rapports dans un centre de données.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-157">Provides timing and performance information that is used for reporting in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="1cb3e-158">Erreurs</span><span class="sxs-lookup"><span data-stu-id="1cb3e-158">Errors</span></span>](errors-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1cb3e-159">Contient un ensemble de propriétés pour stocker les erreurs retournées par le service Web.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-159">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="1cb3e-160">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="1cb3e-160">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="1cb3e-161">Contient une liste d’un ou plusieurs des propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-161">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1cb3e-162">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1cb3e-162">Parent elements</span></span>

<span data-ttu-id="1cb3e-163">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-163">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="1cb3e-164">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1cb3e-164">Text value</span></span>

<span data-ttu-id="1cb3e-165">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1cb3e-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="1cb3e-166">Remarks</span></span>

<span data-ttu-id="1cb3e-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1cb3e-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1cb3e-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1cb3e-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cb3e-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1cb3e-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1cb3e-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1cb3e-170">Schema Name</span></span>  <br/> |<span data-ttu-id="1cb3e-171">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1cb3e-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1cb3e-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1cb3e-172">Validation File</span></span>  <br/> |<span data-ttu-id="1cb3e-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1cb3e-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1cb3e-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1cb3e-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="1cb3e-175">False</span><span class="sxs-lookup"><span data-stu-id="1cb3e-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1cb3e-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1cb3e-176">See also</span></span>

- [<span data-ttu-id="1cb3e-177">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="1cb3e-177">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="1cb3e-178">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1cb3e-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
