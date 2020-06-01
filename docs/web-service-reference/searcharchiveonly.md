---
title: SearchArchiveOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: L’élément SearchArchiveOnly indique si seule la boîte aux lettres d’archivage est recherchée pour les éléments qui ne sont pas indexables.
ms.openlocfilehash: 9014044ed06c697cc43dd62103d7a1a907bda5a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460497"
---
# <a name="searcharchiveonly"></a><span data-ttu-id="ff8e9-103">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="ff8e9-103">SearchArchiveOnly</span></span>

<span data-ttu-id="ff8e9-104">L’élément **SearchArchiveOnly** indique si seule la boîte aux lettres d’archivage est recherchée pour les éléments qui ne sont pas indexables.</span><span class="sxs-lookup"><span data-stu-id="ff8e9-104">The **SearchArchiveOnly** element indicates whether only the archive mailbox is searched for non-indexable items.</span></span> 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 <span data-ttu-id="ff8e9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ff8e9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff8e9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ff8e9-106">Attributes and elements</span></span>

<span data-ttu-id="ff8e9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ff8e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff8e9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ff8e9-108">Attributes</span></span>

<span data-ttu-id="ff8e9-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ff8e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff8e9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ff8e9-110">Child elements</span></span>

<span data-ttu-id="ff8e9-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ff8e9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff8e9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ff8e9-112">Parent elements</span></span>

<span data-ttu-id="ff8e9-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span><span class="sxs-lookup"><span data-stu-id="ff8e9-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ff8e9-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ff8e9-114">Text value</span></span>

<span data-ttu-id="ff8e9-115">Une valeur de texte de **true** pour l’élément **SearchArchiveOnly** indique que la recherche d’élément non indexable est effectuée uniquement sur la boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="ff8e9-115">A text value of **true** for the **SearchArchiveOnly** element indicates that non-indexable item search is only performed on the archive mailbox.</span></span> <span data-ttu-id="ff8e9-116">Une valeur de texte **false** indique que la recherche est effectuée sur la boîte aux lettres principale et la boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="ff8e9-116">A text value of **false** indicates that the search is performed against the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ff8e9-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="ff8e9-117">Remarks</span></span>

<span data-ttu-id="ff8e9-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ff8e9-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ff8e9-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff8e9-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff8e9-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ff8e9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff8e9-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ff8e9-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff8e9-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ff8e9-122">Schema name</span></span>  <br/> |<span data-ttu-id="ff8e9-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ff8e9-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff8e9-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ff8e9-124">Validation file</span></span>  <br/> |<span data-ttu-id="ff8e9-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ff8e9-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff8e9-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ff8e9-126">Can be empty</span></span>  <br/> ||
   

