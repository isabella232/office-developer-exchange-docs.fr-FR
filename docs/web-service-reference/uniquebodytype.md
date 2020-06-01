---
title: UniqueBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f7276aa-e354-40e4-b9cb-950fad46ac93
description: L’élément UniqueBodyType spécifie si le corps unique est renvoyé au format texte ou HTML.
ms.openlocfilehash: 7e6c4631ef589555ce4d5da747c200ffe956f3a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459439"
---
# <a name="uniquebodytype"></a><span data-ttu-id="112a8-103">UniqueBodyType</span><span class="sxs-lookup"><span data-stu-id="112a8-103">UniqueBodyType</span></span>

<span data-ttu-id="112a8-104">L’élément **UniqueBodyType** spécifie si le corps unique est renvoyé au format texte ou html.</span><span class="sxs-lookup"><span data-stu-id="112a8-104">The **UniqueBodyType** element specifies whether the unique body is returned in text or HTML format.</span></span> 
  
```XML
<UniqueBodyType> Best | HTML | Text </UniqueBodyType>
```

 <span data-ttu-id="112a8-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="112a8-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="112a8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="112a8-106">Attributes and elements</span></span>

<span data-ttu-id="112a8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="112a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="112a8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="112a8-108">Attributes</span></span>

<span data-ttu-id="112a8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="112a8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="112a8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="112a8-110">Child elements</span></span>

<span data-ttu-id="112a8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="112a8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="112a8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="112a8-112">Parent elements</span></span>

[<span data-ttu-id="112a8-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="112a8-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="112a8-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="112a8-114">Text value</span></span>

<span data-ttu-id="112a8-115">La valeur de texte de l’élément **UniqueBodyType** indique le format dans lequel le corps unique est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="112a8-115">The text value of the **UniqueBodyType** element indicates format the unique body is returned in.</span></span> <span data-ttu-id="112a8-116">Le tableau suivant répertorie les valeurs possibles pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="112a8-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="112a8-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="112a8-117">**Value**</span></span>|<span data-ttu-id="112a8-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="112a8-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="112a8-119">Idéale</span><span class="sxs-lookup"><span data-stu-id="112a8-119">Best</span></span>  <br/> |<span data-ttu-id="112a8-120">La réponse renverra le contenu disponible le plus riche du corps de texte.</span><span class="sxs-lookup"><span data-stu-id="112a8-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="112a8-121">Ceci est utile s’il n’est pas connu si le contenu est du texte ou du code HTML.</span><span class="sxs-lookup"><span data-stu-id="112a8-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="112a8-122">Le corps renvoyé sera du texte si le corps stocké est en texte brut.</span><span class="sxs-lookup"><span data-stu-id="112a8-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="112a8-123">Dans le cas contraire, la réponse renvoie HTML si le corps stocké est au format HTML ou RTF.</span><span class="sxs-lookup"><span data-stu-id="112a8-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="112a8-124">Il s’agit de la valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="112a8-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="112a8-125">HTML</span><span class="sxs-lookup"><span data-stu-id="112a8-125">HTML</span></span>  <br/> |<span data-ttu-id="112a8-126">La réponse renverra un corps unique au format HTML.</span><span class="sxs-lookup"><span data-stu-id="112a8-126">The response will return a unique body as HTML.</span></span>  <br/> |
|<span data-ttu-id="112a8-127">Texte</span><span class="sxs-lookup"><span data-stu-id="112a8-127">Text</span></span>  <br/> |<span data-ttu-id="112a8-128">La réponse renverra un corps unique en tant que texte brut.</span><span class="sxs-lookup"><span data-stu-id="112a8-128">The response will return a unique body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="112a8-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="112a8-129">Remarks</span></span>

<span data-ttu-id="112a8-130">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="112a8-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="112a8-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="112a8-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="112a8-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="112a8-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="112a8-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="112a8-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="112a8-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="112a8-134">Schema Name</span></span>  <br/> |<span data-ttu-id="112a8-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="112a8-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="112a8-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="112a8-136">Validation File</span></span>  <br/> |<span data-ttu-id="112a8-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="112a8-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="112a8-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="112a8-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="112a8-139">True</span><span class="sxs-lookup"><span data-stu-id="112a8-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="112a8-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="112a8-140">See also</span></span>



[<span data-ttu-id="112a8-141">ItemShape</span><span class="sxs-lookup"><span data-stu-id="112a8-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="112a8-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="112a8-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

