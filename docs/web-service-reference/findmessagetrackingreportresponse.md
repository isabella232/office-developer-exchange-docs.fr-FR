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
description: L’élément FindMessageTrackingReportResponse contient l’État et le résultat d’une seule demande d’opération FindMessageTrackingReport.
ms.openlocfilehash: a72ae3b20f2cae3d37a90da36b816e6f3265c716
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462914"
---
# <a name="findmessagetrackingreportresponse"></a><span data-ttu-id="f0480-103">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="f0480-103">FindMessageTrackingReportResponse</span></span>

<span data-ttu-id="f0480-104">L’élément **FindMessageTrackingReportResponse** contient l’État et le résultat d’une seule demande d' [opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f0480-104">The **FindMessageTrackingReportResponse** element contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="f0480-105">**FindMessageTrackingReportResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f0480-105">**FindMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0480-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f0480-106">Attributes and elements</span></span>

<span data-ttu-id="f0480-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f0480-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0480-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f0480-108">Attributes</span></span>

|<span data-ttu-id="f0480-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="f0480-109">**Attribute**</span></span>|<span data-ttu-id="f0480-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="f0480-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f0480-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f0480-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f0480-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f0480-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="f0480-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="f0480-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="f0480-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="f0480-114">-  Success</span></span>  <br/><span data-ttu-id="f0480-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="f0480-115">-  Warning</span></span>  <br/><span data-ttu-id="f0480-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="f0480-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f0480-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f0480-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="f0480-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f0480-118">**Value**</span></span>|<span data-ttu-id="f0480-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="f0480-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f0480-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="f0480-120">**Success**</span></span> <br/> |<span data-ttu-id="f0480-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="f0480-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f0480-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f0480-122">**Warning**</span></span> <br/> | <span data-ttu-id="f0480-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="f0480-123">Describes a request that was not processed.</span></span> <span data-ttu-id="f0480-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="f0480-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="f0480-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="f0480-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="f0480-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="f0480-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f0480-127">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f0480-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="f0480-128">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="f0480-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="f0480-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f0480-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f0480-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="f0480-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="f0480-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="f0480-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="f0480-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="f0480-132">**Error**</span></span> <br/> | <span data-ttu-id="f0480-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="f0480-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f0480-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="f0480-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f0480-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="f0480-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f0480-136">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="f0480-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="f0480-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="f0480-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="f0480-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="f0480-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="f0480-139">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="f0480-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f0480-140">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="f0480-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="f0480-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f0480-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f0480-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f0480-142">Child elements</span></span>

|<span data-ttu-id="f0480-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f0480-143">**Element**</span></span>|<span data-ttu-id="f0480-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="f0480-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0480-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="f0480-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f0480-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f0480-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f0480-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f0480-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f0480-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="f0480-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f0480-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f0480-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f0480-150">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="f0480-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f0480-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="f0480-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f0480-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f0480-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f0480-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="f0480-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f0480-154">Diagnostics</span><span class="sxs-lookup"><span data-stu-id="f0480-154">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="f0480-155">Contient des informations qui seront utilisées pour produire différents rapports statistiques pour la fonctionnalité de suivi dans un centre de données.</span><span class="sxs-lookup"><span data-stu-id="f0480-155">Contains information that will be used to produce various statistical reports for the tracking feature in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="f0480-156">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="f0480-156">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="f0480-157">Contient et tableau de messages qui correspondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="f0480-157">Contains and array of messages that match the search requirements.</span></span>  <br/> |
|[<span data-ttu-id="f0480-158">ExecutedSearchScope</span><span class="sxs-lookup"><span data-stu-id="f0480-158">ExecutedSearchScope</span></span>](executedsearchscope.md) <br/> |<span data-ttu-id="f0480-159">Contient l’étendue de la recherche effectuée pour obtenir les résultats de la recherche.</span><span class="sxs-lookup"><span data-stu-id="f0480-159">Contains the scope of the search that was performed to get the search results.</span></span>  <br/> |
|[<span data-ttu-id="f0480-160">Erreurs</span><span class="sxs-lookup"><span data-stu-id="f0480-160">Errors</span></span>](errors-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f0480-161">Contient un conteneur de propriétés permettant de stocker les erreurs renvoyées via le service Web.</span><span class="sxs-lookup"><span data-stu-id="f0480-161">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="f0480-162">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="f0480-162">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="f0480-163">Contient une liste d’une ou plusieurs propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="f0480-163">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0480-164">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f0480-164">Parent elements</span></span>

<span data-ttu-id="f0480-165">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f0480-165">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f0480-166">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f0480-166">Text value</span></span>

<span data-ttu-id="f0480-167">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f0480-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f0480-168">Remarques</span><span class="sxs-lookup"><span data-stu-id="f0480-168">Remarks</span></span>

<span data-ttu-id="f0480-169">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0480-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0480-170">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f0480-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0480-171">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f0480-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f0480-172">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f0480-172">Schema Name</span></span>  <br/> |<span data-ttu-id="f0480-173">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f0480-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f0480-174">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f0480-174">Validation File</span></span>  <br/> |<span data-ttu-id="f0480-175">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f0480-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0480-176">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f0480-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0480-177">False</span><span class="sxs-lookup"><span data-stu-id="f0480-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0480-178">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f0480-178">See also</span></span>

- [<span data-ttu-id="f0480-179">Opération FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f0480-179">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="f0480-180">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f0480-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

