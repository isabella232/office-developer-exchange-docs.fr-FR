---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: L’élément DateTimePrecision spécifie la précision des valeurs de date/heure renvoyée.
ms.openlocfilehash: 4d11598628228b41adf021adbbaa77e6348534bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755802"
---
# <a name="datetimeprecision"></a><span data-ttu-id="d4201-103">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="d4201-103">DateTimePrecision</span></span>

<span data-ttu-id="d4201-104">L’élément **DateTimePrecision** spécifie la précision des valeurs de date/heure renvoyée.</span><span class="sxs-lookup"><span data-stu-id="d4201-104">The **DateTimePrecision** element specifies the precision for returned date/time values.</span></span> 
  
```XML
<DateTimePrecision />
```

<span data-ttu-id="d4201-105">**DateTimePrecisionType**</span><span class="sxs-lookup"><span data-stu-id="d4201-105">**DateTimePrecisionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d4201-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4201-106">Attributes and elements</span></span>

<span data-ttu-id="d4201-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4201-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4201-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4201-108">Attributes</span></span>

<span data-ttu-id="d4201-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="d4201-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4201-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4201-110">Child elements</span></span>

<span data-ttu-id="d4201-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4201-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4201-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4201-112">Parent elements</span></span>

<span data-ttu-id="d4201-113">L’élément **DateTimePrecision** se trouve dans l’en-tête SOAP.</span><span class="sxs-lookup"><span data-stu-id="d4201-113">The **DateTimePrecision** element is located in the SOAP header.</span></span> 
  
## <a name="text-value"></a><span data-ttu-id="d4201-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d4201-114">Text value</span></span>

<span data-ttu-id="d4201-115">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="d4201-115">A text value is required.</span></span> <span data-ttu-id="d4201-116">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="d4201-116">The following are the possible values:</span></span>
  
- <span data-ttu-id="d4201-117">Secondes</span><span class="sxs-lookup"><span data-stu-id="d4201-117">Seconds</span></span>
    
- <span data-ttu-id="d4201-118">Millisecondes</span><span class="sxs-lookup"><span data-stu-id="d4201-118">Milliseconds</span></span>
    
## <a name="remarks"></a><span data-ttu-id="d4201-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="d4201-119">Remarks</span></span>

<span data-ttu-id="d4201-120">Date/heure lorsqu’un en-tête SOAP avec l’élément **DateTimePrecision** défini sur « Secondes » est utilisé, les valeurs sont renvoyées aux plus proche secondes (00 : 00:00).</span><span class="sxs-lookup"><span data-stu-id="d4201-120">When a SOAP header with the **DateTimePrecision** element set to "Seconds" is used, date/time values are returned to the nearest seconds (00:00:00).</span></span> <span data-ttu-id="d4201-121">Date/heure lorsque « Millisecondes » sont utilisées, les valeurs sont renvoyées à la milliseconde (00:00:00.0000).</span><span class="sxs-lookup"><span data-stu-id="d4201-121">When "Milliseconds" is used, date/time values are returned to the nearest millisecond (00:00:00.0000).</span></span> 
  
<span data-ttu-id="d4201-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4201-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="d4201-123">Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="d4201-123">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4201-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4201-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4201-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4201-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4201-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4201-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d4201-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d4201-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4201-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4201-128">Validation File</span></span>  <br/> |<span data-ttu-id="d4201-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4201-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4201-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4201-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4201-131">False</span><span class="sxs-lookup"><span data-stu-id="d4201-131">False</span></span>  <br/> |
   

