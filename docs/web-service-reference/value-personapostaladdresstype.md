---
title: Valeur (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be838fc2-cfcb-4856-b095-a8e5366bb6c6
description: L’élément valeur spécifie les informations associées à une adresse postale.
ms.openlocfilehash: 048d3a49552f1a9e89744e4cd16ec1745417e923
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838998"
---
# <a name="value-personapostaladdresstype"></a><span data-ttu-id="7e2ad-103">Valeur (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="7e2ad-103">Value (PersonaPostalAddressType)</span></span>

<span data-ttu-id="7e2ad-104">L’élément de **valeur** spécifie les informations associées à une adresse postale.</span><span class="sxs-lookup"><span data-stu-id="7e2ad-104">The **Value** element specifies information associated with a postal address.</span></span> 
  
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

<span data-ttu-id="7e2ad-105">**PersonaPostalAddressType**</span><span class="sxs-lookup"><span data-stu-id="7e2ad-105">**PersonaPostalAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7e2ad-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7e2ad-106">Attributes and elements</span></span>

<span data-ttu-id="7e2ad-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7e2ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e2ad-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7e2ad-108">Attributes</span></span>

<span data-ttu-id="7e2ad-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7e2ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e2ad-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7e2ad-110">Child elements</span></span>

<span data-ttu-id="7e2ad-111">[Rue](street.md) | [Ville](city.md) | [état](state-ex15websvcsotherref.md) | [pays](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md)  |  [ Longitude](longitude.md) | [précision](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="7e2ad-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e2ad-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7e2ad-112">Parent elements</span></span>

[<span data-ttu-id="7e2ad-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="7e2ad-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md)
  
## <a name="remarks"></a><span data-ttu-id="7e2ad-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="7e2ad-114">Remarks</span></span>

<span data-ttu-id="7e2ad-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7e2ad-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7e2ad-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e2ad-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e2ad-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7e2ad-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e2ad-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7e2ad-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e2ad-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7e2ad-119">Schema name</span></span>  <br/> |<span data-ttu-id="7e2ad-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7e2ad-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e2ad-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7e2ad-121">Validation file</span></span>  <br/> |<span data-ttu-id="7e2ad-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e2ad-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e2ad-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7e2ad-123">Can be empty</span></span>  <br/> ||
   

