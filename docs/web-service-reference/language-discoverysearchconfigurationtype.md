---
title: Langue (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: L’élément Language (DiscoverySearchConfigurationType) identifie la culture à utiliser pour le format spécifique à la culture des plages de dates. Il spécifie également la langue utilisée dans une requête de recherche.
ms.openlocfilehash: 3cf85525147bec5d6dfc6fe2b2af5916d42c44be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463285"
---
# <a name="language-discoverysearchconfigurationtype"></a><span data-ttu-id="80f0b-104">Langue (DiscoverySearchConfigurationType)</span><span class="sxs-lookup"><span data-stu-id="80f0b-104">Language (DiscoverySearchConfigurationType)</span></span>

<span data-ttu-id="80f0b-105">L’élément **Language (DiscoverySearchConfigurationType)** identifie la culture à utiliser pour le format spécifique à la culture des plages de dates.</span><span class="sxs-lookup"><span data-stu-id="80f0b-105">The **Language (DiscoverySearchConfigurationType)** element identifies the culture to be used for the culture-specific format of date ranges.</span></span> <span data-ttu-id="80f0b-106">Il spécifie également la langue utilisée dans une requête de recherche.</span><span class="sxs-lookup"><span data-stu-id="80f0b-106">It also specifies the language used in a search query.</span></span> 
  
```XML
<Language />
```

 <span data-ttu-id="80f0b-107">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="80f0b-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80f0b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="80f0b-108">Attributes and elements</span></span>

<span data-ttu-id="80f0b-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="80f0b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80f0b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="80f0b-110">Attributes</span></span>

<span data-ttu-id="80f0b-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="80f0b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80f0b-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="80f0b-112">Child elements</span></span>

<span data-ttu-id="80f0b-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="80f0b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80f0b-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="80f0b-114">Parent elements</span></span>

[<span data-ttu-id="80f0b-115">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="80f0b-115">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="80f0b-116">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="80f0b-116">Text value</span></span>

<span data-ttu-id="80f0b-117">La valeur de texte de l’élément **Language (DiscoverySearchConfigurationType)** est une culture ou une langue.</span><span class="sxs-lookup"><span data-stu-id="80f0b-117">The text value of the **Language (DiscoverySearchConfigurationType)** element is a culture or language.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="80f0b-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="80f0b-118">Remarks</span></span>

<span data-ttu-id="80f0b-119">Cet élément spécifie le format des plages de dates spécifiées dans l' [opération SearchMailboxes](searchmailboxes-operation.md) ou l' [opération SetHoldOnMailboxes](setholdonmailboxes-operation.md).</span><span class="sxs-lookup"><span data-stu-id="80f0b-119">This element specifies the format of date ranges specified in the [SearchMailboxes operation](searchmailboxes-operation.md) or the [SetHoldOnMailboxes operation](setholdonmailboxes-operation.md).</span></span>
  
<span data-ttu-id="80f0b-120">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="80f0b-120">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="80f0b-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="80f0b-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80f0b-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="80f0b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80f0b-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="80f0b-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80f0b-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="80f0b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="80f0b-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="80f0b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="80f0b-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="80f0b-126">Validation File</span></span>  <br/> |<span data-ttu-id="80f0b-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="80f0b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80f0b-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="80f0b-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="80f0b-129">True</span><span class="sxs-lookup"><span data-stu-id="80f0b-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80f0b-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="80f0b-130">See also</span></span>



[<span data-ttu-id="80f0b-131">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="80f0b-131">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)


- [<span data-ttu-id="80f0b-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="80f0b-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

