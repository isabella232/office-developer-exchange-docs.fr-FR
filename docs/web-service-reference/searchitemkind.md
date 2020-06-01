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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463999"
---
# <a name="searchitemkind"></a><span data-ttu-id="cbdfe-103">SearchItemKind</span><span class="sxs-lookup"><span data-stu-id="cbdfe-103">SearchItemKind</span></span>

<span data-ttu-id="cbdfe-104">L’élément **SearchItemKind** indique le type d’éléments recherchés pour une opération **FindMailboxStatisticsByKeyword** .</span><span class="sxs-lookup"><span data-stu-id="cbdfe-104">The **SearchItemKind** element indicates the type of items that are searched for a **FindMailboxStatisticsByKeyword** operation.</span></span> 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 <span data-ttu-id="cbdfe-105">**SearchItemKindType**</span><span class="sxs-lookup"><span data-stu-id="cbdfe-105">**SearchItemKindType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cbdfe-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cbdfe-106">Attributes and elements</span></span>

<span data-ttu-id="cbdfe-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cbdfe-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cbdfe-108">Attributes</span></span>

<span data-ttu-id="cbdfe-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cbdfe-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cbdfe-110">Child elements</span></span>

<span data-ttu-id="cbdfe-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cbdfe-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cbdfe-112">Parent elements</span></span>

[<span data-ttu-id="cbdfe-113">MessageTypes</span><span class="sxs-lookup"><span data-stu-id="cbdfe-113">MessageTypes</span></span>](messagetypes.md)
  
## <a name="text-value"></a><span data-ttu-id="cbdfe-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="cbdfe-114">Text value</span></span>

<span data-ttu-id="cbdfe-115">La valeur de texte de l’élément **SearchItemKind** est le type d’élément qui fait l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-115">The text value of the **SearchItemKind** element is the type of item that is searched for keywords.</span></span> <span data-ttu-id="cbdfe-116">La liste suivante contient les valeurs de texte qui peuvent être utilisées dans l’élément **SearchItemKind** .</span><span class="sxs-lookup"><span data-stu-id="cbdfe-116">The following list contains the text values that can be used in the **SearchItemKind** element.</span></span> 
  
- <span data-ttu-id="cbdfe-117">**Email** : indique que les messages électroniques font l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-117">**Email** - Indicates that email messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="cbdfe-118">**Réunions** : indique que des mots clés sont recherchés dans les réunions.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-118">**Meetings** - Indicates that meetings are searched for keywords.</span></span> 
    
- <span data-ttu-id="cbdfe-119">**Tasks** : indique que les tâches font l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-119">**Tasks** - Indicates that tasks are searched for keywords.</span></span> 
    
- <span data-ttu-id="cbdfe-120">**Remarques** : indique que des mots clés sont recherchés dans les notes.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-120">**Notes** - Indicates that notes are searched for keywords.</span></span> 
    
- <span data-ttu-id="cbdfe-121">**Docs** : indique que des mots clés sont recherchés dans les documents.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-121">**Docs** - Indicates that documents are searched for keywords.</span></span> 
    
- <span data-ttu-id="cbdfe-122">**Feuilles** : indique que les journaux font l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-122">**Journals** - Indicates that journals are searched for keywords.</span></span> 
    
- <span data-ttu-id="cbdfe-123">**Contacts** : indique que des mots clés sont recherchés dans les contacts.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-123">**Contacts** - Indicates that contacts are searched for keywords.</span></span> 
    
- <span data-ttu-id="cbdfe-124">**Im** : indique que des mots clés sont recherchés dans les messages instantanés.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-124">**Im** - Indicates that instant messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="cbdfe-125">**Messagerie vocale** : indique que les messages vocaux font l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-125">**Voicemail** - Indicates that voice mails are searched for keywords.</span></span> 
    
- <span data-ttu-id="cbdfe-126">**Télécopies** : indique que des mots clés sont recherchés dans les télécopies.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-126">**Faxes** - Indicates that faxes are searched for keywords.</span></span> 
    
- <span data-ttu-id="cbdfe-127">**Publications** : indique que des mots clés sont recherchés dans les publications.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-127">**Posts** - Indicates that posts are searched for keywords.</span></span> 
    
- <span data-ttu-id="cbdfe-128">**RSSFeeds** : indique que les flux RSS font l’objet de recherches de mots clés.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-128">**Rssfeeds** - Indicates that RSS feeds are searched for keywords.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="cbdfe-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="cbdfe-129">Remarks</span></span>

<span data-ttu-id="cbdfe-130">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cbdfe-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cbdfe-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cbdfe-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cbdfe-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cbdfe-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cbdfe-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cbdfe-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cbdfe-134">Schema name</span></span>  <br/> |<span data-ttu-id="cbdfe-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cbdfe-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="cbdfe-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cbdfe-136">Validation file</span></span>  <br/> |<span data-ttu-id="cbdfe-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cbdfe-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cbdfe-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cbdfe-138">Can be empty</span></span>  <br/> ||
   

