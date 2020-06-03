---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: L’élément AggregationRestriction spécifie une valeur qui est appliquée à un ensemble de propriétés Persona résultant d’une demande FindPeople et filtre le résultat en fonction de la restriction spécifiée.
ms.openlocfilehash: f07e54235cf13b43da26ed1c56596d3c7c357bf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463523"
---
# <a name="aggregationrestriction"></a><span data-ttu-id="825c2-103">AggregationRestriction</span><span class="sxs-lookup"><span data-stu-id="825c2-103">AggregationRestriction</span></span>

<span data-ttu-id="825c2-104">L’élément **AggregationRestriction** spécifie une valeur qui est appliquée à un ensemble de propriétés Persona résultant d’une demande FindPeople et filtre le résultat en fonction de la restriction spécifiée.</span><span class="sxs-lookup"><span data-stu-id="825c2-104">The **AggregationRestriction** element specifies a value that is applied to a set of Persona properties resulting from a FindPeople request and filters the result according to the specified restriction.</span></span> 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 <span data-ttu-id="825c2-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="825c2-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="825c2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="825c2-106">Attributes and elements</span></span>

<span data-ttu-id="825c2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="825c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="825c2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="825c2-108">Attributes</span></span>

<span data-ttu-id="825c2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="825c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="825c2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="825c2-110">Child elements</span></span>

[<span data-ttu-id="825c2-111">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="825c2-111">SearchExpression</span></span>](searchexpression.md)
  
### <a name="parent-elements"></a><span data-ttu-id="825c2-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="825c2-112">Parent elements</span></span>

[<span data-ttu-id="825c2-113">FindPeople</span><span class="sxs-lookup"><span data-stu-id="825c2-113">FindPeople</span></span>](findpeople.md)
  
## <a name="remarks"></a><span data-ttu-id="825c2-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="825c2-114">Remarks</span></span>

<span data-ttu-id="825c2-115">L’élément **AggregationRestriction** peut contenir n’importe quel élément enfant qui utilise le groupe de substitution **SearchExpression** .</span><span class="sxs-lookup"><span data-stu-id="825c2-115">The **AggregationRestriction** element can contain any child element that uses the **SearchExpression** substitution group.</span></span> <span data-ttu-id="825c2-116">Les éléments qui font partie du groupe de substitution **SearchExpression** sont les suivants : [Contains](contains.md), [excludes](excludes.md), [Exists](exists.md), [not](not.md), [or](or.md), [and](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md)et [IsLessThanOrEqualTo](islessthanorequalto.md).</span><span class="sxs-lookup"><span data-stu-id="825c2-116">The elements that are a part of the **SearchExpression** substitution group are: [Contains](contains.md), [Excludes](excludes.md), [Exists](exists.md), [Not](not.md), [Or](or.md), [And](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md), and [IsLessThanOrEqualTo](islessthanorequalto.md).</span></span>
  
<span data-ttu-id="825c2-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="825c2-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="825c2-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="825c2-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="825c2-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="825c2-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="825c2-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="825c2-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="825c2-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="825c2-121">Schema name</span></span>  <br/> |<span data-ttu-id="825c2-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="825c2-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="825c2-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="825c2-123">Validation file</span></span>  <br/> |<span data-ttu-id="825c2-124">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="825c2-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="825c2-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="825c2-125">Can be empty</span></span>  <br/> |<span data-ttu-id="825c2-126">false</span><span class="sxs-lookup"><span data-stu-id="825c2-126">false</span></span>  <br/> |
   

