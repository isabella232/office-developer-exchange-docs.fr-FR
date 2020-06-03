---
title: Valeur (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be838fc2-cfcb-4856-b095-a8e5366bb6c6
description: L’élément Value spécifie les informations associées à une adresse postale.
ms.openlocfilehash: 2d644ff45fe89061ccd90279773f3a5a5b7fe7cc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466471"
---
# <a name="value-personapostaladdresstype"></a><span data-ttu-id="fef80-103">Valeur (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="fef80-103">Value (PersonaPostalAddressType)</span></span>

<span data-ttu-id="fef80-104">L’élément **value** spécifie les informations associées à une adresse postale.</span><span class="sxs-lookup"><span data-stu-id="fef80-104">The **Value** element specifies information associated with a postal address.</span></span> 
  
```XML
<Value>
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
</Value>
```

<span data-ttu-id="fef80-105">**PersonaPostalAddressType**</span><span class="sxs-lookup"><span data-stu-id="fef80-105">**PersonaPostalAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fef80-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fef80-106">Attributes and elements</span></span>

<span data-ttu-id="fef80-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fef80-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fef80-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fef80-108">Attributes</span></span>

<span data-ttu-id="fef80-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fef80-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fef80-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fef80-110">Child elements</span></span>

<span data-ttu-id="fef80-111">[Rue](street.md)  |  [Ville](city.md)  |  [État](state-ex15websvcsotherref.md)  |  [Pays](country.md)  |  [CodePostal](postalcode.md)  |  [PostOfficeBox](postofficebox.md)  |  [Type (chaîne)](type-string.md)  |  [Latitude](latitude.md)  |  [Longitude](longitude.md)  |  [Précision](accuracy.md)  |  [Altitude](altitude.md)  |  [AltitudeAccuracy](altitudeaccuracy.md)  |  [FormattedAddress](formattedaddress.md)  |  [LocationUri](locationuri.md)  |  [LocationSource](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="fef80-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fef80-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fef80-112">Parent elements</span></span>

[<span data-ttu-id="fef80-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="fef80-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md)
  
## <a name="remarks"></a><span data-ttu-id="fef80-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="fef80-114">Remarks</span></span>

<span data-ttu-id="fef80-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fef80-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fef80-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fef80-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fef80-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fef80-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fef80-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fef80-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fef80-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fef80-119">Schema name</span></span>  <br/> |<span data-ttu-id="fef80-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fef80-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="fef80-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fef80-121">Validation file</span></span>  <br/> |<span data-ttu-id="fef80-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fef80-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fef80-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fef80-123">Can be empty</span></span>  <br/> ||
   

