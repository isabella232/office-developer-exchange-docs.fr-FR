---
title: BusinessPhoneNumbers2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f335ea74-9b5b-4224-9475-40ef33fe76bd
description: L’élément BusinessPhoneNumbers2 spécifie un tableau d’éléments BusinessPhoneNumber2 et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: c8879e3f7ab996d7e761a72b7ce5f332a9006aed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461603"
---
# <a name="businessphonenumbers2"></a><span data-ttu-id="7b674-103">BusinessPhoneNumbers2</span><span class="sxs-lookup"><span data-stu-id="7b674-103">BusinessPhoneNumbers2</span></span>

<span data-ttu-id="7b674-104">L’élément **BusinessPhoneNumbers2** spécifie un tableau d’éléments **BusinessPhoneNumber2** et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="7b674-104">The **BusinessPhoneNumbers2** element specifies an array of **BusinessPhoneNumber2** elements and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessPhoneNumbers2>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers2>
```

 <span data-ttu-id="7b674-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="7b674-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b674-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7b674-106">Attributes and elements</span></span>

<span data-ttu-id="7b674-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7b674-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b674-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7b674-108">Attributes</span></span>

<span data-ttu-id="7b674-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7b674-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b674-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7b674-110">Child elements</span></span>

|<span data-ttu-id="7b674-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7b674-111">**Element**</span></span>|<span data-ttu-id="7b674-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7b674-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b674-113">Valeur (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="7b674-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="7b674-114">Spécifie un numéro de téléphone et des informations de type et est associé à un ensemble d’attributions.</span><span class="sxs-lookup"><span data-stu-id="7b674-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="7b674-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="7b674-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="7b674-116">Spécifie un tableau des attributions de l’élément **value** associé.</span><span class="sxs-lookup"><span data-stu-id="7b674-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7b674-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7b674-117">Parent elements</span></span>

|<span data-ttu-id="7b674-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7b674-118">**Element**</span></span>|<span data-ttu-id="7b674-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="7b674-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b674-120">Persona</span><span class="sxs-lookup"><span data-stu-id="7b674-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="7b674-121">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="7b674-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7b674-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="7b674-122">Remarks</span></span>

<span data-ttu-id="7b674-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7b674-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7b674-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b674-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b674-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7b674-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b674-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7b674-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7b674-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7b674-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7b674-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="7b674-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="7b674-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="7b674-129">Validation File</span></span>  <br/> |<span data-ttu-id="7b674-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="7b674-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7b674-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7b674-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7b674-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7b674-132">See also</span></span>



- [<span data-ttu-id="7b674-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7b674-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

