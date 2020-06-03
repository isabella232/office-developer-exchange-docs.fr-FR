---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: L’élément SeekToConditionPageItemView identifie la condition qui est utilisée pour identifier la fin d’une recherche, l’index de départ d’une recherche, les entrées maximales à renvoyer et les instructions de recherche pour une recherche FindItem ou FindConversation.
ms.openlocfilehash: dbb073263740ccdf75367f85f672b7d5ec78f7a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466835"
---
# <a name="seektoconditionpageitemview"></a><span data-ttu-id="82ac8-103">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="82ac8-103">SeekToConditionPageItemView</span></span>

<span data-ttu-id="82ac8-104">L’élément **SeekToConditionPageItemView** identifie la condition qui est utilisée pour identifier la fin d’une recherche, l’index de départ d’une recherche, les entrées maximales à renvoyer et les instructions de recherche pour une recherche **FindItem** ou **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="82ac8-104">The **SeekToConditionPageItemView** element identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span> 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 <span data-ttu-id="82ac8-105">**SeekToConditionPageViewType**</span><span class="sxs-lookup"><span data-stu-id="82ac8-105">**SeekToConditionPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82ac8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="82ac8-106">Attributes and elements</span></span>

<span data-ttu-id="82ac8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="82ac8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82ac8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="82ac8-108">Attributes</span></span>

|<span data-ttu-id="82ac8-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="82ac8-109">**Attribute**</span></span>|<span data-ttu-id="82ac8-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="82ac8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="82ac8-111">BasePoint</span><span class="sxs-lookup"><span data-stu-id="82ac8-111">BasePoint</span></span>  <br/> |<span data-ttu-id="82ac8-112">La valeur de texte de l’attribut **BasePoint** est le point de base de l’emplacement de démarrage de la recherche.</span><span class="sxs-lookup"><span data-stu-id="82ac8-112">The text value of the **BasePoint** attribute is the base point from where the search will start.</span></span> <span data-ttu-id="82ac8-113">Une valeur de **départ** indique que la recherche commence au début du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="82ac8-113">A text value of **Beginning** indicates that the search will start at the beginning of the result set.</span></span> <span data-ttu-id="82ac8-114">Une valeur de **fin** indique que la recherche commence à la fin du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="82ac8-114">A text value of **End** indicates that the search will start at the end of the result set.</span></span>  <br/> |
|<span data-ttu-id="82ac8-115">MaxEntriesReturned</span><span class="sxs-lookup"><span data-stu-id="82ac8-115">MaxEntriesReturned</span></span>  <br/> |<span data-ttu-id="82ac8-116">La valeur de texte de l’attribut **MaxEntriesReturned** est le nombre maximal d’éléments qui peuvent être renvoyés dans un jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="82ac8-116">The text value of the **MaxEntriesReturned** attribute is the maximum number of items that can be returned in a result set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="82ac8-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="82ac8-117">Child elements</span></span>

[<span data-ttu-id="82ac8-118">Condition (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="82ac8-118">Condition (RestrictionType)</span></span>](condition-restrictiontype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="82ac8-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="82ac8-119">Parent elements</span></span>

<span data-ttu-id="82ac8-120">[FindConversation](findconversation.md)  |  [FindItem](finditem.md)</span><span class="sxs-lookup"><span data-stu-id="82ac8-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="82ac8-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="82ac8-121">Remarks</span></span>

<span data-ttu-id="82ac8-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="82ac8-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="82ac8-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="82ac8-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82ac8-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="82ac8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82ac8-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="82ac8-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="82ac8-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="82ac8-126">Schema name</span></span>  <br/> |<span data-ttu-id="82ac8-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="82ac8-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="82ac8-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="82ac8-128">Validation file</span></span>  <br/> |<span data-ttu-id="82ac8-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="82ac8-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="82ac8-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="82ac8-130">Can be empty</span></span>  <br/> |<span data-ttu-id="82ac8-131">false</span><span class="sxs-lookup"><span data-stu-id="82ac8-131">false</span></span>  <br/> |
   

