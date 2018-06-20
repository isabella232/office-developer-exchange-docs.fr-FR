---
title: MessageTrackingReportId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReportId
api_type:
- schema
ms.assetid: 9c604ca3-10fe-4760-b7fd-8b52f1a0c712
description: L’élément MessageTrackingReportId représente le message par son ID de message, l’organisation où le message a été trouvé, le serveur sur lequel le message a été envoyé et un ID interne qui identifie de manière unique le message.
ms.openlocfilehash: 8e0d85b203b8a34acedb5f6b9fe46359d5e0b97c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828456"
---
# <a name="messagetrackingreportid"></a><span data-ttu-id="b588d-103">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="b588d-103">MessageTrackingReportId</span></span>

<span data-ttu-id="b588d-104">L’élément **MessageTrackingReportId** représente le message par son ID de message, l’organisation où le message a été trouvé, le serveur sur lequel le message a été envoyé et un ID interne qui identifie de manière unique le message.</span><span class="sxs-lookup"><span data-stu-id="b588d-104">The **MessageTrackingReportId** element represents the message by its message ID, the organization where the message was found, the server on which the message was submitted, and an internal ID that uniquely identifies the message.</span></span> 
  
```XML
<MessageTrackingReportId/>
```

 <span data-ttu-id="b588d-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="b588d-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b588d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b588d-106">Attributes and elements</span></span>

<span data-ttu-id="b588d-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b588d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b588d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b588d-108">Attributes</span></span>

<span data-ttu-id="b588d-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b588d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b588d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b588d-110">Child elements</span></span>

<span data-ttu-id="b588d-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b588d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b588d-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b588d-112">Parent elements</span></span>

|<span data-ttu-id="b588d-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b588d-113">**Element**</span></span>|<span data-ttu-id="b588d-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b588d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b588d-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b588d-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="b588d-116">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) récupérer le message complet suivi du rapport pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="b588d-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="b588d-117">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="b588d-117">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="b588d-118">Contient un résultat de message unique d’un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="b588d-118">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b588d-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b588d-119">Text value</span></span>

<span data-ttu-id="b588d-120">Une valeur de texte qui représente une chaîne est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="b588d-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b588d-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="b588d-121">Remarks</span></span>

<span data-ttu-id="b588d-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b588d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b588d-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b588d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b588d-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b588d-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b588d-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b588d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b588d-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b588d-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="b588d-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b588d-127">Validation File</span></span>  <br/> |<span data-ttu-id="b588d-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b588d-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b588d-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b588d-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="b588d-130">False</span><span class="sxs-lookup"><span data-stu-id="b588d-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b588d-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b588d-131">See also</span></span>



[<span data-ttu-id="b588d-132">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b588d-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="b588d-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b588d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

