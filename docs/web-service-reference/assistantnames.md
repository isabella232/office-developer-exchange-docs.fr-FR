---
title: AssistantNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4e69022d-1cef-4744-877c-848a0b5c4f40
description: L’élément AssistantNames spécifie un tableau de noms d’assistants et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: cb3722e07da97ed472f9ae50180d61ed761413c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461540"
---
# <a name="assistantnames"></a><span data-ttu-id="5fe08-103">AssistantNames</span><span class="sxs-lookup"><span data-stu-id="5fe08-103">AssistantNames</span></span>

<span data-ttu-id="5fe08-104">L’élément **AssistantNames** spécifie un tableau de noms d’assistants et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="5fe08-104">The **AssistantNames** element specifies an array of assistant names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantNames>
    <StringAttributedValue></StringAttributedValue>
</AssistantNames>
```

 <span data-ttu-id="5fe08-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="5fe08-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5fe08-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5fe08-106">Attributes and elements</span></span>

<span data-ttu-id="5fe08-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5fe08-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5fe08-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5fe08-108">Attributes</span></span>

<span data-ttu-id="5fe08-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5fe08-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5fe08-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5fe08-110">Child elements</span></span>

|<span data-ttu-id="5fe08-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5fe08-111">**Element**</span></span>|<span data-ttu-id="5fe08-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="5fe08-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fe08-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="5fe08-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="5fe08-114">Spécifie une instance dans un tableau d’attributs associés à un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="5fe08-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5fe08-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5fe08-115">Parent elements</span></span>

|<span data-ttu-id="5fe08-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5fe08-116">**Element**</span></span>|<span data-ttu-id="5fe08-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="5fe08-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fe08-118">Persona</span><span class="sxs-lookup"><span data-stu-id="5fe08-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="5fe08-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="5fe08-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5fe08-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="5fe08-120">Remarks</span></span>

<span data-ttu-id="5fe08-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5fe08-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5fe08-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5fe08-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5fe08-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5fe08-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5fe08-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5fe08-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5fe08-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5fe08-125">Schema Name</span></span>  <br/> |<span data-ttu-id="5fe08-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="5fe08-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="5fe08-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="5fe08-127">Validation File</span></span>  <br/> |<span data-ttu-id="5fe08-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="5fe08-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5fe08-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5fe08-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5fe08-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5fe08-130">See also</span></span>

- [<span data-ttu-id="5fe08-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5fe08-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

