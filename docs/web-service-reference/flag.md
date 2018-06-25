---
title: Indicateur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: L’élément indicateur spécifie un indicateur sur un élément de boîte aux lettres.
ms.openlocfilehash: f30f435e8f064d7165ae52de737bbd75b0546206
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756433"
---
# <a name="flag"></a><span data-ttu-id="aeb8f-103">Indicateur</span><span class="sxs-lookup"><span data-stu-id="aeb8f-103">Flag</span></span>

<span data-ttu-id="aeb8f-104">L’élément **indicateur** spécifie un indicateur sur un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="aeb8f-104">The **Flag** element specifies a flag on a mailbox item.</span></span> 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 <span data-ttu-id="aeb8f-105">**FlagType**</span><span class="sxs-lookup"><span data-stu-id="aeb8f-105">**FlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aeb8f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aeb8f-106">Attributes and elements</span></span>

<span data-ttu-id="aeb8f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aeb8f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aeb8f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="aeb8f-108">Attributes</span></span>

<span data-ttu-id="aeb8f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aeb8f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aeb8f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aeb8f-110">Child elements</span></span>

|<span data-ttu-id="aeb8f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aeb8f-111">**Element**</span></span>|<span data-ttu-id="aeb8f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="aeb8f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aeb8f-113">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="aeb8f-113">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="aeb8f-114">Contient l’état de l’indicateur agrégées pour les éléments dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="aeb8f-114">Contains the aggregated flag status for items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="aeb8f-115">Date de début</span><span class="sxs-lookup"><span data-stu-id="aeb8f-115">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="aeb8f-116">Représente la date de début d’un élément.</span><span class="sxs-lookup"><span data-stu-id="aeb8f-116">Represents the start date of an item.</span></span>  <br/> |
|[<span data-ttu-id="aeb8f-117">DueDate</span><span class="sxs-lookup"><span data-stu-id="aeb8f-117">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="aeb8f-118">Représente la date à laquelle un élément est due.</span><span class="sxs-lookup"><span data-stu-id="aeb8f-118">Represents the date when an item is due.</span></span>  <br/> |
|[<span data-ttu-id="aeb8f-119">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="aeb8f-119">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="aeb8f-120">Représente la date à laquelle un élément a été effectué.</span><span class="sxs-lookup"><span data-stu-id="aeb8f-120">Represents the date on which an item was completed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aeb8f-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aeb8f-121">Parent elements</span></span>

|<span data-ttu-id="aeb8f-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aeb8f-122">**Element**</span></span>|<span data-ttu-id="aeb8f-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="aeb8f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aeb8f-124">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="aeb8f-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="aeb8f-125">Contient une seule action à appliquer à une même conversation.</span><span class="sxs-lookup"><span data-stu-id="aeb8f-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="aeb8f-126">Item</span><span class="sxs-lookup"><span data-stu-id="aeb8f-126">Item</span></span>](item.md) <br/> |<span data-ttu-id="aeb8f-127">Représente un élément générique dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="aeb8f-127">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aeb8f-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="aeb8f-128">Remarks</span></span>

<span data-ttu-id="aeb8f-129">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="aeb8f-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aeb8f-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="aeb8f-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aeb8f-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aeb8f-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aeb8f-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aeb8f-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aeb8f-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aeb8f-133">Schema Name</span></span>  <br/> |<span data-ttu-id="aeb8f-134">Schéma type</span><span class="sxs-lookup"><span data-stu-id="aeb8f-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="aeb8f-135">Validation File</span><span class="sxs-lookup"><span data-stu-id="aeb8f-135">Validation File</span></span>  <br/> |<span data-ttu-id="aeb8f-136">types.xsd</span><span class="sxs-lookup"><span data-stu-id="aeb8f-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="aeb8f-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aeb8f-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="aeb8f-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aeb8f-138">See also</span></span>



- [<span data-ttu-id="aeb8f-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="aeb8f-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

