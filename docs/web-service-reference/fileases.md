---
title: FileAses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81efc37-bb70-4d52-a614-cec87d1b0f04
description: L’élément FileAses spécifie un tableau d’éléments StringAttributedValue et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: e660c74135dca9a2eb58b3486e0d2e19f85e012f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19756358"
---
# <a name="fileases"></a><span data-ttu-id="673d6-103">FileAses</span><span class="sxs-lookup"><span data-stu-id="673d6-103">FileAses</span></span>

<span data-ttu-id="673d6-104">L’élément **FileAses** spécifie un tableau d’éléments **StringAttributedValue** et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="673d6-104">The **FileAses** element specifies an array of **StringAttributedValue** elements and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<FileAses>
    <StringAttributedValue/>
</FileAses>
```

 <span data-ttu-id="673d6-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="673d6-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="673d6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="673d6-106">Attributes and elements</span></span>

<span data-ttu-id="673d6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="673d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="673d6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="673d6-108">Attributes</span></span>

<span data-ttu-id="673d6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="673d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="673d6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="673d6-110">Child elements</span></span>

|<span data-ttu-id="673d6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="673d6-111">**Element**</span></span>|<span data-ttu-id="673d6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="673d6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="673d6-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="673d6-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="673d6-114">Spécifie une instance d’un tableau d’attributs associés à un élément personnage.</span><span class="sxs-lookup"><span data-stu-id="673d6-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="673d6-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="673d6-115">Parent elements</span></span>

|<span data-ttu-id="673d6-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="673d6-116">**Element**</span></span>|<span data-ttu-id="673d6-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="673d6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="673d6-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="673d6-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="673d6-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="673d6-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="673d6-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="673d6-120">Remarks</span></span>

<span data-ttu-id="673d6-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="673d6-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="673d6-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="673d6-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="673d6-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="673d6-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="673d6-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="673d6-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="673d6-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="673d6-125">Schema Name</span></span>  <br/> |<span data-ttu-id="673d6-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="673d6-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="673d6-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="673d6-127">Validation File</span></span>  <br/> |<span data-ttu-id="673d6-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="673d6-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="673d6-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="673d6-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="673d6-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="673d6-130">See also</span></span>



- [<span data-ttu-id="673d6-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="673d6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

