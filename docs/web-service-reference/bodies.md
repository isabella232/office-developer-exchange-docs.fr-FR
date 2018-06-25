---
title: Corps
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a71a75f0-0b77-4cb9-8f9d-319de72fc1fd
description: L’élément de corps spécifie un tableau d’éléments BodyContentAttributedValue.
ms.openlocfilehash: 3316d25a567a791301c0e703a912ef28da42fa74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755406"
---
# <a name="bodies"></a><span data-ttu-id="09eb2-103">Corps</span><span class="sxs-lookup"><span data-stu-id="09eb2-103">Bodies</span></span>

<span data-ttu-id="09eb2-104">L’élément de **corps** spécifie un tableau d’éléments **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="09eb2-104">The **Bodies** element specifies an array of **BodyContentAttributedValue** elements.</span></span> 
  
```XML
<Bodies>
    <BodyContentAttributedValue></BodyContentAttributedValue>
<Bodies>
```

 <span data-ttu-id="09eb2-105">**ArrayOfBodyContentAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="09eb2-105">**ArrayOfBodyContentAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09eb2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="09eb2-106">Attributes and elements</span></span>

<span data-ttu-id="09eb2-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="09eb2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09eb2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="09eb2-108">Attributes</span></span>

<span data-ttu-id="09eb2-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="09eb2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09eb2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="09eb2-110">Child elements</span></span>

|<span data-ttu-id="09eb2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="09eb2-111">**Element**</span></span>|<span data-ttu-id="09eb2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="09eb2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09eb2-113">BodyContentAttributedValue</span><span class="sxs-lookup"><span data-stu-id="09eb2-113">BodyContentAttributedValue</span></span>](bodycontentattributedvalue.md) <br/> |<span data-ttu-id="09eb2-114">Spécifie le contenu du corps d’un élément.</span><span class="sxs-lookup"><span data-stu-id="09eb2-114">Specifies the body content of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="09eb2-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="09eb2-115">Parent elements</span></span>

|<span data-ttu-id="09eb2-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="09eb2-116">**Element**</span></span>|<span data-ttu-id="09eb2-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="09eb2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09eb2-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="09eb2-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="09eb2-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="09eb2-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="09eb2-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="09eb2-120">Remarks</span></span>

<span data-ttu-id="09eb2-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="09eb2-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="09eb2-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="09eb2-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09eb2-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="09eb2-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09eb2-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="09eb2-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="09eb2-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="09eb2-125">Schema Name</span></span>  <br/> |<span data-ttu-id="09eb2-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="09eb2-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="09eb2-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="09eb2-127">Validation File</span></span>  <br/> |<span data-ttu-id="09eb2-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="09eb2-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="09eb2-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="09eb2-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="09eb2-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="09eb2-130">See also</span></span>



- [<span data-ttu-id="09eb2-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="09eb2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

