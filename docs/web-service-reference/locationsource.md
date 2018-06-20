---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: L’élément LocationSource spécifie des informations sur l’origine de l’adresse postale associée, par exemple, un contact ou un annuaire téléphonique.
ms.openlocfilehash: 7f5cf5fcca0a72287593349fcf5090a74225d012
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828248"
---
# <a name="locationsource"></a><span data-ttu-id="30cd7-103">LocationSource</span><span class="sxs-lookup"><span data-stu-id="30cd7-103">LocationSource</span></span>

<span data-ttu-id="30cd7-104">L’élément **LocationSource** spécifie des informations sur l’origine de l’adresse postale associée, par exemple, un contact ou un annuaire téléphonique.</span><span class="sxs-lookup"><span data-stu-id="30cd7-104">The **LocationSource** element specifies information about the origin of the associated postal address, for example, a contact or a telephone book.</span></span> 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 <span data-ttu-id="30cd7-105">**LocationSourceType**</span><span class="sxs-lookup"><span data-stu-id="30cd7-105">**LocationSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30cd7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="30cd7-106">Attributes and elements</span></span>

<span data-ttu-id="30cd7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="30cd7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30cd7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="30cd7-108">Attributes</span></span>

<span data-ttu-id="30cd7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="30cd7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30cd7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="30cd7-110">Child elements</span></span>

<span data-ttu-id="30cd7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="30cd7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="30cd7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="30cd7-112">Parent elements</span></span>

<span data-ttu-id="30cd7-113">[Valeur (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span><span class="sxs-lookup"><span data-stu-id="30cd7-113">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="30cd7-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="30cd7-114">Text value</span></span>

<span data-ttu-id="30cd7-115">Les valeurs de texte de l’élément **LocationSource** sont répertoriées dans le tableau suivant :</span><span class="sxs-lookup"><span data-stu-id="30cd7-115">The text values for the **LocationSource** element are listed in the following table:</span></span> 
  
<span data-ttu-id="30cd7-116">**Valeurs de texte des éléments LocationSource**</span><span class="sxs-lookup"><span data-stu-id="30cd7-116">**LocationSource element text values**</span></span>

|<span data-ttu-id="30cd7-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="30cd7-117">**Value**</span></span>|<span data-ttu-id="30cd7-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="30cd7-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="30cd7-119">None</span><span class="sxs-lookup"><span data-stu-id="30cd7-119">None</span></span>  <br/> |<span data-ttu-id="30cd7-120">Il n’existe aucune source d’emplacement.</span><span class="sxs-lookup"><span data-stu-id="30cd7-120">There is no location source.</span></span>  <br/> |
|<span data-ttu-id="30cd7-121">LocationServices</span><span class="sxs-lookup"><span data-stu-id="30cd7-121">LocationServices</span></span>  <br/> |<span data-ttu-id="30cd7-122">Les informations a été obtenues à partir des services de localisation.</span><span class="sxs-lookup"><span data-stu-id="30cd7-122">The information was obtained from location services.</span></span>  <br/> |
|<span data-ttu-id="30cd7-123">PhonebookServices</span><span class="sxs-lookup"><span data-stu-id="30cd7-123">PhonebookServices</span></span>  <br/> |<span data-ttu-id="30cd7-124">Les informations ont été obtenues à partir des services d’annuaire.</span><span class="sxs-lookup"><span data-stu-id="30cd7-124">The information was obtained from phonebook services.</span></span>  <br/> |
|<span data-ttu-id="30cd7-125">Appareil</span><span class="sxs-lookup"><span data-stu-id="30cd7-125">Device</span></span>  <br/> |<span data-ttu-id="30cd7-126">Les informations a été obtenues à partir du périphérique.</span><span class="sxs-lookup"><span data-stu-id="30cd7-126">The information was obtained from the device.</span></span>  <br/> |
|<span data-ttu-id="30cd7-127">Contact</span><span class="sxs-lookup"><span data-stu-id="30cd7-127">Contact</span></span>  <br/> |<span data-ttu-id="30cd7-128">Les informations ont été obtenues à partir d’un contact.</span><span class="sxs-lookup"><span data-stu-id="30cd7-128">The information was obtained from a contact.</span></span>  <br/> |
|<span data-ttu-id="30cd7-129">Ressource</span><span class="sxs-lookup"><span data-stu-id="30cd7-129">Resource</span></span>  <br/> |<span data-ttu-id="30cd7-130">Les informations ont été obtenues à partir d’une ressource.</span><span class="sxs-lookup"><span data-stu-id="30cd7-130">The information was obtained from a resource.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="30cd7-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="30cd7-131">Remarks</span></span>

<span data-ttu-id="30cd7-132">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="30cd7-132">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="30cd7-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="30cd7-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

