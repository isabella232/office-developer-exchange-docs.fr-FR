---
title: Adresses (ArrayOfAddressesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 711acc90-8e5b-4658-92d2-16cd441db56e
description: L’élément adresses spécifie un tableau d’éléments de l’adresse.
ms.openlocfilehash: c1ee79611da1d19ce85202f9e3c0f68c421e98c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755187"
---
# <a name="addresses-arrayofaddressestype"></a><span data-ttu-id="d573c-103">Adresses (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="d573c-103">Addresses (ArrayOfAddressesType)</span></span>

<span data-ttu-id="d573c-104">L’élément **adresses** spécifie un tableau d’éléments de **l’adresse** .</span><span class="sxs-lookup"><span data-stu-id="d573c-104">The **Addresses** element specifies an array of **Address** elements.</span></span> 
  
```XML
<Addresses>
    <Address></Address>
</Addresses>
```

 <span data-ttu-id="d573c-105">**ArrayOfAddressesType**</span><span class="sxs-lookup"><span data-stu-id="d573c-105">**ArrayOfAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d573c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d573c-106">Attributes and elements</span></span>

<span data-ttu-id="d573c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d573c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d573c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d573c-108">Attributes</span></span>

<span data-ttu-id="d573c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d573c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d573c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d573c-110">Child elements</span></span>

|<span data-ttu-id="d573c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d573c-111">**Element**</span></span>|<span data-ttu-id="d573c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d573c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d573c-113">Adresse (TypeContact)</span><span class="sxs-lookup"><span data-stu-id="d573c-113">Address (ContactType)</span></span>](address-contacttype.md) <br/> |<span data-ttu-id="d573c-114">Spécifie l’adresse d’un contact.</span><span class="sxs-lookup"><span data-stu-id="d573c-114">Specifies the address of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d573c-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d573c-115">Parent elements</span></span>

|<span data-ttu-id="d573c-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d573c-116">**Element**</span></span>|<span data-ttu-id="d573c-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d573c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d573c-118">Contact (TypeContact)</span><span class="sxs-lookup"><span data-stu-id="d573c-118">Contact (ContactType)</span></span>](contact-contacttype.md) <br/> |<span data-ttu-id="d573c-119">Spécifie un contact dans le magasin de contacts unifié.</span><span class="sxs-lookup"><span data-stu-id="d573c-119">Specifies a contact in the Unified Contact Store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d573c-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="d573c-120">Remarks</span></span>

<span data-ttu-id="d573c-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d573c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d573c-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d573c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d573c-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d573c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d573c-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d573c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d573c-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d573c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d573c-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="d573c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d573c-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="d573c-127">Validation File</span></span>  <br/> |<span data-ttu-id="d573c-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d573c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d573c-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d573c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d573c-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d573c-130">See also</span></span>

- [<span data-ttu-id="d573c-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d573c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

