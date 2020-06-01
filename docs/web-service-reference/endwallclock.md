---
title: EndWallClock
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc04e44e-e6d1-4355-a2b1-feb6663dc647
description: L’élément EndWallClock spécifie l’heure de fin d’une réunion dans le fuseau horaire de l’emplacement où la réunion a lieu.
ms.openlocfilehash: 48b762d0bfe367b966b6f1790230f6a2118c3fd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462970"
---
# <a name="endwallclock"></a><span data-ttu-id="f40b1-103">EndWallClock</span><span class="sxs-lookup"><span data-stu-id="f40b1-103">EndWallClock</span></span>

<span data-ttu-id="f40b1-104">L’élément **EndWallClock** spécifie l’heure de fin d’une réunion dans le fuseau horaire de l’emplacement où la réunion a lieu.</span><span class="sxs-lookup"><span data-stu-id="f40b1-104">The **EndWallClock** element specifies the end time of a meeting in the time zone of the location in which the meeting takes place.</span></span> 
  
```XML
<EndWallClock></EndWallClock>
```

 <span data-ttu-id="f40b1-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="f40b1-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f40b1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f40b1-106">Attributes and elements</span></span>

<span data-ttu-id="f40b1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f40b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f40b1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f40b1-108">Attributes</span></span>

<span data-ttu-id="f40b1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f40b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f40b1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f40b1-110">Child elements</span></span>

<span data-ttu-id="f40b1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f40b1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f40b1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f40b1-112">Parent elements</span></span>

|<span data-ttu-id="f40b1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f40b1-113">**Element**</span></span>|<span data-ttu-id="f40b1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f40b1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f40b1-115">Persona</span><span class="sxs-lookup"><span data-stu-id="f40b1-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="f40b1-116">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="f40b1-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f40b1-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f40b1-117">Text value</span></span>

<span data-ttu-id="f40b1-118">La valeur de texte de l’élément **EndWallClock** est une valeur de type String qui spécifie l’identificateur du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="f40b1-118">The text value of the **EndWallClock** element is a string value that specifies the time zone identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f40b1-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="f40b1-119">Remarks</span></span>

<span data-ttu-id="f40b1-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f40b1-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f40b1-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f40b1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f40b1-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f40b1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f40b1-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f40b1-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f40b1-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f40b1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f40b1-125">Schéma type</span><span class="sxs-lookup"><span data-stu-id="f40b1-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="f40b1-126">Validation File</span><span class="sxs-lookup"><span data-stu-id="f40b1-126">Validation File</span></span>  <br/> |<span data-ttu-id="f40b1-127">types. xsd</span><span class="sxs-lookup"><span data-stu-id="f40b1-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f40b1-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f40b1-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f40b1-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f40b1-129">See also</span></span>



- [<span data-ttu-id="f40b1-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f40b1-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

