---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: L’élément AggregationRestriction spécifie une valeur qui est appliquée à un ensemble de propriétés personnage résultant d’une demande FindPeople et filtre les résultats en fonction de la restriction spécifiée.
ms.openlocfilehash: 8b4d5952dedb4de0201d2ecf2219c69f65f7dc09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755193"
---
# <a name="aggregationrestriction"></a><span data-ttu-id="245ee-103">AggregationRestriction</span><span class="sxs-lookup"><span data-stu-id="245ee-103">AggregationRestriction</span></span>

<span data-ttu-id="245ee-104">L’élément **AggregationRestriction** spécifie une valeur qui est appliquée à un ensemble de propriétés personnage résultant d’une demande FindPeople et filtre les résultats en fonction de la restriction spécifiée.</span><span class="sxs-lookup"><span data-stu-id="245ee-104">The **AggregationRestriction** element specifies a value that is applied to a set of Persona properties resulting from a FindPeople request and filters the result according to the specified restriction.</span></span> 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 <span data-ttu-id="245ee-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="245ee-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="245ee-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="245ee-106">Attributes and elements</span></span>

<span data-ttu-id="245ee-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="245ee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="245ee-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="245ee-108">Attributes</span></span>

<span data-ttu-id="245ee-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="245ee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="245ee-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="245ee-110">Child elements</span></span>

[<span data-ttu-id="245ee-111">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="245ee-111">SearchExpression</span></span>](searchexpression.md)
  
### <a name="parent-elements"></a><span data-ttu-id="245ee-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="245ee-112">Parent elements</span></span>

[<span data-ttu-id="245ee-113">FindPeople</span><span class="sxs-lookup"><span data-stu-id="245ee-113">FindPeople</span></span>](findpeople.md)
  
## <a name="remarks"></a><span data-ttu-id="245ee-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="245ee-114">Remarks</span></span>

<span data-ttu-id="245ee-115">L’élément **AggregationRestriction** peut contenir n’importe quel élément enfant qui utilise le groupe de substitution **SearchExpression** .</span><span class="sxs-lookup"><span data-stu-id="245ee-115">The **AggregationRestriction** element can contain any child element that uses the **SearchExpression** substitution group.</span></span> <span data-ttu-id="245ee-116">Les éléments qui font partie du groupe de substitution **SearchExpression** sont : [Contains](contains.md), [exclut](excludes.md), [Exists](exists.md), [pas](not.md), [ou](or.md) [et](and.md), [plutôt IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan ](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md)et [IsLessThanOrEqualTo](islessthanorequalto.md).</span><span class="sxs-lookup"><span data-stu-id="245ee-116">The elements that are a part of the **SearchExpression** substitution group are: [Contains](contains.md), [Excludes](excludes.md), [Exists](exists.md), [Not](not.md), [Or](or.md), [And](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md), and [IsLessThanOrEqualTo](islessthanorequalto.md).</span></span>
  
<span data-ttu-id="245ee-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="245ee-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="245ee-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="245ee-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="245ee-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="245ee-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="245ee-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="245ee-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="245ee-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="245ee-121">Schema name</span></span>  <br/> |<span data-ttu-id="245ee-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="245ee-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="245ee-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="245ee-123">Validation file</span></span>  <br/> |<span data-ttu-id="245ee-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="245ee-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="245ee-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="245ee-125">Can be empty</span></span>  <br/> |<span data-ttu-id="245ee-126">false</span><span class="sxs-lookup"><span data-stu-id="245ee-126">false</span></span>  <br/> |
   

