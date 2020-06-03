---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: L’élément DateTimePrecision spécifie la précision pour les valeurs de date/heure renvoyées.
ms.openlocfilehash: 9d245dfb0123daae42ba9b9b4e98aff872b67d80
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529223"
---
# <a name="datetimeprecision"></a><span data-ttu-id="6268e-103">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="6268e-103">DateTimePrecision</span></span>

<span data-ttu-id="6268e-104">L’élément **DateTimePrecision** spécifie la précision pour les valeurs de date/heure renvoyées.</span><span class="sxs-lookup"><span data-stu-id="6268e-104">The **DateTimePrecision** element specifies the precision for returned date/time values.</span></span> 
  
```XML
<DateTimePrecision />
```

<span data-ttu-id="6268e-105">**DateTimePrecisionType**</span><span class="sxs-lookup"><span data-stu-id="6268e-105">**DateTimePrecisionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6268e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6268e-106">Attributes and elements</span></span>

<span data-ttu-id="6268e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6268e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6268e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6268e-108">Attributes</span></span>

<span data-ttu-id="6268e-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="6268e-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6268e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6268e-110">Child elements</span></span>

<span data-ttu-id="6268e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6268e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6268e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6268e-112">Parent elements</span></span>

<span data-ttu-id="6268e-113">L’élément **DateTimePrecision** se trouve dans l’en-tête SOAP.</span><span class="sxs-lookup"><span data-stu-id="6268e-113">The **DateTimePrecision** element is located in the SOAP header.</span></span> 
  
## <a name="text-value"></a><span data-ttu-id="6268e-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="6268e-114">Text value</span></span>

<span data-ttu-id="6268e-115">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="6268e-115">A text value is required.</span></span> <span data-ttu-id="6268e-116">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="6268e-116">The following are the possible values:</span></span>
  
- <span data-ttu-id="6268e-117">Secondes</span><span class="sxs-lookup"><span data-stu-id="6268e-117">Seconds</span></span>
    
- <span data-ttu-id="6268e-118">Millisecondes</span><span class="sxs-lookup"><span data-stu-id="6268e-118">Milliseconds</span></span>
    
## <a name="remarks"></a><span data-ttu-id="6268e-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="6268e-119">Remarks</span></span>

<span data-ttu-id="6268e-120">Lorsqu’un en-tête SOAP avec l’élément **DateTimePrecision** défini sur « seconds » est utilisé, les valeurs de date/heure sont renvoyées aux secondes les plus proches (00:00:00).</span><span class="sxs-lookup"><span data-stu-id="6268e-120">When a SOAP header with the **DateTimePrecision** element set to "Seconds" is used, date/time values are returned to the nearest seconds (00:00:00).</span></span> <span data-ttu-id="6268e-121">Lorsque « millisecondes » est utilisé, les valeurs de date/heure sont renvoyées à la milliseconde près (00:00:00.0000).</span><span class="sxs-lookup"><span data-stu-id="6268e-121">When "Milliseconds" is used, date/time values are returned to the nearest millisecond (00:00:00.0000).</span></span> 
  
<span data-ttu-id="6268e-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6268e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="6268e-123">Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="6268e-123">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6268e-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6268e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6268e-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6268e-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6268e-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6268e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="6268e-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6268e-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="6268e-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6268e-128">Validation File</span></span>  <br/> |<span data-ttu-id="6268e-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6268e-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6268e-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6268e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="6268e-131">False</span><span class="sxs-lookup"><span data-stu-id="6268e-131">False</span></span>  <br/> |
   

