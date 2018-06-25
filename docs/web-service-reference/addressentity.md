---
title: AddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ead22eab-f1e7-48b4-a165-db0e49fe86a8
description: L’élément AddressEntity spécifie une entité d’adresse unique.
ms.openlocfilehash: 6a46a64c9824efdd8df6a08fe1a159e7e42b3731
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755192"
---
# <a name="addressentity"></a><span data-ttu-id="d2a8f-103">AddressEntity</span><span class="sxs-lookup"><span data-stu-id="d2a8f-103">AddressEntity</span></span>

<span data-ttu-id="d2a8f-104">L’élément **AddressEntity** spécifie une entité d’adresse unique.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-104">The **AddressEntity** element specifies a single address entity.</span></span> 
  
```XML
<AddressEntity>
    <Address></Address>
    <Position></Position>
</AddressEntity>
```

 <span data-ttu-id="d2a8f-105">**AddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="d2a8f-105">**AddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2a8f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d2a8f-106">Attributes and elements</span></span>

<span data-ttu-id="d2a8f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2a8f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d2a8f-108">Attributes</span></span>

<span data-ttu-id="d2a8f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2a8f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d2a8f-110">Child elements</span></span>

|<span data-ttu-id="d2a8f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d2a8f-111">**Element**</span></span>|<span data-ttu-id="d2a8f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2a8f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2a8f-113">Adresse (chaîne)</span><span class="sxs-lookup"><span data-stu-id="d2a8f-113">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="d2a8f-114">Spécifie une adresse.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-114">Specifies an address.</span></span>  <br/> |
|[<span data-ttu-id="d2a8f-115">Position</span><span class="sxs-lookup"><span data-stu-id="d2a8f-115">Position</span></span>](position.md) <br/> |<span data-ttu-id="d2a8f-116">Spécifie la position dans un message électronique.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-116">Specifies the position in an email message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2a8f-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d2a8f-117">Parent elements</span></span>

|<span data-ttu-id="d2a8f-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d2a8f-118">**Element**</span></span>|<span data-ttu-id="d2a8f-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2a8f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2a8f-120">Adresses (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="d2a8f-120">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="d2a8f-121">Spécifie un tableau d’éléments **AddressEntity** .</span><span class="sxs-lookup"><span data-stu-id="d2a8f-121">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d2a8f-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d2a8f-122">Text value</span></span>

<span data-ttu-id="d2a8f-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d2a8f-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="d2a8f-124">Remarks</span></span>

<span data-ttu-id="d2a8f-125">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d2a8f-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2a8f-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2a8f-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d2a8f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2a8f-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d2a8f-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2a8f-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d2a8f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d2a8f-130">Schéma type</span><span class="sxs-lookup"><span data-stu-id="d2a8f-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="d2a8f-131">Validation File</span><span class="sxs-lookup"><span data-stu-id="d2a8f-131">Validation File</span></span>  <br/> |<span data-ttu-id="d2a8f-132">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d2a8f-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2a8f-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d2a8f-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d2a8f-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d2a8f-134">See also</span></span>

- [<span data-ttu-id="d2a8f-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d2a8f-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

