---
title: ReportTemplate
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
ms.openlocfilehash: 22f14d326032a30e5cb4c2c9e1aff390d98e95e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528698"
---
# <a name="reporttemplate"></a><span data-ttu-id="4a2ef-103">ReportTemplate</span><span class="sxs-lookup"><span data-stu-id="4a2ef-103">ReportTemplate</span></span>

<span data-ttu-id="4a2ef-104">L’élément **ReportTemplate** représente le type de rapport à obtenir.</span><span class="sxs-lookup"><span data-stu-id="4a2ef-104">The **ReportTemplate** element represents the type of report to get.</span></span> 
  
```xml
<ReportTemplate>Summary or RecipientPath</ReportTemplate>
```

 <span data-ttu-id="4a2ef-105">**MessageTrackingReportTemplateType**</span><span class="sxs-lookup"><span data-stu-id="4a2ef-105">**MessageTrackingReportTemplateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a2ef-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4a2ef-106">Attributes and elements</span></span>

<span data-ttu-id="4a2ef-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4a2ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a2ef-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4a2ef-108">Attributes</span></span>

<span data-ttu-id="4a2ef-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4a2ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a2ef-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4a2ef-110">Child elements</span></span>

<span data-ttu-id="4a2ef-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4a2ef-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4a2ef-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4a2ef-112">Parent elements</span></span>

|<span data-ttu-id="4a2ef-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a2ef-113">**Element**</span></span>|<span data-ttu-id="4a2ef-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a2ef-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a2ef-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="4a2ef-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="4a2ef-116">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) afin de récupérer le rapport de suivi complet des messages pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="4a2ef-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a2ef-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4a2ef-117">Text value</span></span>

<span data-ttu-id="4a2ef-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **ReportTemplate** .</span><span class="sxs-lookup"><span data-stu-id="4a2ef-118">The following table lists the possible values for the **ReportTemplate** element.</span></span> 
  
<span data-ttu-id="4a2ef-119">**Valeurs de l’élément ReportTemplate**</span><span class="sxs-lookup"><span data-stu-id="4a2ef-119">**ReportTemplate element values**</span></span>

|<span data-ttu-id="4a2ef-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4a2ef-120">**Value**</span></span>|<span data-ttu-id="4a2ef-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a2ef-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4a2ef-122">Résumé</span><span class="sxs-lookup"><span data-stu-id="4a2ef-122">Summary</span></span>  <br/> |<span data-ttu-id="4a2ef-123">Spécifie que le rapport affichera tous les destinataires du message et l’état de remise du message pour chaque destinataire.</span><span class="sxs-lookup"><span data-stu-id="4a2ef-123">Specifies that the report will display all the recipients of the message and the delivery status of the message to each recipient.</span></span>  <br/> |
|<span data-ttu-id="4a2ef-124">RecipientPath</span><span class="sxs-lookup"><span data-stu-id="4a2ef-124">RecipientPath</span></span>  <br/> |<span data-ttu-id="4a2ef-125">Spécifie que pour un destinataire unique, le rapport affichera un historique complet des événements qui se sont produits.</span><span class="sxs-lookup"><span data-stu-id="4a2ef-125">Specifies that for a single recipient, the report will display a full history of the events that occurred.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4a2ef-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="4a2ef-126">Remarks</span></span>

<span data-ttu-id="4a2ef-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4a2ef-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a2ef-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4a2ef-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a2ef-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4a2ef-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4a2ef-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4a2ef-130">Schema Name</span></span>  <br/> |<span data-ttu-id="4a2ef-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4a2ef-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4a2ef-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4a2ef-132">Validation File</span></span>  <br/> |<span data-ttu-id="4a2ef-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4a2ef-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4a2ef-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4a2ef-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a2ef-135">False</span><span class="sxs-lookup"><span data-stu-id="4a2ef-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a2ef-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4a2ef-136">See also</span></span>



- [<span data-ttu-id="4a2ef-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4a2ef-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

