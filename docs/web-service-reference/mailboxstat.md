---
title: MailboxStat
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: L’élément MailboxStat spécifie les statistiques pour une boîte aux lettres des recherches en recherche de découverte.
ms.openlocfilehash: 692f15904467ce192074b14f7c2a742b3e76de8e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828296"
---
# <a name="mailboxstat"></a><span data-ttu-id="06f10-103">MailboxStat</span><span class="sxs-lookup"><span data-stu-id="06f10-103">MailboxStat</span></span>

<span data-ttu-id="06f10-104">L’élément **MailboxStat** spécifie les statistiques pour une boîte aux lettres des recherches en recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="06f10-104">The **MailboxStat** element specifies statistics for a mailbox searched by discovery search.</span></span> 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

<span data-ttu-id="06f10-105">**MailboxStatisticsItemType**</span><span class="sxs-lookup"><span data-stu-id="06f10-105">**MailboxStatisticsItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="06f10-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="06f10-106">Attributes and elements</span></span>

<span data-ttu-id="06f10-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="06f10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06f10-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="06f10-108">Attributes</span></span>

<span data-ttu-id="06f10-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="06f10-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06f10-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="06f10-110">Child elements</span></span>

<span data-ttu-id="06f10-111">[MailboxId](mailboxid.md) | [DisplayName (string)](displayname-string.md) | [ItemCount](itemcount.md) | [taille (longue)](size-long.md)</span><span class="sxs-lookup"><span data-stu-id="06f10-111">[MailboxId](mailboxid.md) | [DisplayName (string)](displayname-string.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="06f10-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="06f10-112">Parent elements</span></span>

[<span data-ttu-id="06f10-113">MailboxStats</span><span class="sxs-lookup"><span data-stu-id="06f10-113">MailboxStats</span></span>](mailboxstats.md)
  
## <a name="remarks"></a><span data-ttu-id="06f10-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="06f10-114">Remarks</span></span>

<span data-ttu-id="06f10-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="06f10-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="06f10-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="06f10-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06f10-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="06f10-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06f10-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="06f10-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="06f10-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="06f10-119">Schema name</span></span>  <br/> |<span data-ttu-id="06f10-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="06f10-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="06f10-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="06f10-121">Validation file</span></span>  <br/> |<span data-ttu-id="06f10-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="06f10-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="06f10-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="06f10-123">Can be empty</span></span>  <br/> |<span data-ttu-id="06f10-124">false</span><span class="sxs-lookup"><span data-stu-id="06f10-124">false</span></span>  <br/> |
   

