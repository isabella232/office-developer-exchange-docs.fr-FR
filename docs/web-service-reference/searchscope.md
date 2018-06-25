---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: L’élément SearchScope Spécifie l’étendue d’une recherche.
ms.openlocfilehash: 352292952c735e7d3893790a660096c6b6966536
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829315"
---
# <a name="searchscope"></a><span data-ttu-id="d461f-103">SearchScope</span><span class="sxs-lookup"><span data-stu-id="d461f-103">SearchScope</span></span>

<span data-ttu-id="d461f-104">L’élément **SearchScope** Spécifie l’étendue d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="d461f-104">The **SearchScope** element specifies the scope of a search.</span></span> 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 <span data-ttu-id="d461f-105">**MailboxSearchLocationType**</span><span class="sxs-lookup"><span data-stu-id="d461f-105">**MailboxSearchLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d461f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d461f-106">Attributes and elements</span></span>

<span data-ttu-id="d461f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d461f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d461f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d461f-108">Attributes</span></span>

<span data-ttu-id="d461f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d461f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d461f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d461f-110">Child elements</span></span>

<span data-ttu-id="d461f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d461f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d461f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d461f-112">Parent elements</span></span>

[<span data-ttu-id="d461f-113">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="d461f-113">MailboxSearchScope</span></span>](mailboxsearchscope.md)
  
## <a name="text-value"></a><span data-ttu-id="d461f-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d461f-114">Text value</span></span>

<span data-ttu-id="d461f-115">La valeur de texte de l’élément **SearchScope** indique le type de boîte aux lettres qui est recherché dans une recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="d461f-115">The text value of the **SearchScope** element indicates the mailbox type that is searched for a discovery search.</span></span> <span data-ttu-id="d461f-116">Une valeur texte **PrimaryOnly** indique que la boîte aux lettres principale est recherché.</span><span class="sxs-lookup"><span data-stu-id="d461f-116">A text value of **PrimaryOnly** indicates that the primary mailbox is searched.</span></span> <span data-ttu-id="d461f-117">Une valeur texte **ArchiveOnly** indique que la boîte aux lettres d’archive est recherché.</span><span class="sxs-lookup"><span data-stu-id="d461f-117">A text value of **ArchiveOnly** indicates that the archive mailbox is searched.</span></span> <span data-ttu-id="d461f-118">Une valeur de texte de **toutes les** indique que les deux principales et de boîtes aux lettres d’archivage sont recherchés.</span><span class="sxs-lookup"><span data-stu-id="d461f-118">A text value of **All** indicates that both the primary and archive mailboxes are searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d461f-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="d461f-119">Remarks</span></span>

<span data-ttu-id="d461f-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d461f-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d461f-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d461f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d461f-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d461f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d461f-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d461f-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d461f-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d461f-124">Schema name</span></span>  <br/> |<span data-ttu-id="d461f-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d461f-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="d461f-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d461f-126">Validation file</span></span>  <br/> |<span data-ttu-id="d461f-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d461f-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d461f-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d461f-128">Can be empty</span></span>  <br/> ||
   

