---
title: Erreurs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Errors
api_type:
- schema
ms.assetid: ea37a2b5-e2d1-4089-960f-7014b9535a50
description: L’élément erreurs contient un ensemble de propriétés pour stocker les erreurs retournées par le service Web.
ms.openlocfilehash: a029492c1e3c11cc31d3501bd4ea0024ef8ecb91
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756217"
---
# <a name="errors"></a><span data-ttu-id="240fd-103">Erreurs</span><span class="sxs-lookup"><span data-stu-id="240fd-103">Errors</span></span>

<span data-ttu-id="240fd-104">L’élément **erreurs** contient un ensemble de propriétés pour stocker les erreurs retournées par le service Web.</span><span class="sxs-lookup"><span data-stu-id="240fd-104">The **Errors** element contains a property bag to store errors that are returned through the Web service.</span></span> 
  
[<span data-ttu-id="240fd-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="240fd-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
[<span data-ttu-id="240fd-106">Erreurs</span><span class="sxs-lookup"><span data-stu-id="240fd-106">Errors</span></span>](errors-ex15websvcsotherref.md)
  
```xml
<Errors>
   <Properties/>
</Errors>
```

 <span data-ttu-id="240fd-107">**ArrayOfArraysOfTrackingPropertiesType**</span><span class="sxs-lookup"><span data-stu-id="240fd-107">**ArrayOfArraysOfTrackingPropertiesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="240fd-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="240fd-108">Attributes and elements</span></span>

<span data-ttu-id="240fd-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="240fd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="240fd-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="240fd-110">Attributes</span></span>

<span data-ttu-id="240fd-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="240fd-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="240fd-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="240fd-112">Child elements</span></span>

|<span data-ttu-id="240fd-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="240fd-113">**Element**</span></span>|<span data-ttu-id="240fd-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="240fd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="240fd-115">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="240fd-115">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="240fd-116">Contient une liste d’un ou plusieurs des propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="240fd-116">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="240fd-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="240fd-117">Parent elements</span></span>

|<span data-ttu-id="240fd-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="240fd-118">**Element**</span></span>|<span data-ttu-id="240fd-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="240fd-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="240fd-120">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="240fd-120">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="240fd-121">Contient l’état et les résultats d’une seule demande [d’opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="240fd-121">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="240fd-122">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="240fd-122">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="240fd-123">Contient le résultat d’une seule demande [d’opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="240fd-123">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="240fd-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="240fd-124">Text value</span></span>

<span data-ttu-id="240fd-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="240fd-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="240fd-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="240fd-126">Remarks</span></span>

<span data-ttu-id="240fd-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="240fd-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="240fd-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="240fd-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="240fd-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="240fd-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="240fd-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="240fd-130">Schema Name</span></span>  <br/> |<span data-ttu-id="240fd-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="240fd-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="240fd-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="240fd-132">Validation File</span></span>  <br/> |<span data-ttu-id="240fd-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="240fd-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="240fd-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="240fd-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="240fd-135">False</span><span class="sxs-lookup"><span data-stu-id="240fd-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="240fd-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="240fd-136">See also</span></span>



[<span data-ttu-id="240fd-137">Opération FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="240fd-137">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
  
[<span data-ttu-id="240fd-138">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="240fd-138">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="240fd-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="240fd-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

