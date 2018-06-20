---
title: GetMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReport
api_type:
- schema
ms.assetid: b6ffa8ef-90f6-402d-afac-c3f5ee55cf49
description: L’élément GetMessageTrackingReport contient la demande pour l’opération GetMessageTrackingReport récupérer le message complet suivi du rapport pour l’ID spécifié.
ms.openlocfilehash: cb16f6e9d322cefb0d59c962af8e2f60ebae0e90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756680"
---
# <a name="getmessagetrackingreport"></a><span data-ttu-id="c6aff-103">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="c6aff-103">GetMessageTrackingReport</span></span>

<span data-ttu-id="c6aff-104">L’élément **GetMessageTrackingReport** contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) récupérer le message complet suivi du rapport pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="c6aff-104">The **GetMessageTrackingReport** element contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span> 
  
```XML
<GetMessageTrackingReport>
   <Scope/>
   <ReportTemplate/>
   <RecipientFilter/>
   <MessageTrackingReportId/>
   <ReturnQueueEvents/>
   <DiagnosticsLevel/>
   <Properties/>
</GetMessageTrackingReport>
```

 <span data-ttu-id="c6aff-105">**GetMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="c6aff-105">**GetMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6aff-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c6aff-106">Attributes and elements</span></span>

<span data-ttu-id="c6aff-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c6aff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6aff-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c6aff-108">Attributes</span></span>

<span data-ttu-id="c6aff-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c6aff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6aff-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c6aff-110">Child elements</span></span>

|<span data-ttu-id="c6aff-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c6aff-111">**Element**</span></span>|<span data-ttu-id="c6aff-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c6aff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6aff-113">Étendue (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="c6aff-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="c6aff-114">Spécifie l’emplacement où effectuer la recherche.</span><span class="sxs-lookup"><span data-stu-id="c6aff-114">Specifies where to perform the search.</span></span> <span data-ttu-id="c6aff-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c6aff-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c6aff-116">Modèle d’état</span><span class="sxs-lookup"><span data-stu-id="c6aff-116">ReportTemplate</span></span>](reporttemplate.md) <br/> |<span data-ttu-id="c6aff-117">Spécifie le type de suivi du rapport à récupérer.</span><span class="sxs-lookup"><span data-stu-id="c6aff-117">Specifies the type of tracking report to retrieve.</span></span> <span data-ttu-id="c6aff-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c6aff-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c6aff-119">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="c6aff-119">RecipientFilter</span></span>](recipientfilter.md) <br/> |<span data-ttu-id="c6aff-120">Spécifie une adresse de destinataire à utiliser avec le rapport de suivi spécifié.</span><span class="sxs-lookup"><span data-stu-id="c6aff-120">Specifies a recipient address to use with the specified tracking report.</span></span> <span data-ttu-id="c6aff-121">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="c6aff-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c6aff-122">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="c6aff-122">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="c6aff-123">Spécifie une chaîne d’identité qui proviennent de l’opération **FindMessageTrackingReport** .</span><span class="sxs-lookup"><span data-stu-id="c6aff-123">Specifies an identity string that was obtained from the **FindMessageTrackingReport** operation.</span></span> <span data-ttu-id="c6aff-124">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c6aff-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c6aff-125">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="c6aff-125">ReturnQueueEvents</span></span>](returnqueueevents.md) <br/> |<span data-ttu-id="c6aff-126">Spécifie que la personne qui exécute la tâche a un rôle de privilège.</span><span class="sxs-lookup"><span data-stu-id="c6aff-126">Specifies that the person who is running the task has a privileged role.</span></span> <span data-ttu-id="c6aff-127">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="c6aff-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c6aff-128">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="c6aff-128">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="c6aff-129">Spécifie les informations de synchronisation et les performances qui seront utilisées pour déterminer le rapport de suivi.</span><span class="sxs-lookup"><span data-stu-id="c6aff-129">Specifies timing and performance information that will be used to derive the tracking report.</span></span> <span data-ttu-id="c6aff-130">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="c6aff-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c6aff-131">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="c6aff-131">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="c6aff-132">Spécifie une liste d’un ou plusieurs des propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="c6aff-132">Specifies a list of one or more tracking properties.</span></span> <span data-ttu-id="c6aff-133">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="c6aff-133">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c6aff-134">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c6aff-134">Parent elements</span></span>

<span data-ttu-id="c6aff-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c6aff-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c6aff-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="c6aff-136">Remarks</span></span>

<span data-ttu-id="c6aff-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c6aff-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6aff-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c6aff-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6aff-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c6aff-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c6aff-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c6aff-140">Schema Name</span></span>  <br/> |<span data-ttu-id="c6aff-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c6aff-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c6aff-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c6aff-142">Validation File</span></span>  <br/> |<span data-ttu-id="c6aff-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c6aff-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c6aff-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c6aff-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6aff-145">False</span><span class="sxs-lookup"><span data-stu-id="c6aff-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6aff-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c6aff-146">See also</span></span>



[<span data-ttu-id="c6aff-147">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="c6aff-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="c6aff-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c6aff-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

