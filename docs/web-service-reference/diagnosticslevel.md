---
title: DiagnosticsLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DiagnosticsLevel
api_type:
- schema
ms.assetid: 66794226-f5e0-44f0-8a0e-1f194bb0ba0f
description: L’élément DiagnosticsLevel représente les informations de synchronisation et les performances qui seront utilisées pour déterminer l’état.
ms.openlocfilehash: 9205625bb6cf38e370e29d96770eb293ed9277f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755914"
---
# <a name="diagnosticslevel"></a><span data-ttu-id="ee9c4-103">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="ee9c4-103">DiagnosticsLevel</span></span>

<span data-ttu-id="ee9c4-104">L’élément **DiagnosticsLevel** représente les informations de synchronisation et les performances qui seront utilisées pour déterminer l’état.</span><span class="sxs-lookup"><span data-stu-id="ee9c4-104">The **DiagnosticsLevel** element represents timing and performance information that will be used to derive the report.</span></span> 
  
```XML
<DiagnosticsLevel/>
```

 <span data-ttu-id="ee9c4-105">**string**</span><span class="sxs-lookup"><span data-stu-id="ee9c4-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee9c4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ee9c4-106">Attributes and elements</span></span>

<span data-ttu-id="ee9c4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ee9c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee9c4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ee9c4-108">Attributes</span></span>

<span data-ttu-id="ee9c4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ee9c4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ee9c4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ee9c4-110">Child elements</span></span>

<span data-ttu-id="ee9c4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ee9c4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ee9c4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ee9c4-112">Parent elements</span></span>

|<span data-ttu-id="ee9c4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ee9c4-113">**Element**</span></span>|<span data-ttu-id="ee9c4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ee9c4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee9c4-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="ee9c4-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="ee9c4-116">Contient des critères pour les types de messages.</span><span class="sxs-lookup"><span data-stu-id="ee9c4-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="ee9c4-117">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="ee9c4-117">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="ee9c4-118">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) récupérer le message complet suivi du rapport pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="ee9c4-118">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ee9c4-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ee9c4-119">Text value</span></span>

<span data-ttu-id="ee9c4-120">Une valeur de texte qui représente une chaîne est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="ee9c4-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ee9c4-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="ee9c4-121">Remarks</span></span>

<span data-ttu-id="ee9c4-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee9c4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee9c4-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ee9c4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee9c4-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ee9c4-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ee9c4-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ee9c4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ee9c4-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ee9c4-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ee9c4-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ee9c4-127">Validation File</span></span>  <br/> |<span data-ttu-id="ee9c4-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ee9c4-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ee9c4-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ee9c4-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ee9c4-130">False</span><span class="sxs-lookup"><span data-stu-id="ee9c4-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee9c4-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ee9c4-131">See also</span></span>

- [<span data-ttu-id="ee9c4-132">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="ee9c4-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="ee9c4-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ee9c4-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

