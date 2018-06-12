---
title: NonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12f2934a-008c-4236-b8b3-7c7b6b5707e2
description: L’élément NonIndexableItemStatistics contient un tableau de statistiques relatives aux éléments qui ne peuvent pas être indexés.
ms.openlocfilehash: 1414053b6d39f4cd08ccfd1a11faaf1b13c2052b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828544"
---
# <a name="nonindexableitemstatistics"></a><span data-ttu-id="e8532-103">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="e8532-103">NonIndexableItemStatistics</span></span>

<span data-ttu-id="e8532-104">L’élément **NonIndexableItemStatistics** contient un tableau de statistiques relatives aux éléments qui ne peuvent pas être indexés.</span><span class="sxs-lookup"><span data-stu-id="e8532-104">The **NonIndexableItemStatistics** element contains an array of statistics for items that could not be indexed.</span></span> 
  
```XML
<NonIndexableItemStatistics>
   <NonIndexableItemStatistic/>
</NonIndexableItemStatistics>
```

 <span data-ttu-id="e8532-105">**ArrayOfNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="e8532-105">**ArrayOfNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8532-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e8532-106">Attributes and elements</span></span>

<span data-ttu-id="e8532-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e8532-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8532-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e8532-108">Attributes</span></span>

<span data-ttu-id="e8532-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e8532-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8532-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e8532-110">Child elements</span></span>

[<span data-ttu-id="e8532-111">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="e8532-111">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
  
### <a name="parent-elements"></a><span data-ttu-id="e8532-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e8532-112">Parent elements</span></span>

<span data-ttu-id="e8532-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="e8532-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8532-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="e8532-114">Remarks</span></span>

<span data-ttu-id="e8532-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e8532-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e8532-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8532-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8532-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e8532-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8532-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e8532-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e8532-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e8532-119">Schema name</span></span>  <br/> |<span data-ttu-id="e8532-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e8532-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e8532-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e8532-121">Validation file</span></span>  <br/> |<span data-ttu-id="e8532-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e8532-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8532-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e8532-123">Can be empty</span></span>  <br/> |<span data-ttu-id="e8532-124">False</span><span class="sxs-lookup"><span data-stu-id="e8532-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8532-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e8532-125">See also</span></span>



[<span data-ttu-id="e8532-126">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="e8532-126">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)


- [<span data-ttu-id="e8532-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e8532-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

