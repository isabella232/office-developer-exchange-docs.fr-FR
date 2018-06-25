---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: L’élément SeekToConditionPageItemView identifie la condition est utilisée pour identifier la fin d’une recherche, l’index de début d’une recherche, les entrées maximum pour renvoyer et les instructions de recherche pour une recherche FindItem ou FindConversation.
ms.openlocfilehash: e95246079f8c6e7acffac1dabb278895265767d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829328"
---
# <a name="seektoconditionpageitemview"></a><span data-ttu-id="f98e3-103">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="f98e3-103">SeekToConditionPageItemView</span></span>

<span data-ttu-id="f98e3-104">L’élément **SeekToConditionPageItemView** identifie la condition est utilisée pour identifier la fin d’une recherche, l’index de début d’une recherche, les entrées maximum pour renvoyer et les instructions de recherche pour un **FindItem** ou un **FindConversation **recherche.</span><span class="sxs-lookup"><span data-stu-id="f98e3-104">The **SeekToConditionPageItemView** element identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span> 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 <span data-ttu-id="f98e3-105">**SeekToConditionPageViewType**</span><span class="sxs-lookup"><span data-stu-id="f98e3-105">**SeekToConditionPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f98e3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f98e3-106">Attributes and elements</span></span>

<span data-ttu-id="f98e3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f98e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f98e3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f98e3-108">Attributes</span></span>

|<span data-ttu-id="f98e3-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="f98e3-109">**Attribute**</span></span>|<span data-ttu-id="f98e3-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="f98e3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f98e3-111">Point de base</span><span class="sxs-lookup"><span data-stu-id="f98e3-111">BasePoint</span></span>  <br/> |<span data-ttu-id="f98e3-112">La valeur de texte de l’attribut de **point de base** est le point de base à partir de dans laquelle la recherche est lancée.</span><span class="sxs-lookup"><span data-stu-id="f98e3-112">The text value of the **BasePoint** attribute is the base point from where the search will start.</span></span> <span data-ttu-id="f98e3-113">Une valeur de texte de **début** indique que la recherche commence au début du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="f98e3-113">A text value of **Beginning** indicates that the search will start at the beginning of the result set.</span></span> <span data-ttu-id="f98e3-114">Une valeur de texte **fin** indique que la recherche démarre à la fin du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="f98e3-114">A text value of **End** indicates that the search will start at the end of the result set.</span></span>  <br/> |
|<span data-ttu-id="f98e3-115">MaxEntriesReturned</span><span class="sxs-lookup"><span data-stu-id="f98e3-115">MaxEntriesReturned</span></span>  <br/> |<span data-ttu-id="f98e3-116">La valeur de texte de l’attribut **MaxEntriesReturned** est le nombre maximal d’éléments pouvant être renvoyés dans un jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="f98e3-116">The text value of the **MaxEntriesReturned** attribute is the maximum number of items that can be returned in a result set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f98e3-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f98e3-117">Child elements</span></span>

[<span data-ttu-id="f98e3-118">Condition (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="f98e3-118">Condition (RestrictionType)</span></span>](condition-restrictiontype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="f98e3-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f98e3-119">Parent elements</span></span>

<span data-ttu-id="f98e3-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span><span class="sxs-lookup"><span data-stu-id="f98e3-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f98e3-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="f98e3-121">Remarks</span></span>

<span data-ttu-id="f98e3-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f98e3-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f98e3-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f98e3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f98e3-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f98e3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f98e3-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f98e3-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f98e3-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f98e3-126">Schema name</span></span>  <br/> |<span data-ttu-id="f98e3-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f98e3-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f98e3-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f98e3-128">Validation file</span></span>  <br/> |<span data-ttu-id="f98e3-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f98e3-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f98e3-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f98e3-130">Can be empty</span></span>  <br/> |<span data-ttu-id="f98e3-131">false</span><span class="sxs-lookup"><span data-stu-id="f98e3-131">false</span></span>  <br/> |
   

