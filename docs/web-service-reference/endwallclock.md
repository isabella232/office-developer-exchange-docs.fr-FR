---
title: EndWallClock
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc04e44e-e6d1-4355-a2b1-feb6663dc647
description: L’élément EndWallClock Spécifie l’heure de fin d’une réunion dans le fuseau horaire de l’emplacement dans lequel la réunion a lieu.
ms.openlocfilehash: 10e4a2bde50354b2f2752751c01a6a70aa084d05
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756182"
---
# <a name="endwallclock"></a><span data-ttu-id="e610c-103">EndWallClock</span><span class="sxs-lookup"><span data-stu-id="e610c-103">EndWallClock</span></span>

<span data-ttu-id="e610c-104">L’élément **EndWallClock** Spécifie l’heure de fin d’une réunion dans le fuseau horaire de l’emplacement dans lequel la réunion a lieu.</span><span class="sxs-lookup"><span data-stu-id="e610c-104">The **EndWallClock** element specifies the end time of a meeting in the time zone of the location in which the meeting takes place.</span></span> 
  
```XML
<EndWallClock></EndWallClock>
```

 <span data-ttu-id="e610c-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="e610c-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e610c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e610c-106">Attributes and elements</span></span>

<span data-ttu-id="e610c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e610c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e610c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e610c-108">Attributes</span></span>

<span data-ttu-id="e610c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e610c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e610c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e610c-110">Child elements</span></span>

<span data-ttu-id="e610c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e610c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e610c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e610c-112">Parent elements</span></span>

|<span data-ttu-id="e610c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e610c-113">**Element**</span></span>|<span data-ttu-id="e610c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="e610c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e610c-115">Personnage</span><span class="sxs-lookup"><span data-stu-id="e610c-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="e610c-116">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="e610c-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e610c-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e610c-117">Text value</span></span>

<span data-ttu-id="e610c-118">La valeur de texte de l’élément **EndWallClock** est une valeur de type string qui spécifie l’identificateur de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e610c-118">The text value of the **EndWallClock** element is a string value that specifies the time zone identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e610c-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="e610c-119">Remarks</span></span>

<span data-ttu-id="e610c-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e610c-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e610c-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e610c-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e610c-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e610c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e610c-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e610c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e610c-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e610c-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e610c-125">Schéma type</span><span class="sxs-lookup"><span data-stu-id="e610c-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="e610c-126">Validation File</span><span class="sxs-lookup"><span data-stu-id="e610c-126">Validation File</span></span>  <br/> |<span data-ttu-id="e610c-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="e610c-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e610c-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e610c-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e610c-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e610c-129">See also</span></span>



- [<span data-ttu-id="e610c-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e610c-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

