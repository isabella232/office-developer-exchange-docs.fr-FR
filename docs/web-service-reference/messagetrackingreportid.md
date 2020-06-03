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
ms.openlocfilehash: d6e92593d55608e260634602c2aab694804d716d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460595"
---
# <a name="messagetrackingreportid"></a><span data-ttu-id="842e0-103">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="842e0-103">MessageTrackingReportId</span></span>

<span data-ttu-id="842e0-104">L’élément **MessageTrackingReportId** représente le message par son ID de message, l’organisation où le message a été trouvé, le serveur sur lequel le message a été envoyé et un ID interne qui identifie de manière unique le message.</span><span class="sxs-lookup"><span data-stu-id="842e0-104">The **MessageTrackingReportId** element represents the message by its message ID, the organization where the message was found, the server on which the message was submitted, and an internal ID that uniquely identifies the message.</span></span> 
  
```XML
<MessageTrackingReportId/>
```

 <span data-ttu-id="842e0-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="842e0-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="842e0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="842e0-106">Attributes and elements</span></span>

<span data-ttu-id="842e0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="842e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="842e0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="842e0-108">Attributes</span></span>

<span data-ttu-id="842e0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="842e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="842e0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="842e0-110">Child elements</span></span>

<span data-ttu-id="842e0-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="842e0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="842e0-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="842e0-112">Parent elements</span></span>

|<span data-ttu-id="842e0-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="842e0-113">**Element**</span></span>|<span data-ttu-id="842e0-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="842e0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="842e0-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="842e0-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="842e0-116">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) afin de récupérer le rapport de suivi complet des messages pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="842e0-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="842e0-117">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="842e0-117">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="842e0-118">Contient un seul résultat de message pour un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="842e0-118">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="842e0-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="842e0-119">Text value</span></span>

<span data-ttu-id="842e0-120">Une valeur de texte qui représente une chaîne est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="842e0-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="842e0-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="842e0-121">Remarks</span></span>

<span data-ttu-id="842e0-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="842e0-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="842e0-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="842e0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="842e0-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="842e0-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="842e0-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="842e0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="842e0-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="842e0-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="842e0-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="842e0-127">Validation File</span></span>  <br/> |<span data-ttu-id="842e0-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="842e0-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="842e0-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="842e0-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="842e0-130">False</span><span class="sxs-lookup"><span data-stu-id="842e0-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="842e0-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="842e0-131">See also</span></span>



[<span data-ttu-id="842e0-132">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="842e0-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="842e0-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="842e0-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

