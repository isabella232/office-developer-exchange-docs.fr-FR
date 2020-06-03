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
description: L’élément properties contient une liste d’une ou plusieurs propriétés de suivi.
ms.openlocfilehash: 007a4dc14c84c47ea7af8ccacc554c134d563e44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465631"
---
# <a name="properties-arrayoftrackingpropertiestype"></a><span data-ttu-id="4c97d-103">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="4c97d-103">Properties (ArrayOfTrackingPropertiesType)</span></span>

<span data-ttu-id="4c97d-104">L’élément **Properties** contient une liste d’une ou plusieurs propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="4c97d-104">The **Properties** element contains a list of one or more tracking properties.</span></span> 
  
- [<span data-ttu-id="4c97d-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="4c97d-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
- [<span data-ttu-id="4c97d-106">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="4c97d-106">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

<span data-ttu-id="4c97d-107">**ArrayOfTrackingPropertiesType**</span><span class="sxs-lookup"><span data-stu-id="4c97d-107">**ArrayOfTrackingPropertiesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4c97d-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4c97d-108">Attributes and elements</span></span>

<span data-ttu-id="4c97d-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4c97d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c97d-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="4c97d-110">Attributes</span></span>

<span data-ttu-id="4c97d-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4c97d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c97d-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4c97d-112">Child elements</span></span>

|<span data-ttu-id="4c97d-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4c97d-113">**Element**</span></span>|<span data-ttu-id="4c97d-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="4c97d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c97d-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="4c97d-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="4c97d-116">Représente une paire nom/valeur de chaînes qui est utilisée pour créer des propriétés pour les rapports de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="4c97d-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4c97d-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4c97d-117">Parent elements</span></span>

|<span data-ttu-id="4c97d-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4c97d-118">**Element**</span></span>|<span data-ttu-id="4c97d-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="4c97d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c97d-120">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="4c97d-120">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="4c97d-121">Spécifie les critères pour les types de messages à rechercher.</span><span class="sxs-lookup"><span data-stu-id="4c97d-121">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="4c97d-122">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="4c97d-122">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="4c97d-123">Contient l’État et le résultat d’une seule demande d' [opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4c97d-123">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="4c97d-124">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="4c97d-124">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="4c97d-125">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) afin de récupérer le rapport de suivi complet des messages pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="4c97d-125">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="4c97d-126">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="4c97d-126">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="4c97d-127">Contient le résultat d’une demande d' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) unique.</span><span class="sxs-lookup"><span data-stu-id="4c97d-127">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="4c97d-128">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="4c97d-128">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="4c97d-129">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="4c97d-129">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="4c97d-130">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="4c97d-130">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="4c97d-131">Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4c97d-131">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="4c97d-132">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="4c97d-132">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="4c97d-133">Contient un seul résultat de message pour un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="4c97d-133">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4c97d-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4c97d-134">Text value</span></span>

<span data-ttu-id="4c97d-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4c97d-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4c97d-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="4c97d-136">Remarks</span></span>

<span data-ttu-id="4c97d-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4c97d-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c97d-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4c97d-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c97d-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4c97d-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4c97d-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4c97d-140">Schema Name</span></span>  <br/> |<span data-ttu-id="4c97d-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4c97d-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4c97d-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4c97d-142">Validation File</span></span>  <br/> |<span data-ttu-id="4c97d-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4c97d-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4c97d-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4c97d-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="4c97d-145">False</span><span class="sxs-lookup"><span data-stu-id="4c97d-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4c97d-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4c97d-146">See also</span></span>

- [<span data-ttu-id="4c97d-147">Opération FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="4c97d-147">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="4c97d-148">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="4c97d-148">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="4c97d-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4c97d-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

