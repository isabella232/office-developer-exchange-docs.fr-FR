---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: L’élément SearchItemKind indique le type d’éléments qui sont recherchées dans une opération FindMailboxStatisticsByKeyword.
ms.openlocfilehash: 1c099fc49ec882c1672b265ff0e3aa2c71c5f95b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829298"
---
# <a name="searchitemkind"></a><span data-ttu-id="ddadc-103">SearchItemKind</span><span class="sxs-lookup"><span data-stu-id="ddadc-103">SearchItemKind</span></span>

<span data-ttu-id="ddadc-104">L’élément **SearchItemKind** indique le type d’éléments qui sont recherchées dans une opération **FindMailboxStatisticsByKeyword** .</span><span class="sxs-lookup"><span data-stu-id="ddadc-104">The **SearchItemKind** element indicates the type of items that are searched for a **FindMailboxStatisticsByKeyword** operation.</span></span> 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 <span data-ttu-id="ddadc-105">**SearchItemKindType**</span><span class="sxs-lookup"><span data-stu-id="ddadc-105">**SearchItemKindType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ddadc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ddadc-106">Attributes and elements</span></span>

<span data-ttu-id="ddadc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ddadc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ddadc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ddadc-108">Attributes</span></span>

<span data-ttu-id="ddadc-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ddadc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ddadc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ddadc-110">Child elements</span></span>

<span data-ttu-id="ddadc-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ddadc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ddadc-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ddadc-112">Parent elements</span></span>

[<span data-ttu-id="ddadc-113">MessageTypes</span><span class="sxs-lookup"><span data-stu-id="ddadc-113">MessageTypes</span></span>](messagetypes.md)
  
## <a name="text-value"></a><span data-ttu-id="ddadc-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ddadc-114">Text value</span></span>

<span data-ttu-id="ddadc-115">La valeur de texte de l’élément **SearchItemKind** est le type d’élément dans laquelle recherche des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-115">The text value of the **SearchItemKind** element is the type of item that is searched for keywords.</span></span> <span data-ttu-id="ddadc-116">La liste suivante contient les valeurs de texte qui peuvent être utilisés dans l’élément **SearchItemKind** .</span><span class="sxs-lookup"><span data-stu-id="ddadc-116">The following list contains the text values that can be used in the **SearchItemKind** element.</span></span> 
  
- <span data-ttu-id="ddadc-117">**Courrier électronique** - indique que les messages électroniques sont exclus des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-117">**Email** - Indicates that email messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="ddadc-118">**Réunions** - indique que les réunions sont exclues des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-118">**Meetings** - Indicates that meetings are searched for keywords.</span></span> 
    
- <span data-ttu-id="ddadc-119">**Tâches** - indique que les tâches sont exclus des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-119">**Tasks** - Indicates that tasks are searched for keywords.</span></span> 
    
- <span data-ttu-id="ddadc-120">**Notes** - indique que les notes sont exclus des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-120">**Notes** - Indicates that notes are searched for keywords.</span></span> 
    
- <span data-ttu-id="ddadc-121">**Documents** - indique que les documents sont exclus des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-121">**Docs** - Indicates that documents are searched for keywords.</span></span> 
    
- <span data-ttu-id="ddadc-122">**Feuilles** - indique que les journaux sont exclus des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-122">**Journals** - Indicates that journals are searched for keywords.</span></span> 
    
- <span data-ttu-id="ddadc-123">**Contacts** - indique que les contacts sont exclus des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-123">**Contacts** - Indicates that contacts are searched for keywords.</span></span> 
    
- <span data-ttu-id="ddadc-124">**Messagerie instantanée** - indique que les messages instantanés sont exclus des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-124">**Im** - Indicates that instant messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="ddadc-125">**Messagerie vocale** - indique que les messages vocaux sont exclus des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-125">**Voicemail** - Indicates that voice mails are searched for keywords.</span></span> 
    
- <span data-ttu-id="ddadc-126">**Télécopies** - indique que les télécopies sont exclus des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-126">**Faxes** - Indicates that faxes are searched for keywords.</span></span> 
    
- <span data-ttu-id="ddadc-127">**Billets** - indique que les billets sont recherchés des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-127">**Posts** - Indicates that posts are searched for keywords.</span></span> 
    
- <span data-ttu-id="ddadc-128">**Rssfeeds** - indique que les flux RSS sont exclus des mots clés.</span><span class="sxs-lookup"><span data-stu-id="ddadc-128">**Rssfeeds** - Indicates that RSS feeds are searched for keywords.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="ddadc-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="ddadc-129">Remarks</span></span>

<span data-ttu-id="ddadc-130">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ddadc-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ddadc-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ddadc-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ddadc-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ddadc-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ddadc-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ddadc-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ddadc-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ddadc-134">Schema name</span></span>  <br/> |<span data-ttu-id="ddadc-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ddadc-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="ddadc-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ddadc-136">Validation file</span></span>  <br/> |<span data-ttu-id="ddadc-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ddadc-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ddadc-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ddadc-138">Can be empty</span></span>  <br/> ||
   

