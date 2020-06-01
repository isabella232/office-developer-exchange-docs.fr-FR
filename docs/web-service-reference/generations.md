---
title: Production
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 637560b5-2b08-4787-a5d8-e0467f83acca
description: L’élément complications spécifie un tableau de valeurs de génération et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: a3ef0e2c73e2ebd7c121f817b8ea97c5e4d4d333
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463012"
---
# <a name="generations"></a><span data-ttu-id="0f7ab-103">Production</span><span class="sxs-lookup"><span data-stu-id="0f7ab-103">Generations</span></span>

<span data-ttu-id="0f7ab-104">L’élément **complications** spécifie un tableau de valeurs de génération et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="0f7ab-104">The **Generations** element specifies an array of generation values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Generations>
    <StringAttributedValue/>
</Generations>
```

 <span data-ttu-id="0f7ab-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="0f7ab-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f7ab-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0f7ab-106">Attributes and elements</span></span>

<span data-ttu-id="0f7ab-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0f7ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f7ab-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0f7ab-108">Attributes</span></span>

<span data-ttu-id="0f7ab-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0f7ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f7ab-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0f7ab-110">Child elements</span></span>

|<span data-ttu-id="0f7ab-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f7ab-111">**Element**</span></span>|<span data-ttu-id="0f7ab-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f7ab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f7ab-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="0f7ab-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="0f7ab-114">Spécifie une instance dans un tableau d’attributs associés à un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="0f7ab-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f7ab-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0f7ab-115">Parent elements</span></span>

|<span data-ttu-id="0f7ab-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f7ab-116">**Element**</span></span>|<span data-ttu-id="0f7ab-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f7ab-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f7ab-118">Persona</span><span class="sxs-lookup"><span data-stu-id="0f7ab-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="0f7ab-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="0f7ab-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0f7ab-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="0f7ab-120">Remarks</span></span>

<span data-ttu-id="0f7ab-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0f7ab-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0f7ab-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f7ab-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f7ab-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0f7ab-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f7ab-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0f7ab-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f7ab-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0f7ab-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0f7ab-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="0f7ab-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="0f7ab-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="0f7ab-127">Validation File</span></span>  <br/> |<span data-ttu-id="0f7ab-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="0f7ab-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f7ab-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0f7ab-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0f7ab-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0f7ab-130">See also</span></span>



- [<span data-ttu-id="0f7ab-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0f7ab-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

