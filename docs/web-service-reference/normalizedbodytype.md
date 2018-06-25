---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: L’élément NormalizedBodyType Spécifie si le corps normalisé est retourné dans le format HTML ou texte.
ms.openlocfilehash: 33575594b22f972a9eb762dfac884fa91459f04a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828554"
---
# <a name="normalizedbodytype"></a><span data-ttu-id="811c0-103">NormalizedBodyType</span><span class="sxs-lookup"><span data-stu-id="811c0-103">NormalizedBodyType</span></span>

<span data-ttu-id="811c0-104">L’élément **NormalizedBodyType** Spécifie si le corps normalisé est retourné dans le format HTML ou texte.</span><span class="sxs-lookup"><span data-stu-id="811c0-104">The **NormalizedBodyType** element specifies whether the normalized body is returned in text or HTML format.</span></span> 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 <span data-ttu-id="811c0-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="811c0-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="811c0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="811c0-106">Attributes and elements</span></span>

<span data-ttu-id="811c0-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="811c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="811c0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="811c0-108">Attributes</span></span>

<span data-ttu-id="811c0-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="811c0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="811c0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="811c0-110">Child elements</span></span>

<span data-ttu-id="811c0-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="811c0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="811c0-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="811c0-112">Parent elements</span></span>

[<span data-ttu-id="811c0-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="811c0-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="811c0-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="811c0-114">Text value</span></span>

<span data-ttu-id="811c0-115">La valeur de texte de l’élément **NormalizedBodyType** indique le format du corps normalisé est renvoyée dans.</span><span class="sxs-lookup"><span data-stu-id="811c0-115">The text value of the **NormalizedBodyType** element indicates format the normalized body is returned in.</span></span> <span data-ttu-id="811c0-116">Le tableau suivant répertorie les valeurs possibles de cet élément.</span><span class="sxs-lookup"><span data-stu-id="811c0-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="811c0-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="811c0-117">**Value**</span></span>|<span data-ttu-id="811c0-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="811c0-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="811c0-119">Recommandé</span><span class="sxs-lookup"><span data-stu-id="811c0-119">Best</span></span>  <br/> |<span data-ttu-id="811c0-120">La réponse renvoie le contenu disponible plus riche du corps de texte.</span><span class="sxs-lookup"><span data-stu-id="811c0-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="811c0-121">Cela est utile si elle est inconnue ou non le contenu est texte ou HTML.</span><span class="sxs-lookup"><span data-stu-id="811c0-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="811c0-122">Le corps retourné sera texte si le corps stocké est en texte brut.</span><span class="sxs-lookup"><span data-stu-id="811c0-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="811c0-123">Dans le cas contraire, la réponse renverra HTML si le corps stocké est au format HTML ou RTF.</span><span class="sxs-lookup"><span data-stu-id="811c0-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="811c0-124">Il s'agit de la valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="811c0-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="811c0-125">HTML</span><span class="sxs-lookup"><span data-stu-id="811c0-125">HTML</span></span>  <br/> |<span data-ttu-id="811c0-126">La réponse renvoie un corps normalisé au format HTML.</span><span class="sxs-lookup"><span data-stu-id="811c0-126">The response will return a normalized body as HTML.</span></span>  <br/> |
|<span data-ttu-id="811c0-127">Texte</span><span class="sxs-lookup"><span data-stu-id="811c0-127">Text</span></span>  <br/> |<span data-ttu-id="811c0-128">La réponse renvoie un corps normalisé sous forme de texte brut.</span><span class="sxs-lookup"><span data-stu-id="811c0-128">The response will return a normalized body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="811c0-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="811c0-129">Remarks</span></span>

<span data-ttu-id="811c0-130">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="811c0-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="811c0-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="811c0-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="811c0-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="811c0-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="811c0-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="811c0-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="811c0-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="811c0-134">Schema Name</span></span>  <br/> |<span data-ttu-id="811c0-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="811c0-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="811c0-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="811c0-136">Validation File</span></span>  <br/> |<span data-ttu-id="811c0-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="811c0-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="811c0-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="811c0-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="811c0-139">True</span><span class="sxs-lookup"><span data-stu-id="811c0-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="811c0-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="811c0-140">See also</span></span>



[<span data-ttu-id="811c0-141">ItemShape</span><span class="sxs-lookup"><span data-stu-id="811c0-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="811c0-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="811c0-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

