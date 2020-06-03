---
title: BusinessPhoneNumbers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ecbe4f1c-1c9e-44e0-a8f7-08c160a0fddb
description: L’élément BusinessPhoneNumbers spécifie un tableau de numéros de téléphone professionnels et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: 8713af3ad302a2940cab247ff7188e55e8021ca0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461617"
---
# <a name="businessphonenumbers"></a><span data-ttu-id="7fe76-103">BusinessPhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="7fe76-103">BusinessPhoneNumbers</span></span>

<span data-ttu-id="7fe76-104">L’élément **BusinessPhoneNumbers** spécifie un tableau de numéros de téléphone professionnels et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="7fe76-104">The **BusinessPhoneNumbers** element specifies an array of business phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessPhoneNumbers>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers>
```

 <span data-ttu-id="7fe76-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="7fe76-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7fe76-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7fe76-106">Attributes and elements</span></span>

<span data-ttu-id="7fe76-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7fe76-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7fe76-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7fe76-108">Attributes</span></span>

<span data-ttu-id="7fe76-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7fe76-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7fe76-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7fe76-110">Child elements</span></span>

|<span data-ttu-id="7fe76-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7fe76-111">**Element**</span></span>|<span data-ttu-id="7fe76-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7fe76-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7fe76-113">Valeur (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="7fe76-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="7fe76-114">Spécifie un numéro de téléphone et des informations de type et est associé à un ensemble d’attributions.</span><span class="sxs-lookup"><span data-stu-id="7fe76-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="7fe76-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="7fe76-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="7fe76-116">Spécifie un tableau des attributions de l’élément **value** associé.</span><span class="sxs-lookup"><span data-stu-id="7fe76-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7fe76-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7fe76-117">Parent elements</span></span>

|<span data-ttu-id="7fe76-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7fe76-118">**Element**</span></span>|<span data-ttu-id="7fe76-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="7fe76-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7fe76-120">Persona</span><span class="sxs-lookup"><span data-stu-id="7fe76-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="7fe76-121">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="7fe76-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7fe76-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="7fe76-122">Remarks</span></span>

<span data-ttu-id="7fe76-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7fe76-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7fe76-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7fe76-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7fe76-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7fe76-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7fe76-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7fe76-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7fe76-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7fe76-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7fe76-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="7fe76-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="7fe76-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="7fe76-129">Validation File</span></span>  <br/> |<span data-ttu-id="7fe76-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="7fe76-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7fe76-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7fe76-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7fe76-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7fe76-132">See also</span></span>



- [<span data-ttu-id="7fe76-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7fe76-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

