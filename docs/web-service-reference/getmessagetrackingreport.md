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
description: L’élément GetMessageTrackingReport contient la demande pour l’opération GetMessageTrackingReport afin de récupérer le rapport de suivi complet des messages pour l’ID spécifié.
ms.openlocfilehash: 30596acd209580147e0f03e12a7868502159b29c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466576"
---
# <a name="getmessagetrackingreport"></a><span data-ttu-id="28de4-103">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="28de4-103">GetMessageTrackingReport</span></span>

<span data-ttu-id="28de4-104">L’élément **GetMessageTrackingReport** contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) afin de récupérer le rapport de suivi complet des messages pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="28de4-104">The **GetMessageTrackingReport** element contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span> 
  
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

 <span data-ttu-id="28de4-105">**GetMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="28de4-105">**GetMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28de4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="28de4-106">Attributes and elements</span></span>

<span data-ttu-id="28de4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="28de4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28de4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="28de4-108">Attributes</span></span>

<span data-ttu-id="28de4-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="28de4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28de4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="28de4-110">Child elements</span></span>

|<span data-ttu-id="28de4-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28de4-111">**Element**</span></span>|<span data-ttu-id="28de4-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="28de4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28de4-113">Étendue (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="28de4-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="28de4-114">Indique où effectuer la recherche.</span><span class="sxs-lookup"><span data-stu-id="28de4-114">Specifies where to perform the search.</span></span> <span data-ttu-id="28de4-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="28de4-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="28de4-116">ReportTemplate</span><span class="sxs-lookup"><span data-stu-id="28de4-116">ReportTemplate</span></span>](reporttemplate.md) <br/> |<span data-ttu-id="28de4-117">Spécifie le type de rapport de suivi à récupérer.</span><span class="sxs-lookup"><span data-stu-id="28de4-117">Specifies the type of tracking report to retrieve.</span></span> <span data-ttu-id="28de4-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="28de4-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="28de4-119">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="28de4-119">RecipientFilter</span></span>](recipientfilter.md) <br/> |<span data-ttu-id="28de4-120">Spécifie l’adresse d’un destinataire à utiliser avec le rapport de suivi spécifié.</span><span class="sxs-lookup"><span data-stu-id="28de4-120">Specifies a recipient address to use with the specified tracking report.</span></span> <span data-ttu-id="28de4-121">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="28de4-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="28de4-122">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="28de4-122">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="28de4-123">Spécifie une chaîne d’identité obtenue à partir de l’opération **FindMessageTrackingReport** .</span><span class="sxs-lookup"><span data-stu-id="28de4-123">Specifies an identity string that was obtained from the **FindMessageTrackingReport** operation.</span></span> <span data-ttu-id="28de4-124">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="28de4-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="28de4-125">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="28de4-125">ReturnQueueEvents</span></span>](returnqueueevents.md) <br/> |<span data-ttu-id="28de4-126">Spécifie que la personne qui exécute la tâche dispose d’un rôle privilégié.</span><span class="sxs-lookup"><span data-stu-id="28de4-126">Specifies that the person who is running the task has a privileged role.</span></span> <span data-ttu-id="28de4-127">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="28de4-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="28de4-128">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="28de4-128">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="28de4-129">Spécifie les informations de temps et de performances qui seront utilisées pour dériver le rapport de suivi.</span><span class="sxs-lookup"><span data-stu-id="28de4-129">Specifies timing and performance information that will be used to derive the tracking report.</span></span> <span data-ttu-id="28de4-130">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="28de4-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="28de4-131">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="28de4-131">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="28de4-132">Spécifie une liste d’une ou plusieurs propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="28de4-132">Specifies a list of one or more tracking properties.</span></span> <span data-ttu-id="28de4-133">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="28de4-133">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28de4-134">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="28de4-134">Parent elements</span></span>

<span data-ttu-id="28de4-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28de4-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28de4-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="28de4-136">Remarks</span></span>

<span data-ttu-id="28de4-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="28de4-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28de4-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="28de4-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28de4-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="28de4-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="28de4-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="28de4-140">Schema Name</span></span>  <br/> |<span data-ttu-id="28de4-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="28de4-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="28de4-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="28de4-142">Validation File</span></span>  <br/> |<span data-ttu-id="28de4-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="28de4-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28de4-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="28de4-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="28de4-145">False</span><span class="sxs-lookup"><span data-stu-id="28de4-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28de4-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="28de4-146">See also</span></span>



[<span data-ttu-id="28de4-147">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="28de4-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="28de4-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="28de4-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

