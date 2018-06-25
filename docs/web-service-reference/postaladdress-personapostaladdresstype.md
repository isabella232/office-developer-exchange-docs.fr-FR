---
title: PostalAddress (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 075f7d65-9d05-47cb-af26-0dd6d5593439
description: L’élément PostalAddress Spécifie l’adresse postale pour un personnage.
ms.openlocfilehash: fb418154867aebb4d284e75be579003c0ddc88f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828855"
---
# <a name="postaladdress-personapostaladdresstype"></a><span data-ttu-id="aa1ae-103">PostalAddress (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="aa1ae-103">PostalAddress (PersonaPostalAddressType)</span></span>

<span data-ttu-id="aa1ae-104">L’élément **PostalAddress** Spécifie l’adresse postale pour un personnage.</span><span class="sxs-lookup"><span data-stu-id="aa1ae-104">The **PostalAddress** element specifies the postal address for a persona.</span></span> 
  
```XML
<PostalAddress>
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
   <PostOfficeBox/>
   <Type/>
   <Latitude/>
   <Longitude/>
   <Accuracy/>
   <Altitude/>
   <AltitudeAccuracy/>
   <FormattedAddress/>
   <LocationUri/>
   <LocationSource/>
</PostalAddress>
```

 <span data-ttu-id="aa1ae-105">**PersonaPostalAddressType**</span><span class="sxs-lookup"><span data-stu-id="aa1ae-105">**PersonaPostalAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa1ae-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aa1ae-106">Attributes and elements</span></span>

<span data-ttu-id="aa1ae-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aa1ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa1ae-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="aa1ae-108">Attributes</span></span>

<span data-ttu-id="aa1ae-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aa1ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa1ae-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aa1ae-110">Child elements</span></span>

<span data-ttu-id="aa1ae-111">[Rue](street.md) | [Ville](city.md) | [état](state-ex15websvcsotherref.md) | [pays](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md)  |  [ Longitude](longitude.md) | [précision](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="aa1ae-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aa1ae-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aa1ae-112">Parent elements</span></span>

[<span data-ttu-id="aa1ae-113">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="aa1ae-113">EnhancedLocation</span></span>](enhancedlocation.md)
  
## <a name="remarks"></a><span data-ttu-id="aa1ae-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="aa1ae-114">Remarks</span></span>

<span data-ttu-id="aa1ae-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="aa1ae-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aa1ae-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa1ae-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa1ae-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aa1ae-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa1ae-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aa1ae-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aa1ae-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aa1ae-119">Schema name</span></span>  <br/> |<span data-ttu-id="aa1ae-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="aa1ae-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="aa1ae-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="aa1ae-121">Validation file</span></span>  <br/> |<span data-ttu-id="aa1ae-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aa1ae-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aa1ae-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aa1ae-123">Can be empty</span></span>  <br/> ||
   

