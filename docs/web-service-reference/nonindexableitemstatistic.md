---
title: NonIndexableItemStatistic
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 593e0c79-9ec2-4040-a6a3-3c5c61cbdf7c
description: L’élément NonIndexableItemStatistic contient une statistique unique pour un élément qui ne peut pas être indexé.
ms.openlocfilehash: e604f73216aab4cca259bc6cb7eb80a2fd36cd23
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828540"
---
# <a name="nonindexableitemstatistic"></a><span data-ttu-id="a3aa7-103">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="a3aa7-103">NonIndexableItemStatistic</span></span>

<span data-ttu-id="a3aa7-104">L’élément **NonIndexableItemStatistic** contient une statistique unique pour un élément qui ne peut pas être indexé.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-104">The **NonIndexableItemStatistic** element contains a single statistic for an item that could not be indexed</span></span> 
  
```XML
<NonIndexableItemStatistic>
   <Mailbox/>
   <ItemCount/>
   <ErrorMessage/>
</NonIndexableItemStatistic>
```

 <span data-ttu-id="a3aa7-105">**NonIndexableItemStatisticType**</span><span class="sxs-lookup"><span data-stu-id="a3aa7-105">**NonIndexableItemStatisticType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3aa7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a3aa7-106">Attributes and elements</span></span>

<span data-ttu-id="a3aa7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3aa7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a3aa7-108">Attributes</span></span>

<span data-ttu-id="a3aa7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3aa7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a3aa7-110">Child elements</span></span>

<span data-ttu-id="a3aa7-111">[Boîte aux lettres (string)](mailbox-string.md) | [ItemCount](itemcount.md) | [ErrorMessage](errormessage.md)</span><span class="sxs-lookup"><span data-stu-id="a3aa7-111">[Mailbox (string)](mailbox-string.md) | [ItemCount](itemcount.md) | [ErrorMessage](errormessage.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a3aa7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a3aa7-112">Parent elements</span></span>

[<span data-ttu-id="a3aa7-113">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="a3aa7-113">NonIndexableItemStatistics</span></span>](nonindexableitemstatistics.md)
  
## <a name="remarks"></a><span data-ttu-id="a3aa7-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="a3aa7-114">Remarks</span></span>

<span data-ttu-id="a3aa7-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a3aa7-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3aa7-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a3aa7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3aa7-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a3aa7-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a3aa7-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a3aa7-119">Schema name</span></span>  <br/> |<span data-ttu-id="a3aa7-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a3aa7-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a3aa7-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a3aa7-121">Validation file</span></span>  <br/> |<span data-ttu-id="a3aa7-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a3aa7-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a3aa7-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a3aa7-123">Can be empty</span></span>  <br/> |<span data-ttu-id="a3aa7-124">False</span><span class="sxs-lookup"><span data-stu-id="a3aa7-124">False</span></span>  <br/> |
   

