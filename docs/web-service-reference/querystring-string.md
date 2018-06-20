---
title: QueryString (chaîne)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: L’élément QueryString spécifie un ensemble de valeurs à renvoyer qui correspondent à la chaîne de requête dans une requête d’opération FindPeople. Une recherche avec aucune chaîne de requête spécifiée retourne tous les éléments à partir du dossier spécifié.
ms.openlocfilehash: 9c5c733adcec1496e36986fd720b56b0a0274593
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828935"
---
# <a name="querystring-string"></a><span data-ttu-id="3cde0-104">QueryString (chaîne)</span><span class="sxs-lookup"><span data-stu-id="3cde0-104">QueryString (String)</span></span>

<span data-ttu-id="3cde0-105">L’élément **QueryString** spécifie un ensemble de valeurs à renvoyer qui correspondent à la chaîne de requête dans une requête [d’opération FindPeople](findpeople-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3cde0-105">The **QueryString** element specifies a set of values to be returned that match the query string in a [FindPeople operation](findpeople-operation.md) request.</span></span> <span data-ttu-id="3cde0-106">Une recherche avec aucune **chaîne de requête** spécifiée retourne tous les éléments à partir du dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="3cde0-106">A search with no **QueryString** specified returns all items from the specified folder.</span></span> 
  
```XML
<QueryString/> 
```

 <span data-ttu-id="3cde0-107">**string**</span><span class="sxs-lookup"><span data-stu-id="3cde0-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3cde0-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3cde0-108">Attributes and elements</span></span>

<span data-ttu-id="3cde0-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3cde0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3cde0-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="3cde0-110">Attributes</span></span>

<span data-ttu-id="3cde0-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3cde0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3cde0-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3cde0-112">Child elements</span></span>

<span data-ttu-id="3cde0-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3cde0-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3cde0-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3cde0-114">Parent elements</span></span>

|<span data-ttu-id="3cde0-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3cde0-115">**Element**</span></span>|<span data-ttu-id="3cde0-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="3cde0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3cde0-117">FindPeople</span><span class="sxs-lookup"><span data-stu-id="3cde0-117">FindPeople</span></span>](findpeople.md) <br/> |<span data-ttu-id="3cde0-118">Contient les arguments pour une recherche de [l’opération FindPeople](findpeople-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3cde0-118">Contains the arguments for a [FindPeople operation](findpeople-operation.md) search.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3cde0-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3cde0-119">Text value</span></span>

<span data-ttu-id="3cde0-120">La valeur de texte **QueryString** représente une requête de boîte aux lettres effectuée à l’aide d’un sous-ensemble de [La syntaxe de requête avancée (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="3cde0-120">The **QueryString** text value represents a mailbox query made by using a subset of [Advanced Query Syntax (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="3cde0-121">Pour plus d’informations sur la syntaxe de cet élément, voir [QueryString (QueryStringType)](querystring-querystringtype.md).</span><span class="sxs-lookup"><span data-stu-id="3cde0-121">For information about the syntax for this element, see [QueryString (QueryStringType)](querystring-querystringtype.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3cde0-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="3cde0-122">Remarks</span></span>

<span data-ttu-id="3cde0-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3cde0-123">This element was introduced in Exchange Server 2013.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3cde0-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3cde0-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3cde0-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3cde0-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3cde0-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3cde0-126">Schema name</span></span>  <br/> |<span data-ttu-id="3cde0-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3cde0-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3cde0-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3cde0-128">Validation file</span></span>  <br/> |<span data-ttu-id="3cde0-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3cde0-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3cde0-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3cde0-130">Can be empty</span></span>  <br/> |<span data-ttu-id="3cde0-131">False</span><span class="sxs-lookup"><span data-stu-id="3cde0-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3cde0-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3cde0-132">See also</span></span>



[<span data-ttu-id="3cde0-133">Opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="3cde0-133">FindPeople operation</span></span>](findpeople-operation.md)


- [<span data-ttu-id="3cde0-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3cde0-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

