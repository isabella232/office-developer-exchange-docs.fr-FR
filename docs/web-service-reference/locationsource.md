---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: L’élément LocationSource spécifie les informations relatives à l’origine de l’adresse postale associée, par exemple, un contact ou un annuaire téléphonique.
ms.openlocfilehash: ceba52c43d1c798bb8f5492b779c7c45d7d00b0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467101"
---
# <a name="locationsource"></a><span data-ttu-id="730a2-103">LocationSource</span><span class="sxs-lookup"><span data-stu-id="730a2-103">LocationSource</span></span>

<span data-ttu-id="730a2-104">L’élément **LocationSource** spécifie les informations relatives à l’origine de l’adresse postale associée, par exemple, un contact ou un annuaire téléphonique.</span><span class="sxs-lookup"><span data-stu-id="730a2-104">The **LocationSource** element specifies information about the origin of the associated postal address, for example, a contact or a telephone book.</span></span> 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 <span data-ttu-id="730a2-105">**LocationSourceType**</span><span class="sxs-lookup"><span data-stu-id="730a2-105">**LocationSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="730a2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="730a2-106">Attributes and elements</span></span>

<span data-ttu-id="730a2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="730a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="730a2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="730a2-108">Attributes</span></span>

<span data-ttu-id="730a2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="730a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="730a2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="730a2-110">Child elements</span></span>

<span data-ttu-id="730a2-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="730a2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="730a2-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="730a2-112">Parent elements</span></span>

<span data-ttu-id="730a2-113">[Valeur (PersonaPostalAddressType)](value-personapostaladdresstype.md)  |  [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span><span class="sxs-lookup"><span data-stu-id="730a2-113">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="730a2-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="730a2-114">Text value</span></span>

<span data-ttu-id="730a2-115">Les valeurs de texte de l’élément **LocationSource** sont répertoriées dans le tableau suivant :</span><span class="sxs-lookup"><span data-stu-id="730a2-115">The text values for the **LocationSource** element are listed in the following table:</span></span> 
  
<span data-ttu-id="730a2-116">**Valeurs de texte de l’élément LocationSource**</span><span class="sxs-lookup"><span data-stu-id="730a2-116">**LocationSource element text values**</span></span>

|<span data-ttu-id="730a2-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="730a2-117">**Value**</span></span>|<span data-ttu-id="730a2-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="730a2-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="730a2-119">Aucun</span><span class="sxs-lookup"><span data-stu-id="730a2-119">None</span></span>  <br/> |<span data-ttu-id="730a2-120">Il n’y a pas de source d’emplacement.</span><span class="sxs-lookup"><span data-stu-id="730a2-120">There is no location source.</span></span>  <br/> |
|<span data-ttu-id="730a2-121">LocationServices</span><span class="sxs-lookup"><span data-stu-id="730a2-121">LocationServices</span></span>  <br/> |<span data-ttu-id="730a2-122">Les informations proviennent des services de localisation.</span><span class="sxs-lookup"><span data-stu-id="730a2-122">The information was obtained from location services.</span></span>  <br/> |
|<span data-ttu-id="730a2-123">PhonebookServices</span><span class="sxs-lookup"><span data-stu-id="730a2-123">PhonebookServices</span></span>  <br/> |<span data-ttu-id="730a2-124">Les informations proviennent des services d’annuaire.</span><span class="sxs-lookup"><span data-stu-id="730a2-124">The information was obtained from phonebook services.</span></span>  <br/> |
|<span data-ttu-id="730a2-125">Device</span><span class="sxs-lookup"><span data-stu-id="730a2-125">Device</span></span>  <br/> |<span data-ttu-id="730a2-126">Les informations ont été obtenues à partir de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="730a2-126">The information was obtained from the device.</span></span>  <br/> |
|<span data-ttu-id="730a2-127">Contact</span><span class="sxs-lookup"><span data-stu-id="730a2-127">Contact</span></span>  <br/> |<span data-ttu-id="730a2-128">Les informations ont été obtenues à partir d’un contact.</span><span class="sxs-lookup"><span data-stu-id="730a2-128">The information was obtained from a contact.</span></span>  <br/> |
|<span data-ttu-id="730a2-129">Resource</span><span class="sxs-lookup"><span data-stu-id="730a2-129">Resource</span></span>  <br/> |<span data-ttu-id="730a2-130">Les informations ont été obtenues à partir d’une ressource.</span><span class="sxs-lookup"><span data-stu-id="730a2-130">The information was obtained from a resource.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="730a2-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="730a2-131">Remarks</span></span>

<span data-ttu-id="730a2-132">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="730a2-132">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="730a2-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="730a2-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

