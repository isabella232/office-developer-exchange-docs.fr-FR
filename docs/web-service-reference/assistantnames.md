---
title: AssistantNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4e69022d-1cef-4744-877c-848a0b5c4f40
description: L’élément AssistantNames spécifie un tableau de noms de l’assistant et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: 7414caa74dc8221d0b1b471c3d5ed09552f7e200
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755329"
---
# <a name="assistantnames"></a><span data-ttu-id="982ab-103">AssistantNames</span><span class="sxs-lookup"><span data-stu-id="982ab-103">AssistantNames</span></span>

<span data-ttu-id="982ab-104">L’élément **AssistantNames** spécifie un tableau de noms de l’assistant et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="982ab-104">The **AssistantNames** element specifies an array of assistant names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantNames>
    <StringAttributedValue></StringAttributedValue>
</AssistantNames>
```

 <span data-ttu-id="982ab-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="982ab-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="982ab-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="982ab-106">Attributes and elements</span></span>

<span data-ttu-id="982ab-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="982ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="982ab-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="982ab-108">Attributes</span></span>

<span data-ttu-id="982ab-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="982ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="982ab-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="982ab-110">Child elements</span></span>

|<span data-ttu-id="982ab-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="982ab-111">**Element**</span></span>|<span data-ttu-id="982ab-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="982ab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="982ab-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="982ab-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="982ab-114">Spécifie une instance d’un tableau d’attributs associés à un élément personnage.</span><span class="sxs-lookup"><span data-stu-id="982ab-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="982ab-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="982ab-115">Parent elements</span></span>

|<span data-ttu-id="982ab-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="982ab-116">**Element**</span></span>|<span data-ttu-id="982ab-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="982ab-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="982ab-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="982ab-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="982ab-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="982ab-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="982ab-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="982ab-120">Remarks</span></span>

<span data-ttu-id="982ab-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="982ab-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="982ab-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="982ab-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="982ab-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="982ab-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="982ab-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="982ab-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="982ab-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="982ab-125">Schema Name</span></span>  <br/> |<span data-ttu-id="982ab-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="982ab-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="982ab-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="982ab-127">Validation File</span></span>  <br/> |<span data-ttu-id="982ab-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="982ab-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="982ab-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="982ab-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="982ab-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="982ab-130">See also</span></span>

- [<span data-ttu-id="982ab-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="982ab-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

