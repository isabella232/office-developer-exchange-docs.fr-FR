---
title: Langue (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: L’élément de langage (DiscoverySearchConfigurationType) identifie la culture à utiliser pour le format spécifiques à la culture des plages de dates. Il indique également la langue utilisée dans une requête de recherche.
ms.openlocfilehash: 1e904ac4d7f525b2d12cfe83f0da33b9ed474066
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828197"
---
# <a name="language-discoverysearchconfigurationtype"></a><span data-ttu-id="6e90c-104">Langue (DiscoverySearchConfigurationType)</span><span class="sxs-lookup"><span data-stu-id="6e90c-104">Language (DiscoverySearchConfigurationType)</span></span>

<span data-ttu-id="6e90c-105">L’élément de **langage (DiscoverySearchConfigurationType)** identifie la culture à utiliser pour le format spécifiques à la culture des plages de dates.</span><span class="sxs-lookup"><span data-stu-id="6e90c-105">The **Language (DiscoverySearchConfigurationType)** element identifies the culture to be used for the culture-specific format of date ranges.</span></span> <span data-ttu-id="6e90c-106">Il indique également la langue utilisée dans une requête de recherche.</span><span class="sxs-lookup"><span data-stu-id="6e90c-106">It also specifies the language used in a search query.</span></span> 
  
```XML
<Language />
```

 <span data-ttu-id="6e90c-107">**string**</span><span class="sxs-lookup"><span data-stu-id="6e90c-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e90c-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6e90c-108">Attributes and elements</span></span>

<span data-ttu-id="6e90c-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6e90c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e90c-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="6e90c-110">Attributes</span></span>

<span data-ttu-id="6e90c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6e90c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e90c-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6e90c-112">Child elements</span></span>

<span data-ttu-id="6e90c-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6e90c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6e90c-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6e90c-114">Parent elements</span></span>

[<span data-ttu-id="6e90c-115">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e90c-115">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="6e90c-116">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6e90c-116">Text value</span></span>

<span data-ttu-id="6e90c-117">La valeur de texte de l’élément de **langage (DiscoverySearchConfigurationType)** est une culture ou une langue.</span><span class="sxs-lookup"><span data-stu-id="6e90c-117">The text value of the **Language (DiscoverySearchConfigurationType)** element is a culture or language.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6e90c-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="6e90c-118">Remarks</span></span>

<span data-ttu-id="6e90c-119">Cet élément spécifie le format des plages de dates spécifiée dans l' [opération SearchMailboxes](searchmailboxes-operation.md) ou l' [opération SetHoldOnMailboxes](setholdonmailboxes-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6e90c-119">This element specifies the format of date ranges specified in the [SearchMailboxes operation](searchmailboxes-operation.md) or the [SetHoldOnMailboxes operation](setholdonmailboxes-operation.md).</span></span>
  
<span data-ttu-id="6e90c-120">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6e90c-120">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="6e90c-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e90c-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e90c-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6e90c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e90c-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6e90c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e90c-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6e90c-124">Schema Name</span></span>  <br/> |<span data-ttu-id="6e90c-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6e90c-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="6e90c-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6e90c-126">Validation File</span></span>  <br/> |<span data-ttu-id="6e90c-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6e90c-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e90c-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6e90c-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e90c-129">True</span><span class="sxs-lookup"><span data-stu-id="6e90c-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e90c-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6e90c-130">See also</span></span>



[<span data-ttu-id="6e90c-131">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e90c-131">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)


- [<span data-ttu-id="6e90c-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6e90c-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

