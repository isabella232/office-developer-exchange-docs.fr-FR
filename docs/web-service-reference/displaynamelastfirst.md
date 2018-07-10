---
title: DisplayNameLastFirst
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d392e138-a514-4bce-81b1-1f484e353d1c
description: L’élément DisplayNameLastFirst Spécifie le nom complet du personnage associé dans le format, nom de famille, prénom.
ms.openlocfilehash: 68ebf0e91e216cffa1ba8db425de248f0d4e77b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756009"
---
# <a name="displaynamelastfirst"></a><span data-ttu-id="c4f45-103">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="c4f45-103">DisplayNameLastFirst</span></span>

<span data-ttu-id="c4f45-104">L’élément **DisplayNameLastFirst** Spécifie le nom complet du personnage associé au format « Nom », « Prénom ».</span><span class="sxs-lookup"><span data-stu-id="c4f45-104">The **DisplayNameLastFirst** element specifies the display name of the associated persona in the format, "Last Name", "First Name".</span></span> 
  
```XML
<DisplayNameLastFirst></DisplayNameLastFirst>
```

 <span data-ttu-id="c4f45-105">**string**</span><span class="sxs-lookup"><span data-stu-id="c4f45-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4f45-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c4f45-106">Attributes and elements</span></span>

<span data-ttu-id="c4f45-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c4f45-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4f45-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c4f45-108">Attributes</span></span>

<span data-ttu-id="c4f45-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c4f45-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4f45-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c4f45-110">Child elements</span></span>

<span data-ttu-id="c4f45-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c4f45-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c4f45-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c4f45-112">Parent elements</span></span>

|<span data-ttu-id="c4f45-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c4f45-113">**Element**</span></span>|<span data-ttu-id="c4f45-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="c4f45-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4f45-115">Personnage</span><span class="sxs-lookup"><span data-stu-id="c4f45-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="c4f45-116">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="c4f45-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c4f45-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c4f45-117">Text value</span></span>

<span data-ttu-id="c4f45-118">La valeur de texte de l’élément **DisplayNameLastFirst** est une valeur de type string qui spécifie le nom complet, avec le nom de famille tout d’abord.</span><span class="sxs-lookup"><span data-stu-id="c4f45-118">The text value of the **DisplayNameLastFirst** element is a string value that specifies the display name, with the surname first.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c4f45-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="c4f45-119">Remarks</span></span>

<span data-ttu-id="c4f45-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c4f45-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c4f45-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4f45-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4f45-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c4f45-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4f45-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c4f45-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c4f45-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c4f45-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c4f45-125">Schéma type</span><span class="sxs-lookup"><span data-stu-id="c4f45-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="c4f45-126">Validation File</span><span class="sxs-lookup"><span data-stu-id="c4f45-126">Validation File</span></span>  <br/> |<span data-ttu-id="c4f45-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="c4f45-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c4f45-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c4f45-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c4f45-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c4f45-129">See also</span></span>

- [<span data-ttu-id="c4f45-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c4f45-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
