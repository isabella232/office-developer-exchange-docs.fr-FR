---
title: CallbackPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a7c1377-aac3-42c5-820f-d01cd8e9cf5c
description: L’élément CallbackPhones spécifie un tableau de numéros de téléphone de rappel et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: 79d74beffb8de8981e042b0c80e1aa5505a1048c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529461"
---
# <a name="callbackphones"></a><span data-ttu-id="0f745-103">CallbackPhones</span><span class="sxs-lookup"><span data-stu-id="0f745-103">CallbackPhones</span></span>

<span data-ttu-id="0f745-104">L’élément **CallbackPhones** spécifie un tableau de numéros de téléphone de rappel et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="0f745-104">The **CallbackPhones** element specifies an array of call-back phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CallbackPhones>
    <Value></Value>
    <Attributions></Attributions>
</CallbackPhones>
```

 <span data-ttu-id="0f745-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="0f745-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f745-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0f745-106">Attributes and elements</span></span>

<span data-ttu-id="0f745-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0f745-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f745-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0f745-108">Attributes</span></span>

<span data-ttu-id="0f745-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0f745-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f745-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0f745-110">Child elements</span></span>

|<span data-ttu-id="0f745-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f745-111">**Element**</span></span>|<span data-ttu-id="0f745-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f745-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f745-113">Valeur (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="0f745-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="0f745-114">Spécifie un numéro de téléphone et des informations de type et est associé à un ensemble d’attributions.</span><span class="sxs-lookup"><span data-stu-id="0f745-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="0f745-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="0f745-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="0f745-116">Spécifie un tableau des attributions de l’élément **value** associé.</span><span class="sxs-lookup"><span data-stu-id="0f745-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f745-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0f745-117">Parent elements</span></span>

|<span data-ttu-id="0f745-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f745-118">**Element**</span></span>|<span data-ttu-id="0f745-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f745-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f745-120">Persona</span><span class="sxs-lookup"><span data-stu-id="0f745-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="0f745-121">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="0f745-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0f745-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="0f745-122">Remarks</span></span>

<span data-ttu-id="0f745-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0f745-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0f745-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f745-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f745-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0f745-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f745-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0f745-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f745-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0f745-127">Schema Name</span></span>  <br/> |<span data-ttu-id="0f745-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="0f745-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="0f745-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="0f745-129">Validation File</span></span>  <br/> |<span data-ttu-id="0f745-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="0f745-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f745-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0f745-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0f745-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0f745-132">See also</span></span>



- [<span data-ttu-id="0f745-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0f745-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

