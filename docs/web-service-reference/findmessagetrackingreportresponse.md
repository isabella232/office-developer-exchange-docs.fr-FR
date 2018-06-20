---
title: FindMessageTrackingReportResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReportResponse
api_type:
- schema
ms.assetid: ed4265dc-0e79-4b34-8bf4-88a94875629d
description: L’élément FindMessageTrackingReportResponse contient l’état et les résultats d’une demande d’opération FindMessageTrackingReport unique.
ms.openlocfilehash: fa381f500eac9a46b11aea8c813f1ffc625a3bc3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756414"
---
# <a name="findmessagetrackingreportresponse"></a><span data-ttu-id="a8992-103">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="a8992-103">FindMessageTrackingReportResponse</span></span>

<span data-ttu-id="a8992-104">L’élément **FindMessageTrackingReportResponse** contient l’état et les résultats d’une seule demande [d’opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a8992-104">The **FindMessageTrackingReportResponse** element contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span> 
  
```xml
<FindMessageTrackingReportResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Diagnostics/>
   <MessageTrackingSearchResults/>
   <Errors/>
   <Properties/>
</FindMessageTrackingReportResponse>
```

 <span data-ttu-id="a8992-105">**FindMessageTrackingReportResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a8992-105">**FindMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8992-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a8992-106">Attributes and elements</span></span>

<span data-ttu-id="a8992-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a8992-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8992-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a8992-108">Attributes</span></span>

|<span data-ttu-id="a8992-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a8992-109">**Attribute**</span></span>|<span data-ttu-id="a8992-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8992-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a8992-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="a8992-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a8992-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="a8992-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="a8992-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="a8992-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="a8992-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="a8992-114">-  Success</span></span>  <br/><span data-ttu-id="a8992-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="a8992-115">-  Warning</span></span>  <br/><span data-ttu-id="a8992-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="a8992-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="a8992-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a8992-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="a8992-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a8992-118">**Value**</span></span>|<span data-ttu-id="a8992-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8992-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a8992-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="a8992-120">**Success**</span></span> <br/> |<span data-ttu-id="a8992-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="a8992-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a8992-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="a8992-122">**Warning**</span></span> <br/> | <span data-ttu-id="a8992-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="a8992-123">Describes a request that was not processed.</span></span> <span data-ttu-id="a8992-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="a8992-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="a8992-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="a8992-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="a8992-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="a8992-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="a8992-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="a8992-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="a8992-128">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="a8992-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="a8992-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="a8992-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="a8992-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="a8992-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="a8992-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="a8992-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="a8992-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="a8992-132">**Error**</span></span> <br/> | <span data-ttu-id="a8992-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="a8992-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="a8992-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="a8992-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="a8992-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="a8992-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="a8992-136">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="a8992-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="a8992-137">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="a8992-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="a8992-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="a8992-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="a8992-139">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="a8992-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="a8992-140">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="a8992-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="a8992-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="a8992-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a8992-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a8992-142">Child elements</span></span>

|<span data-ttu-id="a8992-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a8992-143">**Element**</span></span>|<span data-ttu-id="a8992-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8992-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8992-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="a8992-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a8992-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="a8992-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a8992-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a8992-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a8992-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="a8992-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="a8992-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a8992-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a8992-150">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="a8992-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="a8992-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="a8992-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a8992-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a8992-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a8992-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="a8992-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a8992-154">Diagnostics</span><span class="sxs-lookup"><span data-stu-id="a8992-154">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="a8992-155">Contient des informations qui seront utilisées pour générer des rapports de statistiques différentes pour la fonctionnalité de suivi dans un centre de données.</span><span class="sxs-lookup"><span data-stu-id="a8992-155">Contains information that will be used to produce various statistical reports for the tracking feature in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="a8992-156">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="a8992-156">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="a8992-157">Contient les tableau des messages qui correspondent à la configuration requise de recherche.</span><span class="sxs-lookup"><span data-stu-id="a8992-157">Contains and array of messages that match the search requirements.</span></span>  <br/> |
|[<span data-ttu-id="a8992-158">ExecutedSearchScope</span><span class="sxs-lookup"><span data-stu-id="a8992-158">ExecutedSearchScope</span></span>](executedsearchscope.md) <br/> |<span data-ttu-id="a8992-159">Contient l’étendue de la recherche a été effectuée pour obtenir les résultats de recherche.</span><span class="sxs-lookup"><span data-stu-id="a8992-159">Contains the scope of the search that was performed to get the search results.</span></span>  <br/> |
|[<span data-ttu-id="a8992-160">Erreurs</span><span class="sxs-lookup"><span data-stu-id="a8992-160">Errors</span></span>](errors-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a8992-161">Contient un ensemble de propriétés pour stocker les erreurs retournées par le service Web.</span><span class="sxs-lookup"><span data-stu-id="a8992-161">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="a8992-162">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="a8992-162">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="a8992-163">Contient une liste d’un ou plusieurs des propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="a8992-163">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8992-164">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a8992-164">Parent elements</span></span>

<span data-ttu-id="a8992-165">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a8992-165">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a8992-166">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a8992-166">Text value</span></span>

<span data-ttu-id="a8992-167">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a8992-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8992-168">Remarques</span><span class="sxs-lookup"><span data-stu-id="a8992-168">Remarks</span></span>

<span data-ttu-id="a8992-169">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8992-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8992-170">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a8992-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8992-171">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a8992-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a8992-172">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a8992-172">Schema Name</span></span>  <br/> |<span data-ttu-id="a8992-173">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a8992-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a8992-174">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a8992-174">Validation File</span></span>  <br/> |<span data-ttu-id="a8992-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a8992-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a8992-176">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a8992-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8992-177">False</span><span class="sxs-lookup"><span data-stu-id="a8992-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8992-178">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a8992-178">See also</span></span>

- [<span data-ttu-id="a8992-179">Opération FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="a8992-179">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="a8992-180">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a8992-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

