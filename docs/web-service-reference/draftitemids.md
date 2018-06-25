---
title: DraftItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c228f7e7-6dc8-476d-9b8c-99cd5b6f9f0c
description: L’élément DraftItemIds contient un tableau d’identificateurs d’élément pour les éléments de brouillon dans une conversation.
ms.openlocfilehash: f6639b20641ff68fff989d2de5fa4ec2c550d5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756047"
---
# <a name="draftitemids"></a><span data-ttu-id="59200-103">DraftItemIds</span><span class="sxs-lookup"><span data-stu-id="59200-103">DraftItemIds</span></span>

<span data-ttu-id="59200-104">L’élément **DraftItemIds** contient un tableau d’identificateurs d’élément pour les éléments de brouillon dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="59200-104">The **DraftItemIds** element contains an array of item identifiers to draft items in a conversation.</span></span> 
  
```XML
<DraftItemIds>
   <ItemId/>
   <OccirrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</DraftItemIds>
```

 <span data-ttu-id="59200-105">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="59200-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59200-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="59200-106">Attributes and elements</span></span>

<span data-ttu-id="59200-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="59200-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59200-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="59200-108">Attributes</span></span>

<span data-ttu-id="59200-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59200-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59200-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="59200-110">Child elements</span></span>

<span data-ttu-id="59200-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span><span class="sxs-lookup"><span data-stu-id="59200-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="59200-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="59200-112">Parent elements</span></span>

[<span data-ttu-id="59200-113">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="59200-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="remarks"></a><span data-ttu-id="59200-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="59200-114">Remarks</span></span>

<span data-ttu-id="59200-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="59200-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="59200-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="59200-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59200-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="59200-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59200-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="59200-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59200-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="59200-119">Schema name</span></span>  <br/> |<span data-ttu-id="59200-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="59200-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="59200-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="59200-121">Validation file</span></span>  <br/> |<span data-ttu-id="59200-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="59200-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59200-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="59200-123">Can be empty</span></span>  <br/> ||
   

