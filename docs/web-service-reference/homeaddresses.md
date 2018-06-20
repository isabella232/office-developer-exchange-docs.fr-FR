---
title: HomeAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 57fb1b9d-2ba8-4359-ae79-35c0d56a2d0f
description: L’élément HomeAddresses spécifie un tableau d’adresses personnel et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: a9d4ceafcac9cf0809668871b4df932b31525ac8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827817"
---
# <a name="homeaddresses"></a><span data-ttu-id="dbf15-103">HomeAddresses</span><span class="sxs-lookup"><span data-stu-id="dbf15-103">HomeAddresses</span></span>

<span data-ttu-id="dbf15-104">L’élément **HomeAddresses** spécifie un tableau d’adresses personnel et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="dbf15-104">The **HomeAddresses** element specifies an array of home addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeAddresses>
    <PostalAddressAttributedValue/>
</HomeAddresses>
```

 <span data-ttu-id="dbf15-105">**ArrayOfPostalAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="dbf15-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dbf15-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dbf15-106">Attributes and elements</span></span>

<span data-ttu-id="dbf15-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dbf15-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbf15-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="dbf15-108">Attributes</span></span>

<span data-ttu-id="dbf15-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dbf15-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dbf15-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dbf15-110">Child elements</span></span>

|<span data-ttu-id="dbf15-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dbf15-111">**Element**</span></span>|<span data-ttu-id="dbf15-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="dbf15-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbf15-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="dbf15-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="dbf15-114">Spécifie une instance d’un tableau d’adresses postales et leurs attributions associées.</span><span class="sxs-lookup"><span data-stu-id="dbf15-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dbf15-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dbf15-115">Parent elements</span></span>

|<span data-ttu-id="dbf15-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dbf15-116">**Element**</span></span>|<span data-ttu-id="dbf15-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="dbf15-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbf15-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="dbf15-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="dbf15-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="dbf15-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dbf15-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="dbf15-120">Remarks</span></span>

<span data-ttu-id="dbf15-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="dbf15-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dbf15-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="dbf15-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbf15-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dbf15-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbf15-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dbf15-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dbf15-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dbf15-125">Schema Name</span></span>  <br/> |<span data-ttu-id="dbf15-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="dbf15-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="dbf15-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="dbf15-127">Validation File</span></span>  <br/> |<span data-ttu-id="dbf15-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="dbf15-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="dbf15-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dbf15-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="dbf15-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dbf15-130">See also</span></span>



- [<span data-ttu-id="dbf15-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dbf15-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
