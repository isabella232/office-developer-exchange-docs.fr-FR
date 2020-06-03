---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: L’élément SearchScope spécifie l’étendue d’une recherche.
ms.openlocfilehash: df11c8db418ac90d1166030aeed3672c0b810052
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466863"
---
# <a name="searchscope"></a><span data-ttu-id="6daec-103">SearchScope</span><span class="sxs-lookup"><span data-stu-id="6daec-103">SearchScope</span></span>

<span data-ttu-id="6daec-104">L’élément **SearchScope** spécifie l’étendue d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="6daec-104">The **SearchScope** element specifies the scope of a search.</span></span> 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 <span data-ttu-id="6daec-105">**MailboxSearchLocationType**</span><span class="sxs-lookup"><span data-stu-id="6daec-105">**MailboxSearchLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6daec-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6daec-106">Attributes and elements</span></span>

<span data-ttu-id="6daec-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6daec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6daec-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6daec-108">Attributes</span></span>

<span data-ttu-id="6daec-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6daec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6daec-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6daec-110">Child elements</span></span>

<span data-ttu-id="6daec-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6daec-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6daec-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6daec-112">Parent elements</span></span>

[<span data-ttu-id="6daec-113">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="6daec-113">MailboxSearchScope</span></span>](mailboxsearchscope.md)
  
## <a name="text-value"></a><span data-ttu-id="6daec-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="6daec-114">Text value</span></span>

<span data-ttu-id="6daec-115">La valeur de texte de l’élément **SearchScope** indique le type de boîte aux lettres qui fait l’objet d’une recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="6daec-115">The text value of the **SearchScope** element indicates the mailbox type that is searched for a discovery search.</span></span> <span data-ttu-id="6daec-116">Une valeur de texte de **PrimaryOnly** indique que la boîte aux lettres principale fait l’objet d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="6daec-116">A text value of **PrimaryOnly** indicates that the primary mailbox is searched.</span></span> <span data-ttu-id="6daec-117">Une valeur de texte de **ArchiveOnly** indique que la boîte aux lettres d’archivage est recherchée.</span><span class="sxs-lookup"><span data-stu-id="6daec-117">A text value of **ArchiveOnly** indicates that the archive mailbox is searched.</span></span> <span data-ttu-id="6daec-118">Une valeur de texte de **All** indique que la recherche s’effectue dans les boîtes aux lettres principale et d’archivage.</span><span class="sxs-lookup"><span data-stu-id="6daec-118">A text value of **All** indicates that both the primary and archive mailboxes are searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6daec-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="6daec-119">Remarks</span></span>

<span data-ttu-id="6daec-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6daec-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6daec-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6daec-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6daec-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6daec-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6daec-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6daec-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6daec-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6daec-124">Schema name</span></span>  <br/> |<span data-ttu-id="6daec-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6daec-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="6daec-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6daec-126">Validation file</span></span>  <br/> |<span data-ttu-id="6daec-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6daec-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6daec-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6daec-128">Can be empty</span></span>  <br/> ||
   

