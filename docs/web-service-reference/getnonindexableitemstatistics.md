---
title: GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dd16d1fb-d82d-42e5-b64a-bc6c19c48fa8
description: L’élément GetNonIndexableItemStatistics spécifie une demande de récupération des statistiques d’éléments non indexables.
ms.openlocfilehash: 4b605379f20f5558566f1cfbad9ef1aa33b6fce6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452789"
---
# <a name="getnonindexableitemstatistics"></a><span data-ttu-id="9f301-103">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="9f301-103">GetNonIndexableItemStatistics</span></span>

<span data-ttu-id="9f301-104">L’élément **GetNonIndexableItemStatistics** spécifie une demande de récupération des statistiques d’éléments non indexables.</span><span class="sxs-lookup"><span data-stu-id="9f301-104">The **GetNonIndexableItemStatistics** element specifies a request to retrieve nonindexable item statistics.</span></span> 
  
```XML
<GetNonIndexableItemStatistics>
    <Mailboxes/>
</GetNonIndexableItemStatistics>
```

 <span data-ttu-id="9f301-105">**GetNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="9f301-105">**GetNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f301-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9f301-106">Attributes and elements</span></span>

<span data-ttu-id="9f301-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9f301-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f301-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9f301-108">Attributes</span></span>

<span data-ttu-id="9f301-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9f301-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f301-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9f301-110">Child elements</span></span>

|<span data-ttu-id="9f301-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9f301-111">**Element**</span></span>|<span data-ttu-id="9f301-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f301-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f301-113">Boîtes aux lettres (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="9f301-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="9f301-114">Spécifie un tableau d’éléments de **boîte aux lettres** .</span><span class="sxs-lookup"><span data-stu-id="9f301-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f301-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9f301-115">Parent elements</span></span>

<span data-ttu-id="9f301-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9f301-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9f301-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="9f301-117">Remarks</span></span>

<span data-ttu-id="9f301-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9f301-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9f301-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f301-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f301-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9f301-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f301-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9f301-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f301-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9f301-122">Schema Name</span></span>  <br/> |<span data-ttu-id="9f301-123">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="9f301-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="9f301-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9f301-124">Validation File</span></span>  <br/> |<span data-ttu-id="9f301-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9f301-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f301-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9f301-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9f301-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9f301-127">See also</span></span>



- [<span data-ttu-id="9f301-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9f301-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

