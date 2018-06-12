---
title: GivenNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 64d86c24-07b8-448d-ad37-47f104777df3
description: L’élément GivenNames spécifie un tableau de valeurs de nom donné et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: dc86517a06dab0f74350c71488f68bb06e2272bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827709"
---
# <a name="givennames"></a><span data-ttu-id="a8bdd-103">GivenNames</span><span class="sxs-lookup"><span data-stu-id="a8bdd-103">GivenNames</span></span>

<span data-ttu-id="a8bdd-104">L’élément **GivenNames** spécifie un tableau de valeurs de nom donné et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="a8bdd-104">The **GivenNames** element specifies an array of given name values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```xml
<GivenNames>
    <StringAttributedValue/>
</GivenNames>
```

 <span data-ttu-id="a8bdd-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="a8bdd-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8bdd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a8bdd-106">Attributes and elements</span></span>

<span data-ttu-id="a8bdd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a8bdd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8bdd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a8bdd-108">Attributes</span></span>

<span data-ttu-id="a8bdd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a8bdd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8bdd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a8bdd-110">Child elements</span></span>

|<span data-ttu-id="a8bdd-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a8bdd-111">**Element**</span></span>|<span data-ttu-id="a8bdd-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8bdd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8bdd-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="a8bdd-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="a8bdd-114">Spécifie une instance d’un tableau d’attributs associés à un élément personnage.</span><span class="sxs-lookup"><span data-stu-id="a8bdd-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8bdd-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a8bdd-115">Parent elements</span></span>

|<span data-ttu-id="a8bdd-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a8bdd-116">**Element**</span></span>|<span data-ttu-id="a8bdd-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8bdd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8bdd-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="a8bdd-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="a8bdd-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="a8bdd-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a8bdd-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="a8bdd-120">Remarks</span></span>

<span data-ttu-id="a8bdd-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a8bdd-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a8bdd-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8bdd-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8bdd-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a8bdd-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8bdd-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a8bdd-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8bdd-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a8bdd-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a8bdd-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="a8bdd-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="a8bdd-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="a8bdd-127">Validation File</span></span>  <br/> |<span data-ttu-id="a8bdd-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="a8bdd-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8bdd-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a8bdd-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a8bdd-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a8bdd-130">See also</span></span>



- [<span data-ttu-id="a8bdd-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a8bdd-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

