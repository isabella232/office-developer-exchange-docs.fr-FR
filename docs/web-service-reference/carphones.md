---
title: CarPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ad096246-113c-42ea-9e63-861b546003e8
description: L’élément CarPhone spécifie un tableau de numéros de téléphone de voiture et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: 41d0cc264da69ab17b8ebf109759139c4249719e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462226"
---
# <a name="carphones"></a><span data-ttu-id="746d0-103">CarPhones</span><span class="sxs-lookup"><span data-stu-id="746d0-103">CarPhones</span></span>

<span data-ttu-id="746d0-104">L’élément **CarPhone** spécifie un tableau de numéros de téléphone de voiture et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="746d0-104">The **CarPhone** element specifies an array of car phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CarPhones>
    <Value></Value>
    <Attributions></Attributions>
</CarPhones>
```

 <span data-ttu-id="746d0-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="746d0-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="746d0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="746d0-106">Attributes and elements</span></span>

<span data-ttu-id="746d0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="746d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="746d0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="746d0-108">Attributes</span></span>

<span data-ttu-id="746d0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="746d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="746d0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="746d0-110">Child elements</span></span>

|<span data-ttu-id="746d0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="746d0-111">**Element**</span></span>|<span data-ttu-id="746d0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="746d0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="746d0-113">Valeur (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="746d0-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="746d0-114">Spécifie un numéro de téléphone et des informations de type et est associé à un ensemble d’attributions.</span><span class="sxs-lookup"><span data-stu-id="746d0-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="746d0-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="746d0-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="746d0-116">Spécifie un tableau des attributions de l’élément **value** associé.</span><span class="sxs-lookup"><span data-stu-id="746d0-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="746d0-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="746d0-117">Parent elements</span></span>

|<span data-ttu-id="746d0-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="746d0-118">**Element**</span></span>|<span data-ttu-id="746d0-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="746d0-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="746d0-120">Persona</span><span class="sxs-lookup"><span data-stu-id="746d0-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="746d0-121">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="746d0-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="746d0-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="746d0-122">Remarks</span></span>

<span data-ttu-id="746d0-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="746d0-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="746d0-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="746d0-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="746d0-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="746d0-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="746d0-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="746d0-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="746d0-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="746d0-127">Schema Name</span></span>  <br/> |<span data-ttu-id="746d0-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="746d0-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="746d0-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="746d0-129">Validation File</span></span>  <br/> |<span data-ttu-id="746d0-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="746d0-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="746d0-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="746d0-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="746d0-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="746d0-132">See also</span></span>



- [<span data-ttu-id="746d0-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="746d0-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

