---
title: Présentateurs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: L’élément Presenters spécifie les présentateurs d’une réunion en ligne.
ms.openlocfilehash: 0236457020dfc4684569e84d3d54e357af00d102
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529909"
---
# <a name="presenters"></a><span data-ttu-id="41b1b-103">Présentateurs</span><span class="sxs-lookup"><span data-stu-id="41b1b-103">Presenters</span></span>

<span data-ttu-id="41b1b-104">L’élément **Presenters** spécifie les présentateurs d’une réunion en ligne.</span><span class="sxs-lookup"><span data-stu-id="41b1b-104">The **Presenters** element specifies the presenters for an online meeting.</span></span> 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 <span data-ttu-id="41b1b-105">**PresentersType**</span><span class="sxs-lookup"><span data-stu-id="41b1b-105">**PresentersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41b1b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="41b1b-106">Attributes and elements</span></span>

<span data-ttu-id="41b1b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="41b1b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41b1b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="41b1b-108">Attributes</span></span>

<span data-ttu-id="41b1b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="41b1b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41b1b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="41b1b-110">Child elements</span></span>

<span data-ttu-id="41b1b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="41b1b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="41b1b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="41b1b-112">Parent elements</span></span>

[<span data-ttu-id="41b1b-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="41b1b-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="41b1b-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="41b1b-114">Text value</span></span>

<span data-ttu-id="41b1b-115">La valeur de texte de l’élément **Presenters** est le type d’utilisateurs pouvant être présentateur pour une réunion en ligne.</span><span class="sxs-lookup"><span data-stu-id="41b1b-115">The text value of **Presenters** element is the type of users that can be a presenter for an online meeting.</span></span> <span data-ttu-id="41b1b-116">Les valeurs de texte de l’élément **Presenters** sont décrites dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="41b1b-116">The text values for the **Presenters** element are described in the following table.</span></span> 
  
<span data-ttu-id="41b1b-117">**Valeurs de texte de l’élément Presenters**</span><span class="sxs-lookup"><span data-stu-id="41b1b-117">**Presenters element text values**</span></span>

|<span data-ttu-id="41b1b-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="41b1b-118">**Value**</span></span>|<span data-ttu-id="41b1b-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="41b1b-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="41b1b-120">Désactivé</span><span class="sxs-lookup"><span data-stu-id="41b1b-120">Disabled</span></span>  <br/> |<span data-ttu-id="41b1b-121">Les présentateurs sont désactivés.</span><span class="sxs-lookup"><span data-stu-id="41b1b-121">Presenters are disabled.</span></span>  <br/> |
|<span data-ttu-id="41b1b-122">Interne</span><span class="sxs-lookup"><span data-stu-id="41b1b-122">Internal</span></span>  <br/> |<span data-ttu-id="41b1b-123">Seuls les participants internes peuvent être présentateurs.</span><span class="sxs-lookup"><span data-stu-id="41b1b-123">Only internal participants can be presenters.</span></span>  <br/> |
|<span data-ttu-id="41b1b-124">Tout le monde</span><span class="sxs-lookup"><span data-stu-id="41b1b-124">Everyone</span></span>  <br/> |<span data-ttu-id="41b1b-125">Tout participant peut être présentateur.</span><span class="sxs-lookup"><span data-stu-id="41b1b-125">Any participant can be a presenter.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="41b1b-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="41b1b-126">Remarks</span></span>

<span data-ttu-id="41b1b-127">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="41b1b-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="41b1b-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="41b1b-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41b1b-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="41b1b-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41b1b-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="41b1b-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41b1b-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="41b1b-131">Schema name</span></span>  <br/> |<span data-ttu-id="41b1b-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="41b1b-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="41b1b-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="41b1b-133">Validation file</span></span>  <br/> |<span data-ttu-id="41b1b-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="41b1b-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="41b1b-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="41b1b-135">Can be empty</span></span>  <br/> ||
   

