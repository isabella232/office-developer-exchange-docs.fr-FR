---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: L’élément SearchItemKind indique le type d’éléments recherchés pour une opération FindMailboxStatisticsByKeyword.
ms.openlocfilehash: e0625ac169c3083702494c094da15d38d220fe67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463999"
---
# <a name="searchitemkind"></a><span data-ttu-id="1b292-103">SearchItemKind</span><span class="sxs-lookup"><span data-stu-id="1b292-103">SearchItemKind</span></span>

<span data-ttu-id="1b292-104">L’élément **SearchItemKind** indique le type d’éléments recherchés pour une opération **FindMailboxStatisticsByKeyword** .</span><span class="sxs-lookup"><span data-stu-id="1b292-104">The **SearchItemKind** element indicates the type of items that are searched for a **FindMailboxStatisticsByKeyword** operation.</span></span> 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 <span data-ttu-id="1b292-105">**SearchItemKindType**</span><span class="sxs-lookup"><span data-stu-id="1b292-105">**SearchItemKindType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b292-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1b292-106">Attributes and elements</span></span>

<span data-ttu-id="1b292-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1b292-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b292-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1b292-108">Attributes</span></span>

<span data-ttu-id="1b292-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1b292-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b292-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1b292-110">Child elements</span></span>

<span data-ttu-id="1b292-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1b292-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1b292-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1b292-112">Parent elements</span></span>

[<span data-ttu-id="1b292-113">MessageTypes</span><span class="sxs-lookup"><span data-stu-id="1b292-113">MessageTypes</span></span>](messagetypes.md)
  
## <a name="text-value"></a><span data-ttu-id="1b292-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="1b292-114">Text value</span></span>

<span data-ttu-id="1b292-115">La valeur de texte de l’élément **SearchItemKind** est le type d’élément qui fait l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="1b292-115">The text value of the **SearchItemKind** element is the type of item that is searched for keywords.</span></span> <span data-ttu-id="1b292-116">La liste suivante contient les valeurs de texte qui peuvent être utilisées dans l’élément **SearchItemKind** .</span><span class="sxs-lookup"><span data-stu-id="1b292-116">The following list contains the text values that can be used in the **SearchItemKind** element.</span></span> 
  
- <span data-ttu-id="1b292-117">**Email** : indique que les messages électroniques font l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="1b292-117">**Email** - Indicates that email messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="1b292-118">**Réunions** : indique que des mots clés sont recherchés dans les réunions.</span><span class="sxs-lookup"><span data-stu-id="1b292-118">**Meetings** - Indicates that meetings are searched for keywords.</span></span> 
    
- <span data-ttu-id="1b292-119">**Tasks** : indique que les tâches font l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="1b292-119">**Tasks** - Indicates that tasks are searched for keywords.</span></span> 
    
- <span data-ttu-id="1b292-120">**Remarques** : indique que des mots clés sont recherchés dans les notes.</span><span class="sxs-lookup"><span data-stu-id="1b292-120">**Notes** - Indicates that notes are searched for keywords.</span></span> 
    
- <span data-ttu-id="1b292-121">**Docs** : indique que des mots clés sont recherchés dans les documents.</span><span class="sxs-lookup"><span data-stu-id="1b292-121">**Docs** - Indicates that documents are searched for keywords.</span></span> 
    
- <span data-ttu-id="1b292-122">**Feuilles** : indique que les journaux font l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="1b292-122">**Journals** - Indicates that journals are searched for keywords.</span></span> 
    
- <span data-ttu-id="1b292-123">**Contacts** : indique que des mots clés sont recherchés dans les contacts.</span><span class="sxs-lookup"><span data-stu-id="1b292-123">**Contacts** - Indicates that contacts are searched for keywords.</span></span> 
    
- <span data-ttu-id="1b292-124">**Im** : indique que des mots clés sont recherchés dans les messages instantanés.</span><span class="sxs-lookup"><span data-stu-id="1b292-124">**Im** - Indicates that instant messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="1b292-125">**Messagerie vocale** : indique que les messages vocaux font l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="1b292-125">**Voicemail** - Indicates that voice mails are searched for keywords.</span></span> 
    
- <span data-ttu-id="1b292-126">**Télécopies** : indique que des mots clés sont recherchés dans les télécopies.</span><span class="sxs-lookup"><span data-stu-id="1b292-126">**Faxes** - Indicates that faxes are searched for keywords.</span></span> 
    
- <span data-ttu-id="1b292-127">**Publications** : indique que des mots clés sont recherchés dans les publications.</span><span class="sxs-lookup"><span data-stu-id="1b292-127">**Posts** - Indicates that posts are searched for keywords.</span></span> 
    
- <span data-ttu-id="1b292-128">**RSSFeeds** : indique que les flux RSS font l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="1b292-128">**Rssfeeds** - Indicates that RSS feeds are searched for keywords.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="1b292-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="1b292-129">Remarks</span></span>

<span data-ttu-id="1b292-130">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1b292-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1b292-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b292-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b292-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1b292-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b292-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1b292-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1b292-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1b292-134">Schema name</span></span>  <br/> |<span data-ttu-id="1b292-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1b292-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="1b292-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1b292-136">Validation file</span></span>  <br/> |<span data-ttu-id="1b292-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1b292-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1b292-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1b292-138">Can be empty</span></span>  <br/> ||
   

