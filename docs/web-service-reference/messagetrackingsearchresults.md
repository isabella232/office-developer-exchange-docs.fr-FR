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
ms.openlocfilehash: 1e03cb135b7b2a125da1e29f7293d233f4e20ddb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468676"
---
# <a name="messagetrackingsearchresults"></a><span data-ttu-id="3e068-103">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="3e068-103">MessageTrackingSearchResults</span></span>

<span data-ttu-id="3e068-104">L’élément **MessageTrackingSearchResults** contient une liste d’enregistrements qui correspondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="3e068-104">The **MessageTrackingSearchResults** element contains a list of records that match the search criteria.</span></span> 
  
```XML
<MessageTrackingSearchResults>
   <MessageTrackingSearchResult/>
</MessageTrackingSearchResults>
```

 <span data-ttu-id="3e068-105">**ArrayOfFindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="3e068-105">**ArrayOfFindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e068-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3e068-106">Attributes and elements</span></span>

<span data-ttu-id="3e068-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3e068-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e068-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3e068-108">Attributes</span></span>

<span data-ttu-id="3e068-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3e068-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e068-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3e068-110">Child elements</span></span>

|<span data-ttu-id="3e068-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e068-111">**Element**</span></span>|<span data-ttu-id="3e068-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e068-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e068-113">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="3e068-113">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="3e068-114">Contient un seul résultat de message pour un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="3e068-114">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3e068-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3e068-115">Parent elements</span></span>

|<span data-ttu-id="3e068-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e068-116">**Element**</span></span>|<span data-ttu-id="3e068-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e068-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e068-118">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="3e068-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="3e068-119">Contient l’État et le résultat d’une seule demande d' [opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3e068-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3e068-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3e068-120">Text value</span></span>

<span data-ttu-id="3e068-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3e068-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3e068-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="3e068-122">Remarks</span></span>

<span data-ttu-id="3e068-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e068-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e068-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3e068-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e068-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3e068-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3e068-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3e068-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3e068-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3e068-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3e068-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3e068-128">Validation File</span></span>  <br/> |<span data-ttu-id="3e068-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3e068-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3e068-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3e068-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3e068-131">False</span><span class="sxs-lookup"><span data-stu-id="3e068-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e068-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3e068-132">See also</span></span>



- [<span data-ttu-id="3e068-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3e068-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

