---
title: BusinessPhoneNumbers2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f335ea74-9b5b-4224-9475-40ef33fe76bd
description: L’élément BusinessPhoneNumbers2 spécifie un tableau d’éléments BusinessPhoneNumber2 et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: 8a03e102223e5542d6a672c4f47305cef84b850b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19755466"
---
# <a name="businessphonenumbers2"></a><span data-ttu-id="bb14b-103">BusinessPhoneNumbers2</span><span class="sxs-lookup"><span data-stu-id="bb14b-103">BusinessPhoneNumbers2</span></span>

<span data-ttu-id="bb14b-104">L’élément **BusinessPhoneNumbers2** spécifie un tableau d’éléments **BusinessPhoneNumber2** et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="bb14b-104">The **BusinessPhoneNumbers2** element specifies an array of **BusinessPhoneNumber2** elements and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessPhoneNumbers2>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers2>
```

 <span data-ttu-id="bb14b-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="bb14b-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb14b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bb14b-106">Attributes and elements</span></span>

<span data-ttu-id="bb14b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bb14b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb14b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bb14b-108">Attributes</span></span>

<span data-ttu-id="bb14b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bb14b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb14b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bb14b-110">Child elements</span></span>

|<span data-ttu-id="bb14b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bb14b-111">**Element**</span></span>|<span data-ttu-id="bb14b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="bb14b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb14b-113">Valeur (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="bb14b-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="bb14b-114">Spécifie un nombre et le type d’informations téléphoniques et est associé à un ensemble d’attributions.</span><span class="sxs-lookup"><span data-stu-id="bb14b-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="bb14b-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="bb14b-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="bb14b-116">Spécifie un tableau des affectations pour sa **valeur** de l’élément associé.</span><span class="sxs-lookup"><span data-stu-id="bb14b-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bb14b-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bb14b-117">Parent elements</span></span>

|<span data-ttu-id="bb14b-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bb14b-118">**Element**</span></span>|<span data-ttu-id="bb14b-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="bb14b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb14b-120">Personnage</span><span class="sxs-lookup"><span data-stu-id="bb14b-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="bb14b-121">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="bb14b-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bb14b-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="bb14b-122">Remarks</span></span>

<span data-ttu-id="bb14b-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bb14b-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bb14b-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb14b-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb14b-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bb14b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb14b-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bb14b-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bb14b-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bb14b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="bb14b-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="bb14b-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="bb14b-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="bb14b-129">Validation File</span></span>  <br/> |<span data-ttu-id="bb14b-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="bb14b-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bb14b-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bb14b-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bb14b-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bb14b-132">See also</span></span>



- [<span data-ttu-id="bb14b-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bb14b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

