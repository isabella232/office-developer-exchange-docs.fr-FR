---
title: PostalAddress (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 075f7d65-9d05-47cb-af26-0dd6d5593439
description: L’élément PostalAddress spécifie l’adresse postale d’un personnage.
ms.openlocfilehash: 9e316e5e0135c2d18fab4067241988c65eceec66
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465386"
---
# <a name="postaladdress-personapostaladdresstype"></a><span data-ttu-id="850d4-103">PostalAddress (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="850d4-103">PostalAddress (PersonaPostalAddressType)</span></span>

<span data-ttu-id="850d4-104">L’élément **PostalAddress** spécifie l’adresse postale d’un personnage.</span><span class="sxs-lookup"><span data-stu-id="850d4-104">The **PostalAddress** element specifies the postal address for a persona.</span></span> 
  
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

 <span data-ttu-id="850d4-105">**PersonaPostalAddressType**</span><span class="sxs-lookup"><span data-stu-id="850d4-105">**PersonaPostalAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="850d4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="850d4-106">Attributes and elements</span></span>

<span data-ttu-id="850d4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="850d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="850d4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="850d4-108">Attributes</span></span>

<span data-ttu-id="850d4-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="850d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="850d4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="850d4-110">Child elements</span></span>

<span data-ttu-id="850d4-111">[Rue](street.md)  |  [Ville](city.md)  |  [État](state-ex15websvcsotherref.md)  |  [Pays](country.md)  |  [CodePostal](postalcode.md)  |  [PostOfficeBox](postofficebox.md)  |  [Type (chaîne)](type-string.md)  |  [Latitude](latitude.md)  |  [Longitude](longitude.md)  |  [Précision](accuracy.md)  |  [Altitude](altitude.md)  |  [AltitudeAccuracy](altitudeaccuracy.md)  |  [FormattedAddress](formattedaddress.md)  |  [LocationUri](locationuri.md)  |  [LocationSource](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="850d4-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="850d4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="850d4-112">Parent elements</span></span>

[<span data-ttu-id="850d4-113">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="850d4-113">EnhancedLocation</span></span>](enhancedlocation.md)
  
## <a name="remarks"></a><span data-ttu-id="850d4-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="850d4-114">Remarks</span></span>

<span data-ttu-id="850d4-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="850d4-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="850d4-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="850d4-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="850d4-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="850d4-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="850d4-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="850d4-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="850d4-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="850d4-119">Schema name</span></span>  <br/> |<span data-ttu-id="850d4-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="850d4-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="850d4-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="850d4-121">Validation file</span></span>  <br/> |<span data-ttu-id="850d4-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="850d4-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="850d4-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="850d4-123">Can be empty</span></span>  <br/> ||
   

