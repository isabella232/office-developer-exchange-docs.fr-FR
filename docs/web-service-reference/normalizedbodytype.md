---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: L’élément NormalizedBodyType spécifie si le corps normalisé est renvoyé au format texte ou HTML.
ms.openlocfilehash: e5d968673403eba24a68c67175e3ebcbb35eca39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462660"
---
# <a name="normalizedbodytype"></a><span data-ttu-id="5331e-103">NormalizedBodyType</span><span class="sxs-lookup"><span data-stu-id="5331e-103">NormalizedBodyType</span></span>

<span data-ttu-id="5331e-104">L’élément **NormalizedBodyType** spécifie si le corps normalisé est renvoyé au format texte ou html.</span><span class="sxs-lookup"><span data-stu-id="5331e-104">The **NormalizedBodyType** element specifies whether the normalized body is returned in text or HTML format.</span></span> 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 <span data-ttu-id="5331e-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="5331e-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5331e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5331e-106">Attributes and elements</span></span>

<span data-ttu-id="5331e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5331e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5331e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5331e-108">Attributes</span></span>

<span data-ttu-id="5331e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5331e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5331e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5331e-110">Child elements</span></span>

<span data-ttu-id="5331e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5331e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5331e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5331e-112">Parent elements</span></span>

[<span data-ttu-id="5331e-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="5331e-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="5331e-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="5331e-114">Text value</span></span>

<span data-ttu-id="5331e-115">La valeur de texte de l’élément **NormalizedBodyType** indique le format dans lequel le corps normalisé est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="5331e-115">The text value of the **NormalizedBodyType** element indicates format the normalized body is returned in.</span></span> <span data-ttu-id="5331e-116">Le tableau suivant répertorie les valeurs possibles pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="5331e-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="5331e-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="5331e-117">**Value**</span></span>|<span data-ttu-id="5331e-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="5331e-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5331e-119">Idéale</span><span class="sxs-lookup"><span data-stu-id="5331e-119">Best</span></span>  <br/> |<span data-ttu-id="5331e-120">La réponse renverra le contenu disponible le plus riche du corps de texte.</span><span class="sxs-lookup"><span data-stu-id="5331e-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="5331e-121">Ceci est utile s’il n’est pas connu si le contenu est du texte ou du code HTML.</span><span class="sxs-lookup"><span data-stu-id="5331e-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="5331e-122">Le corps renvoyé sera du texte si le corps stocké est en texte brut.</span><span class="sxs-lookup"><span data-stu-id="5331e-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="5331e-123">Dans le cas contraire, la réponse renvoie HTML si le corps stocké est au format HTML ou RTF.</span><span class="sxs-lookup"><span data-stu-id="5331e-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="5331e-124">Il s’agit de la valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="5331e-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="5331e-125">HTML</span><span class="sxs-lookup"><span data-stu-id="5331e-125">HTML</span></span>  <br/> |<span data-ttu-id="5331e-126">La réponse renverra un corps normalisé au format HTML.</span><span class="sxs-lookup"><span data-stu-id="5331e-126">The response will return a normalized body as HTML.</span></span>  <br/> |
|<span data-ttu-id="5331e-127">Texte</span><span class="sxs-lookup"><span data-stu-id="5331e-127">Text</span></span>  <br/> |<span data-ttu-id="5331e-128">La réponse renvoie un corps normalisé en tant que texte brut.</span><span class="sxs-lookup"><span data-stu-id="5331e-128">The response will return a normalized body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5331e-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="5331e-129">Remarks</span></span>

<span data-ttu-id="5331e-130">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5331e-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="5331e-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5331e-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5331e-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5331e-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5331e-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5331e-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5331e-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5331e-134">Schema Name</span></span>  <br/> |<span data-ttu-id="5331e-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5331e-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="5331e-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5331e-136">Validation File</span></span>  <br/> |<span data-ttu-id="5331e-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5331e-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5331e-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5331e-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="5331e-139">True</span><span class="sxs-lookup"><span data-stu-id="5331e-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5331e-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5331e-140">See also</span></span>



[<span data-ttu-id="5331e-141">ItemShape</span><span class="sxs-lookup"><span data-stu-id="5331e-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="5331e-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5331e-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

