---
title: GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dd16d1fb-d82d-42e5-b64a-bc6c19c48fa8
description: L’élément GetNonIndexableItemStatistics spécifie une requête pour récupérer des statistiques d’élément nonindexable.
ms.openlocfilehash: 4e6f9a0ba94e9946a3910661810bc2c9e748ba9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756682"
---
# <a name="getnonindexableitemstatistics"></a><span data-ttu-id="dc4d9-103">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="dc4d9-103">GetNonIndexableItemStatistics</span></span>

<span data-ttu-id="dc4d9-104">L’élément **GetNonIndexableItemStatistics** spécifie une requête pour récupérer des statistiques d’élément nonindexable.</span><span class="sxs-lookup"><span data-stu-id="dc4d9-104">The **GetNonIndexableItemStatistics** element specifies a request to retrieve nonindexable item statistics.</span></span> 
  
```XML
<GetNonIndexableItemStatistics>
    <Mailboxes/>
</GetNonIndexableItemStatistics>
```

 <span data-ttu-id="dc4d9-105">**GetNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="dc4d9-105">**GetNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc4d9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dc4d9-106">Attributes and elements</span></span>

<span data-ttu-id="dc4d9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dc4d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc4d9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="dc4d9-108">Attributes</span></span>

<span data-ttu-id="dc4d9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dc4d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc4d9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dc4d9-110">Child elements</span></span>

|<span data-ttu-id="dc4d9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dc4d9-111">**Element**</span></span>|<span data-ttu-id="dc4d9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="dc4d9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc4d9-113">Boîtes aux lettres (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="dc4d9-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="dc4d9-114">Spécifie un tableau d’éléments de **boîte aux lettres** .</span><span class="sxs-lookup"><span data-stu-id="dc4d9-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc4d9-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dc4d9-115">Parent elements</span></span>

<span data-ttu-id="dc4d9-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dc4d9-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dc4d9-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="dc4d9-117">Remarks</span></span>

<span data-ttu-id="dc4d9-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="dc4d9-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dc4d9-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="dc4d9-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc4d9-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dc4d9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc4d9-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dc4d9-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dc4d9-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dc4d9-122">Schema Name</span></span>  <br/> |<span data-ttu-id="dc4d9-123">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="dc4d9-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="dc4d9-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dc4d9-124">Validation File</span></span>  <br/> |<span data-ttu-id="dc4d9-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dc4d9-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dc4d9-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dc4d9-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="dc4d9-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dc4d9-127">See also</span></span>



- [<span data-ttu-id="dc4d9-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dc4d9-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

