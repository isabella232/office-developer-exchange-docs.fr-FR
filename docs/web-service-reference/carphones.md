---
title: CarPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ad096246-113c-42ea-9e63-861b546003e8
description: L’élément de téléphone de voiture spécifie un tableau des numéros de téléphone de voiture et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: 694b3578e127a84dfd2fb844c6e81b28553b687c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755494"
---
# <a name="carphones"></a><span data-ttu-id="e2ad1-103">CarPhones</span><span class="sxs-lookup"><span data-stu-id="e2ad1-103">CarPhones</span></span>

<span data-ttu-id="e2ad1-104">L’élément de **téléphone de voiture** spécifie un tableau des numéros de téléphone de voiture et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="e2ad1-104">The **CarPhone** element specifies an array of car phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CarPhones>
    <Value></Value>
    <Attributions></Attributions>
</CarPhones>
```

 <span data-ttu-id="e2ad1-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="e2ad1-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2ad1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e2ad1-106">Attributes and elements</span></span>

<span data-ttu-id="e2ad1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e2ad1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2ad1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e2ad1-108">Attributes</span></span>

<span data-ttu-id="e2ad1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e2ad1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2ad1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e2ad1-110">Child elements</span></span>

|<span data-ttu-id="e2ad1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e2ad1-111">**Element**</span></span>|<span data-ttu-id="e2ad1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e2ad1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2ad1-113">Valeur (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="e2ad1-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="e2ad1-114">Spécifie un nombre et le type d’informations téléphoniques et est associé à un ensemble d’attributions.</span><span class="sxs-lookup"><span data-stu-id="e2ad1-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="e2ad1-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="e2ad1-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="e2ad1-116">Spécifie un tableau des affectations pour sa **valeur** de l’élément associé.</span><span class="sxs-lookup"><span data-stu-id="e2ad1-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2ad1-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e2ad1-117">Parent elements</span></span>

|<span data-ttu-id="e2ad1-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e2ad1-118">**Element**</span></span>|<span data-ttu-id="e2ad1-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="e2ad1-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2ad1-120">Personnage</span><span class="sxs-lookup"><span data-stu-id="e2ad1-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="e2ad1-121">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="e2ad1-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e2ad1-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="e2ad1-122">Remarks</span></span>

<span data-ttu-id="e2ad1-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e2ad1-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e2ad1-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2ad1-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2ad1-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e2ad1-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2ad1-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e2ad1-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2ad1-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e2ad1-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e2ad1-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="e2ad1-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="e2ad1-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="e2ad1-129">Validation File</span></span>  <br/> |<span data-ttu-id="e2ad1-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="e2ad1-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2ad1-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e2ad1-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e2ad1-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e2ad1-132">See also</span></span>



- [<span data-ttu-id="e2ad1-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e2ad1-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

