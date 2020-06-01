---
title: Enfants (ArrayOfStringArrayAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d37b3fd5-63f1-4003-a6ec-54adfce23d52
description: L’élément Children spécifie un tableau de noms et d’identificateurs enfants de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: f4217f8a444bfdb6d86ff7b912294cfad9cbdcdc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460231"
---
# <a name="children-arrayofstringarrayattributedvaluestype"></a><span data-ttu-id="d8994-103">Enfants (ArrayOfStringArrayAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="d8994-103">Children (ArrayOfStringArrayAttributedValuesType)</span></span>

<span data-ttu-id="d8994-104">L’élément **Children** spécifie un tableau de noms et d’identificateurs enfants de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="d8994-104">The **Children** element specifies an array of child names and identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Children>
    <StringAttributedValue></StringAttributedValue>
</Children>
```

 <span data-ttu-id="d8994-105">**ArrayOfStringArrayAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="d8994-105">**ArrayOfStringArrayAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8994-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d8994-106">Attributes and elements</span></span>

<span data-ttu-id="d8994-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d8994-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8994-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d8994-108">Attributes</span></span>

<span data-ttu-id="d8994-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d8994-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8994-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d8994-110">Child elements</span></span>

|<span data-ttu-id="d8994-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d8994-111">**Element**</span></span>|<span data-ttu-id="d8994-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d8994-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8994-113">StringArrayAttributedValue</span><span class="sxs-lookup"><span data-stu-id="d8994-113">StringArrayAttributedValue</span></span>](stringarrayattributedvalue.md) <br/> |<span data-ttu-id="d8994-114">Spécifie une instance d’un tableau de données de type chaîne pour un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="d8994-114">Specifies an instance of an array of string data for a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8994-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d8994-115">Parent elements</span></span>

|<span data-ttu-id="d8994-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d8994-116">**Element**</span></span>|<span data-ttu-id="d8994-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d8994-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8994-118">Persona</span><span class="sxs-lookup"><span data-stu-id="d8994-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="d8994-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="d8994-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d8994-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="d8994-120">Remarks</span></span>

<span data-ttu-id="d8994-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d8994-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d8994-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8994-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8994-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d8994-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8994-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d8994-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8994-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d8994-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d8994-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="d8994-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d8994-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="d8994-127">Validation File</span></span>  <br/> |<span data-ttu-id="d8994-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="d8994-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8994-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d8994-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d8994-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d8994-130">See also</span></span>



- [<span data-ttu-id="d8994-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d8994-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

