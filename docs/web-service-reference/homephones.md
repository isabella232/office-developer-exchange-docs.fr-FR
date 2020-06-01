---
title: HomePhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ea43d5a-4bcf-497e-a559-6efe94fa604b
description: L’élément HomePhones spécifie un tableau de numéros de téléphone personnels et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: b55d6ca752a5b00a27eb158c6a22412a9f4ecdda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460833"
---
# <a name="homephones"></a><span data-ttu-id="b21ba-103">HomePhones</span><span class="sxs-lookup"><span data-stu-id="b21ba-103">HomePhones</span></span>

<span data-ttu-id="b21ba-104">L’élément **HomePhones** spécifie un tableau de numéros de téléphone personnels et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="b21ba-104">The **HomePhones** element specifies an array of home phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones>
    <PhoneNumberAttributedValue/>
</HomePhones>
```

 <span data-ttu-id="b21ba-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="b21ba-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b21ba-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b21ba-106">Attributes and elements</span></span>

<span data-ttu-id="b21ba-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b21ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b21ba-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b21ba-108">Attributes</span></span>

<span data-ttu-id="b21ba-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b21ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b21ba-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b21ba-110">Child elements</span></span>

|<span data-ttu-id="b21ba-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b21ba-111">**Element**</span></span>|<span data-ttu-id="b21ba-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b21ba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b21ba-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="b21ba-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="b21ba-114">Contient un seul numéro de téléphone avec attributs pour un personnage.</span><span class="sxs-lookup"><span data-stu-id="b21ba-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b21ba-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b21ba-115">Parent elements</span></span>

|<span data-ttu-id="b21ba-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b21ba-116">**Element**</span></span>|<span data-ttu-id="b21ba-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b21ba-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b21ba-118">Persona</span><span class="sxs-lookup"><span data-stu-id="b21ba-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="b21ba-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="b21ba-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b21ba-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="b21ba-120">Remarks</span></span>

<span data-ttu-id="b21ba-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b21ba-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b21ba-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b21ba-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b21ba-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b21ba-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b21ba-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b21ba-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b21ba-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b21ba-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b21ba-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="b21ba-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b21ba-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="b21ba-127">Validation File</span></span>  <br/> |<span data-ttu-id="b21ba-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="b21ba-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b21ba-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b21ba-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b21ba-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b21ba-130">See also</span></span>



- [<span data-ttu-id="b21ba-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b21ba-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

