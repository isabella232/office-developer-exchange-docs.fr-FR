---
title: Modèle d’état
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReportTemplate
api_type:
- schema
ms.assetid: f528eee6-d5af-4745-8b00-a9834bf34be6
description: L’élément ReportTemplate représente le type de rapport à obtenir.
ms.openlocfilehash: 70aab69f4d20ad9fd7e878c7fccd16e261c9b94c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829118"
---
# <a name="reporttemplate"></a><span data-ttu-id="95033-103">Modèle d’état</span><span class="sxs-lookup"><span data-stu-id="95033-103">ReportTemplate</span></span>

<span data-ttu-id="95033-104">L’élément **ReportTemplate** représente le type de rapport à obtenir.</span><span class="sxs-lookup"><span data-stu-id="95033-104">The **ReportTemplate** element represents the type of report to get.</span></span> 
  
```xml
<ReportTemplate>Summary or RecipientPath</ReportTemplate>
```

 <span data-ttu-id="95033-105">**MessageTrackingReportTemplateType**</span><span class="sxs-lookup"><span data-stu-id="95033-105">**MessageTrackingReportTemplateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95033-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="95033-106">Attributes and elements</span></span>

<span data-ttu-id="95033-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="95033-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95033-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="95033-108">Attributes</span></span>

<span data-ttu-id="95033-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="95033-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95033-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="95033-110">Child elements</span></span>

<span data-ttu-id="95033-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="95033-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="95033-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="95033-112">Parent elements</span></span>

|<span data-ttu-id="95033-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="95033-113">**Element**</span></span>|<span data-ttu-id="95033-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="95033-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95033-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="95033-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="95033-116">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) récupérer le message complet suivi du rapport pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="95033-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="95033-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="95033-117">Text value</span></span>

<span data-ttu-id="95033-118">Le tableau suivant répertorie les valeurs possibles pour l’élément de **modèle d’état** .</span><span class="sxs-lookup"><span data-stu-id="95033-118">The following table lists the possible values for the **ReportTemplate** element.</span></span> 
  
<span data-ttu-id="95033-119">**Valeurs des éléments de modèle d’état**</span><span class="sxs-lookup"><span data-stu-id="95033-119">**ReportTemplate element values**</span></span>

|<span data-ttu-id="95033-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="95033-120">**Value**</span></span>|<span data-ttu-id="95033-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="95033-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="95033-122">Résumé</span><span class="sxs-lookup"><span data-stu-id="95033-122">Summary</span></span>  <br/> |<span data-ttu-id="95033-123">Spécifie que le rapport affiche tous les destinataires du message et l’état de remise du message pour chaque destinataire.</span><span class="sxs-lookup"><span data-stu-id="95033-123">Specifies that the report will display all the recipients of the message and the delivery status of the message to each recipient.</span></span>  <br/> |
|<span data-ttu-id="95033-124">RecipientPath</span><span class="sxs-lookup"><span data-stu-id="95033-124">RecipientPath</span></span>  <br/> |<span data-ttu-id="95033-125">Spécifie que pour un destinataire unique, le rapport affiche un historique complet des événements qui se sont produites.</span><span class="sxs-lookup"><span data-stu-id="95033-125">Specifies that for a single recipient, the report will display a full history of the events that occurred.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="95033-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="95033-126">Remarks</span></span>

<span data-ttu-id="95033-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="95033-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95033-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="95033-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95033-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="95033-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="95033-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="95033-130">Schema Name</span></span>  <br/> |<span data-ttu-id="95033-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="95033-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="95033-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="95033-132">Validation File</span></span>  <br/> |<span data-ttu-id="95033-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="95033-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="95033-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="95033-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="95033-135">False</span><span class="sxs-lookup"><span data-stu-id="95033-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95033-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="95033-136">See also</span></span>



- [<span data-ttu-id="95033-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="95033-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

