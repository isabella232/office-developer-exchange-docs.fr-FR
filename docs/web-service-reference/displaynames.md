---
title: DisplayName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dedd43c8-c1d6-4671-89c5-ce7ab3979fda
description: L’élément DisplayNames spécifie un tableau de noms d’affichage et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: 7d0c528b5b7f9adae271a42380550115fbcf94d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460735"
---
# <a name="displaynames"></a><span data-ttu-id="6e063-103">DisplayName</span><span class="sxs-lookup"><span data-stu-id="6e063-103">DisplayNames</span></span>

<span data-ttu-id="6e063-104">L’élément **DisplayNames** spécifie un tableau de noms d’affichage et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="6e063-104">The **DisplayNames** element specifies an array of display names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```xml
<DisplayNames>
    <StringAttributedValue></StringAttributedValue>
</DisplayNames>
```

 <span data-ttu-id="6e063-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="6e063-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e063-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6e063-106">Attributes and elements</span></span>

<span data-ttu-id="6e063-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6e063-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e063-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6e063-108">Attributes</span></span>

<span data-ttu-id="6e063-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="6e063-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e063-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6e063-110">Child elements</span></span>

|<span data-ttu-id="6e063-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6e063-111">**Element**</span></span>|<span data-ttu-id="6e063-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="6e063-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e063-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="6e063-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="6e063-114">Spécifie une instance dans un tableau d’attributs associés à un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="6e063-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e063-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6e063-115">Parent elements</span></span>

|<span data-ttu-id="6e063-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6e063-116">**Element**</span></span>|<span data-ttu-id="6e063-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="6e063-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e063-118">Persona</span><span class="sxs-lookup"><span data-stu-id="6e063-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="6e063-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="6e063-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6e063-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="6e063-120">Remarks</span></span>

<span data-ttu-id="6e063-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6e063-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6e063-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e063-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e063-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6e063-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e063-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6e063-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e063-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6e063-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6e063-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="6e063-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="6e063-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="6e063-127">Validation File</span></span>  <br/> |<span data-ttu-id="6e063-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="6e063-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e063-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6e063-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6e063-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6e063-130">See also</span></span>

- [<span data-ttu-id="6e063-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6e063-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

