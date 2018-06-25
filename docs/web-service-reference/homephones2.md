---
title: HomePhones2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ba9bb159-362d-48e0-889d-823cb46ecebf
description: L’élément HomePhones2 spécifie un tableau de valeurs HomePhone2 et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: 205f2f71421a0dfc7d0057412529bcefdb6636d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827842"
---
# <a name="homephones2"></a><span data-ttu-id="44d71-103">HomePhones2</span><span class="sxs-lookup"><span data-stu-id="44d71-103">HomePhones2</span></span>

<span data-ttu-id="44d71-104">L’élément **HomePhones2** spécifie un tableau de valeurs **HomePhone2** et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="44d71-104">The **HomePhones2** element specifies an array of **HomePhone2** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones2>
    <PhoneNumberAttributedValue/>
</HomePhones2>
```

 <span data-ttu-id="44d71-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="44d71-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44d71-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="44d71-106">Attributes and elements</span></span>

<span data-ttu-id="44d71-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="44d71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44d71-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="44d71-108">Attributes</span></span>

<span data-ttu-id="44d71-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="44d71-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44d71-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="44d71-110">Child elements</span></span>

|<span data-ttu-id="44d71-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="44d71-111">**Element**</span></span>|<span data-ttu-id="44d71-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="44d71-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44d71-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="44d71-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="44d71-114">Contient un numéro de téléphone attribué unique un personnage.</span><span class="sxs-lookup"><span data-stu-id="44d71-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="44d71-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="44d71-115">Parent elements</span></span>

|<span data-ttu-id="44d71-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="44d71-116">**Element**</span></span>|<span data-ttu-id="44d71-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="44d71-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44d71-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="44d71-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="44d71-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="44d71-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="44d71-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="44d71-120">Remarks</span></span>

<span data-ttu-id="44d71-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="44d71-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="44d71-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="44d71-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44d71-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="44d71-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44d71-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="44d71-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="44d71-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="44d71-125">Schema Name</span></span>  <br/> |<span data-ttu-id="44d71-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="44d71-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="44d71-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="44d71-127">Validation File</span></span>  <br/> |<span data-ttu-id="44d71-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="44d71-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="44d71-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="44d71-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="44d71-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="44d71-130">See also</span></span>



- [<span data-ttu-id="44d71-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="44d71-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

