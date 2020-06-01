---
title: FileAses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81efc37-bb70-4d52-a614-cec87d1b0f04
description: L’élément FileAses spécifie un tableau d’éléments StringAttributedValue et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: 9d97c2c7210e9ae20326d7327c9de4159d5df5a6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461078"
---
# <a name="fileases"></a><span data-ttu-id="b1ebe-103">FileAses</span><span class="sxs-lookup"><span data-stu-id="b1ebe-103">FileAses</span></span>

<span data-ttu-id="b1ebe-104">L’élément **FileAses** spécifie un tableau d’éléments **StringAttributedValue** et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="b1ebe-104">The **FileAses** element specifies an array of **StringAttributedValue** elements and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<FileAses>
    <StringAttributedValue/>
</FileAses>
```

 <span data-ttu-id="b1ebe-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="b1ebe-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1ebe-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b1ebe-106">Attributes and elements</span></span>

<span data-ttu-id="b1ebe-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b1ebe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1ebe-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b1ebe-108">Attributes</span></span>

<span data-ttu-id="b1ebe-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b1ebe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b1ebe-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b1ebe-110">Child elements</span></span>

|<span data-ttu-id="b1ebe-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b1ebe-111">**Element**</span></span>|<span data-ttu-id="b1ebe-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b1ebe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1ebe-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="b1ebe-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="b1ebe-114">Spécifie une instance dans un tableau d’attributs associés à un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="b1ebe-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b1ebe-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b1ebe-115">Parent elements</span></span>

|<span data-ttu-id="b1ebe-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b1ebe-116">**Element**</span></span>|<span data-ttu-id="b1ebe-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b1ebe-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1ebe-118">Persona</span><span class="sxs-lookup"><span data-stu-id="b1ebe-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="b1ebe-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="b1ebe-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b1ebe-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="b1ebe-120">Remarks</span></span>

<span data-ttu-id="b1ebe-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b1ebe-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b1ebe-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b1ebe-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b1ebe-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b1ebe-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1ebe-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b1ebe-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b1ebe-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b1ebe-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b1ebe-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="b1ebe-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b1ebe-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="b1ebe-127">Validation File</span></span>  <br/> |<span data-ttu-id="b1ebe-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="b1ebe-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b1ebe-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b1ebe-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b1ebe-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b1ebe-130">See also</span></span>



- [<span data-ttu-id="b1ebe-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b1ebe-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

