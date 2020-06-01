---
title: BusinessHomePages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9961c0c2-7cac-4af1-84ac-0eafdce0a6ab
description: L’élément BusinessHomePages spécifie un tableau de pages d’accueil professionnelles et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: f0e85e0b3c857e44d94bd42c6d3ea757d015eb25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465911"
---
# <a name="businesshomepages"></a><span data-ttu-id="9f7d6-103">BusinessHomePages</span><span class="sxs-lookup"><span data-stu-id="9f7d6-103">BusinessHomePages</span></span>

<span data-ttu-id="9f7d6-104">L’élément **BusinessHomePages** spécifie un tableau de pages d’accueil professionnelles et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="9f7d6-104">The **BusinessHomePages** element specifies an array of business home pages and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessHomePages>
    <StringAttributedValue></StringAttributedValue>
</BusinessHomePages>
```

 <span data-ttu-id="9f7d6-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="9f7d6-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f7d6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9f7d6-106">Attributes and elements</span></span>

<span data-ttu-id="9f7d6-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9f7d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f7d6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9f7d6-108">Attributes</span></span>

<span data-ttu-id="9f7d6-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9f7d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f7d6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9f7d6-110">Child elements</span></span>

|<span data-ttu-id="9f7d6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9f7d6-111">**Element**</span></span>|<span data-ttu-id="9f7d6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f7d6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f7d6-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="9f7d6-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="9f7d6-114">Spécifie une instance dans un tableau d’attributs associés à un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="9f7d6-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f7d6-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9f7d6-115">Parent elements</span></span>

|<span data-ttu-id="9f7d6-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9f7d6-116">**Element**</span></span>|<span data-ttu-id="9f7d6-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f7d6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f7d6-118">Persona</span><span class="sxs-lookup"><span data-stu-id="9f7d6-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="9f7d6-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="9f7d6-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f7d6-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="9f7d6-120">Remarks</span></span>

<span data-ttu-id="9f7d6-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9f7d6-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9f7d6-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f7d6-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f7d6-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9f7d6-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f7d6-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9f7d6-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f7d6-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9f7d6-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9f7d6-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="9f7d6-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="9f7d6-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="9f7d6-127">Validation File</span></span>  <br/> |<span data-ttu-id="9f7d6-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="9f7d6-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f7d6-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9f7d6-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9f7d6-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9f7d6-130">See also</span></span>



- [<span data-ttu-id="9f7d6-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9f7d6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

