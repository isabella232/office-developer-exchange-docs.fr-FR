---
title: HomeAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 57fb1b9d-2ba8-4359-ae79-35c0d56a2d0f
description: L’élément HomeAddresses spécifie un tableau d’adresses personnelles et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: d6a1808bf000ac8bca1e2ce7865aa099037c5a5d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460889"
---
# <a name="homeaddresses"></a><span data-ttu-id="a2fb4-103">HomeAddresses</span><span class="sxs-lookup"><span data-stu-id="a2fb4-103">HomeAddresses</span></span>

<span data-ttu-id="a2fb4-104">L’élément **HomeAddresses** spécifie un tableau d’adresses personnelles et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="a2fb4-104">The **HomeAddresses** element specifies an array of home addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeAddresses>
    <PostalAddressAttributedValue/>
</HomeAddresses>
```

 <span data-ttu-id="a2fb4-105">**ArrayOfPostalAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="a2fb4-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2fb4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a2fb4-106">Attributes and elements</span></span>

<span data-ttu-id="a2fb4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a2fb4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2fb4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a2fb4-108">Attributes</span></span>

<span data-ttu-id="a2fb4-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a2fb4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2fb4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a2fb4-110">Child elements</span></span>

|<span data-ttu-id="a2fb4-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2fb4-111">**Element**</span></span>|<span data-ttu-id="a2fb4-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2fb4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2fb4-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="a2fb4-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="a2fb4-114">Spécifie une instance d’un tableau d’adresses postales et leurs attributions associées.</span><span class="sxs-lookup"><span data-stu-id="a2fb4-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2fb4-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a2fb4-115">Parent elements</span></span>

|<span data-ttu-id="a2fb4-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2fb4-116">**Element**</span></span>|<span data-ttu-id="a2fb4-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2fb4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2fb4-118">Persona</span><span class="sxs-lookup"><span data-stu-id="a2fb4-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="a2fb4-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="a2fb4-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2fb4-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="a2fb4-120">Remarks</span></span>

<span data-ttu-id="a2fb4-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a2fb4-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a2fb4-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2fb4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2fb4-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a2fb4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2fb4-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a2fb4-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2fb4-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a2fb4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a2fb4-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="a2fb4-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="a2fb4-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="a2fb4-127">Validation File</span></span>  <br/> |<span data-ttu-id="a2fb4-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="a2fb4-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2fb4-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a2fb4-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a2fb4-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a2fb4-130">See also</span></span>



- [<span data-ttu-id="a2fb4-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a2fb4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

