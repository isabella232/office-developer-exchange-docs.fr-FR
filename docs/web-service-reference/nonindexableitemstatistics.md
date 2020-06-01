---
title: NonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12f2934a-008c-4236-b8b3-7c7b6b5707e2
description: L’élément NonIndexableItemStatistics contient un tableau de statistiques pour les éléments qui n’ont pas pu être indexés.
ms.openlocfilehash: 5a11bd4d7ef0c574f26580613063a885530176f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466730"
---
# <a name="nonindexableitemstatistics"></a><span data-ttu-id="83afb-103">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="83afb-103">NonIndexableItemStatistics</span></span>

<span data-ttu-id="83afb-104">L’élément **NonIndexableItemStatistics** contient un tableau de statistiques pour les éléments qui n’ont pas pu être indexés.</span><span class="sxs-lookup"><span data-stu-id="83afb-104">The **NonIndexableItemStatistics** element contains an array of statistics for items that could not be indexed.</span></span> 
  
```XML
<NonIndexableItemStatistics>
   <NonIndexableItemStatistic/>
</NonIndexableItemStatistics>
```

 <span data-ttu-id="83afb-105">**ArrayOfNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="83afb-105">**ArrayOfNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83afb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="83afb-106">Attributes and elements</span></span>

<span data-ttu-id="83afb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="83afb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83afb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="83afb-108">Attributes</span></span>

<span data-ttu-id="83afb-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="83afb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83afb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="83afb-110">Child elements</span></span>

[<span data-ttu-id="83afb-111">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="83afb-111">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
  
### <a name="parent-elements"></a><span data-ttu-id="83afb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="83afb-112">Parent elements</span></span>

<span data-ttu-id="83afb-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="83afb-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="83afb-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="83afb-114">Remarks</span></span>

<span data-ttu-id="83afb-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="83afb-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="83afb-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="83afb-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83afb-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="83afb-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83afb-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="83afb-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="83afb-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="83afb-119">Schema name</span></span>  <br/> |<span data-ttu-id="83afb-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="83afb-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="83afb-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="83afb-121">Validation file</span></span>  <br/> |<span data-ttu-id="83afb-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="83afb-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="83afb-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="83afb-123">Can be empty</span></span>  <br/> |<span data-ttu-id="83afb-124">False</span><span class="sxs-lookup"><span data-stu-id="83afb-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83afb-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="83afb-125">See also</span></span>



[<span data-ttu-id="83afb-126">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="83afb-126">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)


- [<span data-ttu-id="83afb-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="83afb-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

