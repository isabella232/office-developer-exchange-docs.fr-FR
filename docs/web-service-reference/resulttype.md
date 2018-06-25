---
title: ResultType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: L’élément ResultType contient le type de recherche à effectuer. Le type de recherche peut être statistiques uniquement ou afficher un aperçu uniquement.
ms.openlocfilehash: 750f53ae05a7ad9f5aefc9396911a23ef32cdfc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829211"
---
# <a name="resulttype"></a><span data-ttu-id="aa90c-104">ResultType</span><span class="sxs-lookup"><span data-stu-id="aa90c-104">ResultType</span></span>

<span data-ttu-id="aa90c-105">L’élément **ResultType** contient le type de recherche à effectuer.</span><span class="sxs-lookup"><span data-stu-id="aa90c-105">The **ResultType** element contains the type of search to perform.</span></span> <span data-ttu-id="aa90c-106">Le type de recherche peut être statistiques uniquement ou afficher un aperçu uniquement.</span><span class="sxs-lookup"><span data-stu-id="aa90c-106">The type of search can be statistics only or preview only.</span></span> 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 <span data-ttu-id="aa90c-107">**SearchResultType**</span><span class="sxs-lookup"><span data-stu-id="aa90c-107">**SearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa90c-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aa90c-108">Attributes and elements</span></span>

<span data-ttu-id="aa90c-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aa90c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa90c-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="aa90c-110">Attributes</span></span>

<span data-ttu-id="aa90c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aa90c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa90c-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aa90c-112">Child elements</span></span>

<span data-ttu-id="aa90c-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aa90c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aa90c-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aa90c-114">Parent elements</span></span>

<span data-ttu-id="aa90c-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="aa90c-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="aa90c-116">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="aa90c-116">Text value</span></span>

<span data-ttu-id="aa90c-117">La valeur de texte de l’élément **ResultType** est le type de résultat qui est renvoyé pour une recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="aa90c-117">The text value of the **ResultType** element is the type of result that is returned for a discovery search.</span></span> <span data-ttu-id="aa90c-118">Valeur texte **StatisticsOnly** renvoie les statistiques de la recherche.</span><span class="sxs-lookup"><span data-stu-id="aa90c-118">A text value of **StatisticsOnly** will return the search statistics.</span></span> <span data-ttu-id="aa90c-119">Valeur texte **PreviewOnly** retourne des informations d’Aperçu d’élément.</span><span class="sxs-lookup"><span data-stu-id="aa90c-119">A text value of **PreviewOnly** will return item preview information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="aa90c-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="aa90c-120">Remarks</span></span>

<span data-ttu-id="aa90c-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="aa90c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aa90c-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa90c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa90c-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aa90c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa90c-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aa90c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aa90c-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aa90c-125">Schema name</span></span>  <br/> |<span data-ttu-id="aa90c-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="aa90c-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aa90c-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="aa90c-127">Validation file</span></span>  <br/> |<span data-ttu-id="aa90c-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aa90c-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa90c-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aa90c-129">Can be empty</span></span>  <br/> |<span data-ttu-id="aa90c-130">false</span><span class="sxs-lookup"><span data-stu-id="aa90c-130">false</span></span>  <br/> |
   

