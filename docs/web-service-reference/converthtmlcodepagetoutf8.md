---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: L’élément ConvertHtmlCodePageToUTF8 indique si le corps HTML de l’élément est converti en UTF8.
ms.openlocfilehash: a714eacd8cc105146a1471f062ec35dc16730d61
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457591"
---
# <a name="converthtmlcodepagetoutf8"></a><span data-ttu-id="bfa9a-103">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="bfa9a-103">ConvertHtmlCodePageToUTF8</span></span>

<span data-ttu-id="bfa9a-104">L’élément **ConvertHtmlCodePageToUTF8** indique si le corps HTML de l’élément est converti en UTF8.</span><span class="sxs-lookup"><span data-stu-id="bfa9a-104">The **ConvertHtmlCodePageToUTF8** element indicates whether the item HTML body is converted to UTF8.</span></span> 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 <span data-ttu-id="bfa9a-105">**XS : Boolean**</span><span class="sxs-lookup"><span data-stu-id="bfa9a-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bfa9a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bfa9a-106">Attributes and elements</span></span>

<span data-ttu-id="bfa9a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bfa9a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bfa9a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bfa9a-108">Attributes</span></span>

<span data-ttu-id="bfa9a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bfa9a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bfa9a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bfa9a-110">Child elements</span></span>

<span data-ttu-id="bfa9a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bfa9a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bfa9a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bfa9a-112">Parent elements</span></span>

|<span data-ttu-id="bfa9a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bfa9a-113">**Element**</span></span>|<span data-ttu-id="bfa9a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="bfa9a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfa9a-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="bfa9a-115">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="bfa9a-116">Identifie un jeu de propriétés à renvoyer dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="bfa9a-116">Identifies a set of properties to return in a response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bfa9a-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="bfa9a-117">Text value</span></span>

<span data-ttu-id="bfa9a-118">Une valeur de texte de **true** pour l’élément **ConvertHtmlCodePageToUTF8** indique que le corps HTML est converti en UTF8.</span><span class="sxs-lookup"><span data-stu-id="bfa9a-118">A text value of **true** for the **ConvertHtmlCodePageToUTF8** element indicates that the HTML body is converted to UTF8.</span></span> <span data-ttu-id="bfa9a-119">Une valeur de texte **false** indique que le corps HTML n’est pas converti en UTF8.</span><span class="sxs-lookup"><span data-stu-id="bfa9a-119">A text value of **false** indicates that the HTML body is not converted to UTF8.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bfa9a-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="bfa9a-120">Remarks</span></span>

<span data-ttu-id="bfa9a-121">La valeur par défaut **true** est utilisée si l’élément **ConvertHtmlCodePageToUTF8** n’est pas spécifié dans une demande.</span><span class="sxs-lookup"><span data-stu-id="bfa9a-121">The default value of **true** is used if the **ConvertHtmlCodePageToUTF8** element is not specified in a request.</span></span> 
  
<span data-ttu-id="bfa9a-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="bfa9a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bfa9a-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bfa9a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bfa9a-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bfa9a-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bfa9a-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bfa9a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="bfa9a-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bfa9a-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="bfa9a-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bfa9a-127">Validation File</span></span>  <br/> |<span data-ttu-id="bfa9a-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bfa9a-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bfa9a-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bfa9a-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="bfa9a-130">False</span><span class="sxs-lookup"><span data-stu-id="bfa9a-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bfa9a-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bfa9a-131">See also</span></span>



- [<span data-ttu-id="bfa9a-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bfa9a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

