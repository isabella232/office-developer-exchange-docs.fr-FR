---
title: MailboxStat
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: L’élément MailboxStat spécifie les statistiques d’une boîte aux lettres recherchée par la recherche de découverte.
ms.openlocfilehash: 417f63f5e1aa34c2157b1d5ad868461113afec7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44451431"
---
# <a name="mailboxstat"></a><span data-ttu-id="a6c2d-103">MailboxStat</span><span class="sxs-lookup"><span data-stu-id="a6c2d-103">MailboxStat</span></span>

<span data-ttu-id="a6c2d-104">L’élément **MailboxStat** spécifie les statistiques d’une boîte aux lettres recherchée par la recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-104">The **MailboxStat** element specifies statistics for a mailbox searched by discovery search.</span></span> 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

<span data-ttu-id="a6c2d-105">**MailboxStatisticsItemType**</span><span class="sxs-lookup"><span data-stu-id="a6c2d-105">**MailboxStatisticsItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a6c2d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a6c2d-106">Attributes and elements</span></span>

<span data-ttu-id="a6c2d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6c2d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a6c2d-108">Attributes</span></span>

<span data-ttu-id="a6c2d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a6c2d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a6c2d-110">Child elements</span></span>

<span data-ttu-id="a6c2d-111">[MailboxId](mailboxid.md)  |  [DisplayName (String)](displayname-string.md)  |  [ItemCount](itemcount.md)  |  [Taille (long)](size-long.md)</span><span class="sxs-lookup"><span data-stu-id="a6c2d-111">[MailboxId](mailboxid.md) | [DisplayName (string)](displayname-string.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a6c2d-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a6c2d-112">Parent elements</span></span>

[<span data-ttu-id="a6c2d-113">MailboxStats</span><span class="sxs-lookup"><span data-stu-id="a6c2d-113">MailboxStats</span></span>](mailboxstats.md)
  
## <a name="remarks"></a><span data-ttu-id="a6c2d-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="a6c2d-114">Remarks</span></span>

<span data-ttu-id="a6c2d-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a6c2d-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6c2d-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a6c2d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6c2d-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a6c2d-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a6c2d-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a6c2d-119">Schema name</span></span>  <br/> |<span data-ttu-id="a6c2d-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a6c2d-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="a6c2d-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a6c2d-121">Validation file</span></span>  <br/> |<span data-ttu-id="a6c2d-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a6c2d-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a6c2d-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a6c2d-123">Can be empty</span></span>  <br/> |<span data-ttu-id="a6c2d-124">false</span><span class="sxs-lookup"><span data-stu-id="a6c2d-124">false</span></span>  <br/> |
   

