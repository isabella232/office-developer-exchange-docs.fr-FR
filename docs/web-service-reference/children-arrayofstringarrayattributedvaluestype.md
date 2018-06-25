---
title: Enfants (ArrayOfStringArrayAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d37b3fd5-63f1-4003-a6ec-54adfce23d52
description: L’élément enfant spécifie un tableau de noms enfants et les identificateurs des attributions de leur source pour le personnage associé.
ms.openlocfilehash: 7c98e7cb96cecad0d1b5122236b6cd0947c6b3d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755505"
---
# <a name="children-arrayofstringarrayattributedvaluestype"></a><span data-ttu-id="36c18-103">Enfants (ArrayOfStringArrayAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="36c18-103">Children (ArrayOfStringArrayAttributedValuesType)</span></span>

<span data-ttu-id="36c18-104">L’élément **enfant** spécifie un tableau de noms enfants et les identificateurs des attributions de leur source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="36c18-104">The **Children** element specifies an array of child names and identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Children>
    <StringAttributedValue></StringAttributedValue>
</Children>
```

 <span data-ttu-id="36c18-105">**ArrayOfStringArrayAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="36c18-105">**ArrayOfStringArrayAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36c18-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="36c18-106">Attributes and elements</span></span>

<span data-ttu-id="36c18-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="36c18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36c18-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="36c18-108">Attributes</span></span>

<span data-ttu-id="36c18-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="36c18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36c18-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="36c18-110">Child elements</span></span>

|<span data-ttu-id="36c18-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="36c18-111">**Element**</span></span>|<span data-ttu-id="36c18-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="36c18-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36c18-113">StringArrayAttributedValue</span><span class="sxs-lookup"><span data-stu-id="36c18-113">StringArrayAttributedValue</span></span>](stringarrayattributedvalue.md) <br/> |<span data-ttu-id="36c18-114">Spécifie une instance d’un tableau de données de chaîne d’un élément personnage.</span><span class="sxs-lookup"><span data-stu-id="36c18-114">Specifies an instance of an array of string data for a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="36c18-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="36c18-115">Parent elements</span></span>

|<span data-ttu-id="36c18-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="36c18-116">**Element**</span></span>|<span data-ttu-id="36c18-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="36c18-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36c18-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="36c18-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="36c18-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="36c18-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="36c18-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="36c18-120">Remarks</span></span>

<span data-ttu-id="36c18-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="36c18-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="36c18-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="36c18-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36c18-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="36c18-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36c18-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="36c18-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36c18-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="36c18-125">Schema Name</span></span>  <br/> |<span data-ttu-id="36c18-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="36c18-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="36c18-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="36c18-127">Validation File</span></span>  <br/> |<span data-ttu-id="36c18-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="36c18-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="36c18-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="36c18-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="36c18-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="36c18-130">See also</span></span>



- [<span data-ttu-id="36c18-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="36c18-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

