---
title: SearchDumpster
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb62dce-c87a-4714-8023-a6b697a29699
description: L’élément SearchDumpster spécifie s’il faut effectuer une recherche dans la benne Exchange.
ms.openlocfilehash: 067bf8ea3e589aa392c6b8ba6d4dc10b430c1f28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460490"
---
# <a name="searchdumpster"></a><span data-ttu-id="4b11d-103">SearchDumpster</span><span class="sxs-lookup"><span data-stu-id="4b11d-103">SearchDumpster</span></span>

<span data-ttu-id="4b11d-104">L’élément **SearchDumpster** spécifie s’il faut effectuer une recherche dans la benne Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b11d-104">The **SearchDumpster** element specifies whether to search in the Exchange Dumpster.</span></span> 
  
```XML
<SearchDumpster> true | false </SearchDumpster>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="4b11d-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4b11d-105">Attributes and elements</span></span>

<span data-ttu-id="4b11d-106">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4b11d-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b11d-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="4b11d-107">Attributes</span></span>

<span data-ttu-id="4b11d-108">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4b11d-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b11d-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4b11d-109">Child elements</span></span>

<span data-ttu-id="4b11d-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4b11d-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4b11d-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4b11d-111">Parent elements</span></span>

[<span data-ttu-id="4b11d-112">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="4b11d-112">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md)
  
## <a name="text-value"></a><span data-ttu-id="4b11d-113">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4b11d-113">Text value</span></span>

<span data-ttu-id="4b11d-114">Une valeur de texte de **true** pour l’élément **SearchDumpster** indique que la recherche de statistiques de boîte aux lettres inclut la benne Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b11d-114">A text value of **true** for the **SearchDumpster** element indicates that the mailbox statistics search includes the Exchange Dumpster.</span></span> <span data-ttu-id="4b11d-115">La valeur **false** indique que la benne Exchange n’est pas recherchée.</span><span class="sxs-lookup"><span data-stu-id="4b11d-115">A value of **false** indicates that the Exchange Dumpster is not searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4b11d-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="4b11d-116">Remarks</span></span>

<span data-ttu-id="4b11d-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4b11d-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4b11d-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b11d-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b11d-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4b11d-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b11d-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4b11d-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4b11d-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4b11d-121">Schema name</span></span>  <br/> |<span data-ttu-id="4b11d-122">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4b11d-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="4b11d-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4b11d-123">Validation file</span></span>  <br/> |<span data-ttu-id="4b11d-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4b11d-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4b11d-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4b11d-125">Can be empty</span></span>  <br/> ||
   

