---
title: Propriétés (ArrayOfTrackingPropertiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Properties
api_type:
- schema
ms.assetid: 175566d2-fd62-45a2-8518-2827912cec88
description: L’élément Properties contient une liste d’un ou plusieurs des propriétés de suivi.
ms.openlocfilehash: 079d2d2c101fdeb7f26d65798048c3c6c59f3e94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828897"
---
# <a name="properties-arrayoftrackingpropertiestype"></a><span data-ttu-id="9a4e5-103">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="9a4e5-103">Properties (ArrayOfTrackingPropertiesType)</span></span>

<span data-ttu-id="9a4e5-104">L’élément **Properties** contient une liste d’un ou plusieurs des propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="9a4e5-104">The **Properties** element contains a list of one or more tracking properties.</span></span> 
  
- [<span data-ttu-id="9a4e5-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="9a4e5-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
- [<span data-ttu-id="9a4e5-106">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="9a4e5-106">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

<span data-ttu-id="9a4e5-107">**ArrayOfTrackingPropertiesType**</span><span class="sxs-lookup"><span data-stu-id="9a4e5-107">**ArrayOfTrackingPropertiesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9a4e5-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9a4e5-108">Attributes and elements</span></span>

<span data-ttu-id="9a4e5-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9a4e5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a4e5-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="9a4e5-110">Attributes</span></span>

<span data-ttu-id="9a4e5-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9a4e5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a4e5-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9a4e5-112">Child elements</span></span>

|<span data-ttu-id="9a4e5-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a4e5-113">**Element**</span></span>|<span data-ttu-id="9a4e5-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a4e5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a4e5-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="9a4e5-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="9a4e5-116">Représente une paire nom / valeur de chaînes qui sert à créer des propriétés pour les rapports de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="9a4e5-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a4e5-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9a4e5-117">Parent elements</span></span>

|<span data-ttu-id="9a4e5-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a4e5-118">**Element**</span></span>|<span data-ttu-id="9a4e5-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a4e5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a4e5-120">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="9a4e5-120">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="9a4e5-121">Spécifie les critères pour les types de messages.</span><span class="sxs-lookup"><span data-stu-id="9a4e5-121">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="9a4e5-122">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="9a4e5-122">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="9a4e5-123">Contient l’état et les résultats d’une seule demande [d’opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9a4e5-123">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9a4e5-124">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="9a4e5-124">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="9a4e5-125">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) récupérer le message complet suivi du rapport pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="9a4e5-125">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="9a4e5-126">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="9a4e5-126">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="9a4e5-127">Contient le résultat d’une seule demande [d’opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9a4e5-127">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9a4e5-128">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="9a4e5-128">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="9a4e5-129">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="9a4e5-129">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="9a4e5-130">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="9a4e5-130">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="9a4e5-131">Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9a4e5-131">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="9a4e5-132">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="9a4e5-132">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="9a4e5-133">Contient un résultat de message unique d’un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="9a4e5-133">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a4e5-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9a4e5-134">Text value</span></span>

<span data-ttu-id="9a4e5-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9a4e5-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a4e5-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="9a4e5-136">Remarks</span></span>

<span data-ttu-id="9a4e5-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9a4e5-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a4e5-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9a4e5-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a4e5-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9a4e5-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9a4e5-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9a4e5-140">Schema Name</span></span>  <br/> |<span data-ttu-id="9a4e5-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9a4e5-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9a4e5-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9a4e5-142">Validation File</span></span>  <br/> |<span data-ttu-id="9a4e5-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9a4e5-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9a4e5-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9a4e5-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a4e5-145">False</span><span class="sxs-lookup"><span data-stu-id="9a4e5-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a4e5-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9a4e5-146">See also</span></span>

- [<span data-ttu-id="9a4e5-147">Opération FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="9a4e5-147">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="9a4e5-148">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="9a4e5-148">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="9a4e5-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9a4e5-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

