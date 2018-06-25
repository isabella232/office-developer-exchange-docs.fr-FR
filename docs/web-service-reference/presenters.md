---
title: Présentateurs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: L’élément de présentateurs spécifie les présentateurs pour une réunion en ligne.
ms.openlocfilehash: f62b458759e0d8199c98827602d6c3fe16aebeea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828875"
---
# <a name="presenters"></a><span data-ttu-id="6d1aa-103">Présentateurs</span><span class="sxs-lookup"><span data-stu-id="6d1aa-103">Presenters</span></span>

<span data-ttu-id="6d1aa-104">L’élément de **Présentateurs** spécifie les présentateurs pour une réunion en ligne.</span><span class="sxs-lookup"><span data-stu-id="6d1aa-104">The **Presenters** element specifies the presenters for an online meeting.</span></span> 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 <span data-ttu-id="6d1aa-105">**PresentersType**</span><span class="sxs-lookup"><span data-stu-id="6d1aa-105">**PresentersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d1aa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6d1aa-106">Attributes and elements</span></span>

<span data-ttu-id="6d1aa-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6d1aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d1aa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6d1aa-108">Attributes</span></span>

<span data-ttu-id="6d1aa-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6d1aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d1aa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6d1aa-110">Child elements</span></span>

<span data-ttu-id="6d1aa-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6d1aa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d1aa-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6d1aa-112">Parent elements</span></span>

[<span data-ttu-id="6d1aa-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="6d1aa-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="6d1aa-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6d1aa-114">Text value</span></span>

<span data-ttu-id="6d1aa-115">La valeur de texte d’élément de **Présentateurs** est le type d’utilisateurs qui peut être un présentateur pour une réunion en ligne.</span><span class="sxs-lookup"><span data-stu-id="6d1aa-115">The text value of **Presenters** element is the type of users that can be a presenter for an online meeting.</span></span> <span data-ttu-id="6d1aa-116">Les valeurs de texte de l’élément **Présentateurs** sont décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="6d1aa-116">The text values for the **Presenters** element are described in the following table.</span></span> 
  
<span data-ttu-id="6d1aa-117">**Valeurs de texte des éléments présentateurs**</span><span class="sxs-lookup"><span data-stu-id="6d1aa-117">**Presenters element text values**</span></span>

|<span data-ttu-id="6d1aa-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="6d1aa-118">**Value**</span></span>|<span data-ttu-id="6d1aa-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="6d1aa-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6d1aa-120">Désactivé</span><span class="sxs-lookup"><span data-stu-id="6d1aa-120">Disabled</span></span>  <br/> |<span data-ttu-id="6d1aa-121">Les présentateurs sont désactivées.</span><span class="sxs-lookup"><span data-stu-id="6d1aa-121">Presenters are disabled.</span></span>  <br/> |
|<span data-ttu-id="6d1aa-122">Interne</span><span class="sxs-lookup"><span data-stu-id="6d1aa-122">Internal</span></span>  <br/> |<span data-ttu-id="6d1aa-123">Seuls les participants internes peuvent être présentateurs.</span><span class="sxs-lookup"><span data-stu-id="6d1aa-123">Only internal participants can be presenters.</span></span>  <br/> |
|<span data-ttu-id="6d1aa-124">Tout le monde</span><span class="sxs-lookup"><span data-stu-id="6d1aa-124">Everyone</span></span>  <br/> |<span data-ttu-id="6d1aa-125">N’importe quel participant peut être un présentateur.</span><span class="sxs-lookup"><span data-stu-id="6d1aa-125">Any participant can be a presenter.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6d1aa-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="6d1aa-126">Remarks</span></span>

<span data-ttu-id="6d1aa-127">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6d1aa-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6d1aa-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d1aa-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d1aa-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6d1aa-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d1aa-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6d1aa-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d1aa-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6d1aa-131">Schema name</span></span>  <br/> |<span data-ttu-id="6d1aa-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6d1aa-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="6d1aa-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6d1aa-133">Validation file</span></span>  <br/> |<span data-ttu-id="6d1aa-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6d1aa-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d1aa-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6d1aa-135">Can be empty</span></span>  <br/> ||
   

