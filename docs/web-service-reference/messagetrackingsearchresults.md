---
title: MessageTrackingSearchResults
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResults
api_type:
- schema
ms.assetid: 6bf36f37-c2b3-40c1-a4df-31573ed8642a
description: L’élément MessageTrackingSearchResults contient une liste d’enregistrements qui correspondent aux critères de recherche.
ms.openlocfilehash: 866cc8d4e9afa8347eb7bd0d9e9acaddc616c396
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828454"
---
# <a name="messagetrackingsearchresults"></a><span data-ttu-id="1a4f9-103">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="1a4f9-103">MessageTrackingSearchResults</span></span>

<span data-ttu-id="1a4f9-104">L’élément **MessageTrackingSearchResults** contient une liste d’enregistrements qui correspondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="1a4f9-104">The **MessageTrackingSearchResults** element contains a list of records that match the search criteria.</span></span> 
  
```XML
<MessageTrackingSearchResults>
   <MessageTrackingSearchResult/>
</MessageTrackingSearchResults>
```

 <span data-ttu-id="1a4f9-105">**ArrayOfFindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="1a4f9-105">**ArrayOfFindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a4f9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1a4f9-106">Attributes and elements</span></span>

<span data-ttu-id="1a4f9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1a4f9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a4f9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1a4f9-108">Attributes</span></span>

<span data-ttu-id="1a4f9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1a4f9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a4f9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1a4f9-110">Child elements</span></span>

|<span data-ttu-id="1a4f9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1a4f9-111">**Element**</span></span>|<span data-ttu-id="1a4f9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a4f9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a4f9-113">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="1a4f9-113">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="1a4f9-114">Contient un résultat de message unique d’un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="1a4f9-114">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a4f9-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1a4f9-115">Parent elements</span></span>

|<span data-ttu-id="1a4f9-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1a4f9-116">**Element**</span></span>|<span data-ttu-id="1a4f9-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a4f9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a4f9-118">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="1a4f9-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="1a4f9-119">Contient l’état et les résultats d’une seule demande [d’opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1a4f9-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a4f9-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1a4f9-120">Text value</span></span>

<span data-ttu-id="1a4f9-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1a4f9-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1a4f9-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="1a4f9-122">Remarks</span></span>

<span data-ttu-id="1a4f9-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a4f9-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a4f9-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1a4f9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a4f9-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1a4f9-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1a4f9-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1a4f9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="1a4f9-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1a4f9-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1a4f9-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1a4f9-128">Validation File</span></span>  <br/> |<span data-ttu-id="1a4f9-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1a4f9-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1a4f9-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1a4f9-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a4f9-131">False</span><span class="sxs-lookup"><span data-stu-id="1a4f9-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a4f9-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1a4f9-132">See also</span></span>



- [<span data-ttu-id="1a4f9-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1a4f9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

