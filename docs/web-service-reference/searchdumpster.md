---
title: SearchDumpster
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb62dce-c87a-4714-8023-a6b697a29699
description: L’élément SearchDumpster Spécifie s’il faut rechercher dans la benne de Exchange.
ms.openlocfilehash: 4a40ee2da7fdaa4eaa3f5349545a0bfd3e13ba73
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829283"
---
# <a name="searchdumpster"></a><span data-ttu-id="d55e4-103">SearchDumpster</span><span class="sxs-lookup"><span data-stu-id="d55e4-103">SearchDumpster</span></span>

<span data-ttu-id="d55e4-104">L’élément **SearchDumpster** Spécifie s’il faut rechercher dans la benne de Exchange.</span><span class="sxs-lookup"><span data-stu-id="d55e4-104">The **SearchDumpster** element specifies whether to search in the Exchange Dumpster.</span></span> 
  
```XML
<SearchDumpster> true | false </SearchDumpster>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="d55e4-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d55e4-105">Attributes and elements</span></span>

<span data-ttu-id="d55e4-106">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d55e4-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d55e4-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="d55e4-107">Attributes</span></span>

<span data-ttu-id="d55e4-108">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d55e4-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d55e4-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d55e4-109">Child elements</span></span>

<span data-ttu-id="d55e4-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d55e4-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d55e4-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d55e4-111">Parent elements</span></span>

[<span data-ttu-id="d55e4-112">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="d55e4-112">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md)
  
## <a name="text-value"></a><span data-ttu-id="d55e4-113">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d55e4-113">Text value</span></span>

<span data-ttu-id="d55e4-114">Une valeur de texte de **la valeur true** pour l’élément **SearchDumpster** indique que la recherche de statistiques de boîtes aux lettres inclut la benne Exchange.</span><span class="sxs-lookup"><span data-stu-id="d55e4-114">A text value of **true** for the **SearchDumpster** element indicates that the mailbox statistics search includes the Exchange Dumpster.</span></span> <span data-ttu-id="d55e4-115">La valeur **false** indique que la benne Exchange n’est pas recherchée.</span><span class="sxs-lookup"><span data-stu-id="d55e4-115">A value of **false** indicates that the Exchange Dumpster is not searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d55e4-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="d55e4-116">Remarks</span></span>

<span data-ttu-id="d55e4-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d55e4-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d55e4-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d55e4-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d55e4-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d55e4-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d55e4-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d55e4-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d55e4-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d55e4-121">Schema name</span></span>  <br/> |<span data-ttu-id="d55e4-122">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d55e4-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="d55e4-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d55e4-123">Validation file</span></span>  <br/> |<span data-ttu-id="d55e4-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d55e4-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d55e4-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d55e4-125">Can be empty</span></span>  <br/> ||
   

