---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: L’élément ConvertHtmlCodePageToUTF8 indique si l’élément corps HTML est converti en UTF-8.
ms.openlocfilehash: aff6579835097a273101188c02a9919003b71b58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755657"
---
# <a name="converthtmlcodepagetoutf8"></a><span data-ttu-id="9ba55-103">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="9ba55-103">ConvertHtmlCodePageToUTF8</span></span>

<span data-ttu-id="9ba55-104">L’élément **ConvertHtmlCodePageToUTF8** indique si l’élément corps HTML est converti en UTF-8.</span><span class="sxs-lookup"><span data-stu-id="9ba55-104">The **ConvertHtmlCodePageToUTF8** element indicates whether the item HTML body is converted to UTF8.</span></span> 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 <span data-ttu-id="9ba55-105">**xs : Boolean**</span><span class="sxs-lookup"><span data-stu-id="9ba55-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ba55-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9ba55-106">Attributes and elements</span></span>

<span data-ttu-id="9ba55-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9ba55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ba55-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9ba55-108">Attributes</span></span>

<span data-ttu-id="9ba55-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9ba55-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ba55-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9ba55-110">Child elements</span></span>

<span data-ttu-id="9ba55-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9ba55-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9ba55-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9ba55-112">Parent elements</span></span>

|<span data-ttu-id="9ba55-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9ba55-113">**Element**</span></span>|<span data-ttu-id="9ba55-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9ba55-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ba55-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="9ba55-115">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="9ba55-116">Identifie un ensemble de propriétés à retourner dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="9ba55-116">Identifies a set of properties to return in a response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9ba55-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9ba55-117">Text value</span></span>

<span data-ttu-id="9ba55-118">Une valeur de texte de **la valeur true** pour l’élément **ConvertHtmlCodePageToUTF8** indique que le corps HTML est converti en UTF-8.</span><span class="sxs-lookup"><span data-stu-id="9ba55-118">A text value of **true** for the **ConvertHtmlCodePageToUTF8** element indicates that the HTML body is converted to UTF8.</span></span> <span data-ttu-id="9ba55-119">Texte la valeur **false** indique que le corps HTML n’est pas converti en UTF-8.</span><span class="sxs-lookup"><span data-stu-id="9ba55-119">A text value of **false** indicates that the HTML body is not converted to UTF8.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9ba55-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="9ba55-120">Remarks</span></span>

<span data-ttu-id="9ba55-121">La valeur par défaut **true** est utilisée si l’élément **ConvertHtmlCodePageToUTF8** n’est pas spécifié dans une requête.</span><span class="sxs-lookup"><span data-stu-id="9ba55-121">The default value of **true** is used if the **ConvertHtmlCodePageToUTF8** element is not specified in a request.</span></span> 
  
<span data-ttu-id="9ba55-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9ba55-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ba55-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9ba55-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ba55-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9ba55-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ba55-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9ba55-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9ba55-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9ba55-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ba55-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9ba55-127">Validation File</span></span>  <br/> |<span data-ttu-id="9ba55-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9ba55-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ba55-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9ba55-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ba55-130">False</span><span class="sxs-lookup"><span data-stu-id="9ba55-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ba55-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9ba55-131">See also</span></span>



- [<span data-ttu-id="9ba55-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9ba55-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

