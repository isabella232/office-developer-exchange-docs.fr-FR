---
title: Indicateur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: L’élément Flag spécifie un indicateur sur un élément de boîte aux lettres.
ms.openlocfilehash: 7229a26181ee9baf80be5c32c0ef99483310ccb3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466261"
---
# <a name="flag"></a><span data-ttu-id="a8fa5-103">Indicateur</span><span class="sxs-lookup"><span data-stu-id="a8fa5-103">Flag</span></span>

<span data-ttu-id="a8fa5-104">L’élément **Flag** spécifie un indicateur sur un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a8fa5-104">The **Flag** element specifies a flag on a mailbox item.</span></span> 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 <span data-ttu-id="a8fa5-105">**FlagType**</span><span class="sxs-lookup"><span data-stu-id="a8fa5-105">**FlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8fa5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a8fa5-106">Attributes and elements</span></span>

<span data-ttu-id="a8fa5-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a8fa5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8fa5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a8fa5-108">Attributes</span></span>

<span data-ttu-id="a8fa5-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a8fa5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8fa5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a8fa5-110">Child elements</span></span>

|<span data-ttu-id="a8fa5-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a8fa5-111">**Element**</span></span>|<span data-ttu-id="a8fa5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8fa5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8fa5-113">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="a8fa5-113">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="a8fa5-114">Contient l’état de l’indicateur agrégé pour les éléments dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="a8fa5-114">Contains the aggregated flag status for items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="a8fa5-115">StartDate</span><span class="sxs-lookup"><span data-stu-id="a8fa5-115">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="a8fa5-116">Représente la date de début d’un élément.</span><span class="sxs-lookup"><span data-stu-id="a8fa5-116">Represents the start date of an item.</span></span>  <br/> |
|[<span data-ttu-id="a8fa5-117">DueDate</span><span class="sxs-lookup"><span data-stu-id="a8fa5-117">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="a8fa5-118">Représente la date d’échéance d’un élément.</span><span class="sxs-lookup"><span data-stu-id="a8fa5-118">Represents the date when an item is due.</span></span>  <br/> |
|[<span data-ttu-id="a8fa5-119">Terminé</span><span class="sxs-lookup"><span data-stu-id="a8fa5-119">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="a8fa5-120">Représente la date à laquelle un élément a été terminé.</span><span class="sxs-lookup"><span data-stu-id="a8fa5-120">Represents the date on which an item was completed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8fa5-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a8fa5-121">Parent elements</span></span>

|<span data-ttu-id="a8fa5-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a8fa5-122">**Element**</span></span>|<span data-ttu-id="a8fa5-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8fa5-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8fa5-124">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="a8fa5-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="a8fa5-125">Contient une seule action à appliquer à une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="a8fa5-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="a8fa5-126">Élément</span><span class="sxs-lookup"><span data-stu-id="a8fa5-126">Item</span></span>](item.md) <br/> |<span data-ttu-id="a8fa5-127">Représente un élément générique dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8fa5-127">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a8fa5-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="a8fa5-128">Remarks</span></span>

<span data-ttu-id="a8fa5-129">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a8fa5-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a8fa5-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8fa5-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8fa5-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a8fa5-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8fa5-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a8fa5-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8fa5-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a8fa5-133">Schema Name</span></span>  <br/> |<span data-ttu-id="a8fa5-134">Schéma type</span><span class="sxs-lookup"><span data-stu-id="a8fa5-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="a8fa5-135">Validation File</span><span class="sxs-lookup"><span data-stu-id="a8fa5-135">Validation File</span></span>  <br/> |<span data-ttu-id="a8fa5-136">types. xsd</span><span class="sxs-lookup"><span data-stu-id="a8fa5-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8fa5-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a8fa5-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a8fa5-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a8fa5-138">See also</span></span>



- [<span data-ttu-id="a8fa5-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a8fa5-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

