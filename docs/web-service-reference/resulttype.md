---
title: ResultType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: L’élément ResultType contient le type de recherche à effectuer. Le type de recherche peut être statistiques uniquement ou aperçu uniquement.
ms.openlocfilehash: 6617c8b4b64cd9b6728317d7247bcc5378e488f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465281"
---
# <a name="resulttype"></a><span data-ttu-id="93198-104">ResultType</span><span class="sxs-lookup"><span data-stu-id="93198-104">ResultType</span></span>

<span data-ttu-id="93198-105">L’élément **ResultType** contient le type de recherche à effectuer.</span><span class="sxs-lookup"><span data-stu-id="93198-105">The **ResultType** element contains the type of search to perform.</span></span> <span data-ttu-id="93198-106">Le type de recherche peut être statistiques uniquement ou aperçu uniquement.</span><span class="sxs-lookup"><span data-stu-id="93198-106">The type of search can be statistics only or preview only.</span></span> 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 <span data-ttu-id="93198-107">**SearchResultType**</span><span class="sxs-lookup"><span data-stu-id="93198-107">**SearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93198-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="93198-108">Attributes and elements</span></span>

<span data-ttu-id="93198-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="93198-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93198-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="93198-110">Attributes</span></span>

<span data-ttu-id="93198-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="93198-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93198-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="93198-112">Child elements</span></span>

<span data-ttu-id="93198-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="93198-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93198-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="93198-114">Parent elements</span></span>

<span data-ttu-id="93198-115">[SearchMailboxesResult](searchmailboxesresult.md)  |  [SearchMailboxes](searchmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="93198-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="93198-116">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="93198-116">Text value</span></span>

<span data-ttu-id="93198-117">La valeur de texte de l’élément **ResultType** est le type de résultat renvoyé pour une recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="93198-117">The text value of the **ResultType** element is the type of result that is returned for a discovery search.</span></span> <span data-ttu-id="93198-118">Une valeur de texte de **StatisticsOnly** renverra les statistiques de la recherche.</span><span class="sxs-lookup"><span data-stu-id="93198-118">A text value of **StatisticsOnly** will return the search statistics.</span></span> <span data-ttu-id="93198-119">Une valeur de texte de **PreviewOnly** renverra des informations d’aperçu d’élément.</span><span class="sxs-lookup"><span data-stu-id="93198-119">A text value of **PreviewOnly** will return item preview information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="93198-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="93198-120">Remarks</span></span>

<span data-ttu-id="93198-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="93198-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="93198-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="93198-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93198-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="93198-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93198-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="93198-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93198-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="93198-125">Schema name</span></span>  <br/> |<span data-ttu-id="93198-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="93198-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="93198-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="93198-127">Validation file</span></span>  <br/> |<span data-ttu-id="93198-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="93198-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93198-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="93198-129">Can be empty</span></span>  <br/> |<span data-ttu-id="93198-130">false</span><span class="sxs-lookup"><span data-stu-id="93198-130">false</span></span>  <br/> |
   

