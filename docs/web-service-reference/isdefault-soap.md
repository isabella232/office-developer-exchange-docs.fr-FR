---
title: IsDefault (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 7358bb88-c441-4f2c-9647-c030e7303e8a
description: L’élément IsDefault indique si un emplacement de partage de documents sont par défaut de l’utilisateur à l’emplacement de partage.
ms.openlocfilehash: 6e5e2958f4c9909968b976d73584b1060ee58dfa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827997"
---
# <a name="isdefault-soap"></a><span data-ttu-id="488ea-103">IsDefault (SOAP)</span><span class="sxs-lookup"><span data-stu-id="488ea-103">IsDefault (SOAP)</span></span>

<span data-ttu-id="488ea-104">L’élément **IsDefault** indique si un emplacement de partage de documents sont par défaut de l’utilisateur à l’emplacement de partage.</span><span class="sxs-lookup"><span data-stu-id="488ea-104">The **IsDefault** element indicates whether a document sharing location is the user's default sharing location.</span></span> 
  
```XML
<IsDefault /> 
```

 <span data-ttu-id="488ea-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="488ea-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="488ea-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="488ea-106">Attributes and elements</span></span>

<span data-ttu-id="488ea-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="488ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="488ea-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="488ea-108">Attributes</span></span>

<span data-ttu-id="488ea-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="488ea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="488ea-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="488ea-110">Child elements</span></span>

<span data-ttu-id="488ea-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="488ea-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="488ea-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="488ea-112">Parent elements</span></span>

|<span data-ttu-id="488ea-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="488ea-113">**Element**</span></span>|<span data-ttu-id="488ea-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="488ea-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="488ea-115">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="488ea-115">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="488ea-116">Représente les informations d’emplacement et les métadonnées pour un emplacement de partage de document.</span><span class="sxs-lookup"><span data-stu-id="488ea-116">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="488ea-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="488ea-117">Text value</span></span>

<span data-ttu-id="488ea-118">La valeur de type Boolean de l’élément **IsDefault** indique si l’emplacement de partage est par défaut de l’utilisateur à l’emplacement de partage.</span><span class="sxs-lookup"><span data-stu-id="488ea-118">The Boolean value of the **IsDefault** element indicates whether the sharing location is the user's default sharing location.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="488ea-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="488ea-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="488ea-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="488ea-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="488ea-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="488ea-121">Schema Name</span></span>  <br/> |<span data-ttu-id="488ea-122">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="488ea-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="488ea-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="488ea-123">Validation File</span></span>  <br/> |<span data-ttu-id="488ea-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="488ea-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="488ea-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="488ea-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="488ea-126">True</span><span class="sxs-lookup"><span data-stu-id="488ea-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="488ea-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="488ea-127">See also</span></span>



[<span data-ttu-id="488ea-128">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="488ea-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="488ea-129">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="488ea-129">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="488ea-130">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="488ea-130">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

