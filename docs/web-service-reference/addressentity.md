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
ms.openlocfilehash: c597557fe02a9c0ff7ed3c9862e1662cfbae596a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466905"
---
# <a name="addressentity"></a><span data-ttu-id="3c239-103">AddressEntity</span><span class="sxs-lookup"><span data-stu-id="3c239-103">AddressEntity</span></span>

<span data-ttu-id="3c239-104">L’élément **AddressEntity** spécifie une entité d’adresse unique.</span><span class="sxs-lookup"><span data-stu-id="3c239-104">The **AddressEntity** element specifies a single address entity.</span></span> 
  
```XML
<AddressEntity>
    <Address></Address>
    <Position></Position>
</AddressEntity>
```

 <span data-ttu-id="3c239-105">**AddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="3c239-105">**AddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c239-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3c239-106">Attributes and elements</span></span>

<span data-ttu-id="3c239-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3c239-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c239-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3c239-108">Attributes</span></span>

<span data-ttu-id="3c239-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3c239-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c239-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3c239-110">Child elements</span></span>

|<span data-ttu-id="3c239-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3c239-111">**Element**</span></span>|<span data-ttu-id="3c239-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3c239-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c239-113">Address (chaîne)</span><span class="sxs-lookup"><span data-stu-id="3c239-113">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="3c239-114">Spécifie une adresse.</span><span class="sxs-lookup"><span data-stu-id="3c239-114">Specifies an address.</span></span>  <br/> |
|[<span data-ttu-id="3c239-115">Position</span><span class="sxs-lookup"><span data-stu-id="3c239-115">Position</span></span>](position.md) <br/> |<span data-ttu-id="3c239-116">Indique la position dans un message électronique.</span><span class="sxs-lookup"><span data-stu-id="3c239-116">Specifies the position in an email message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c239-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3c239-117">Parent elements</span></span>

|<span data-ttu-id="3c239-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3c239-118">**Element**</span></span>|<span data-ttu-id="3c239-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="3c239-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c239-120">Adresses (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="3c239-120">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="3c239-121">Spécifie un tableau d’éléments **AddressEntity** .</span><span class="sxs-lookup"><span data-stu-id="3c239-121">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3c239-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3c239-122">Text value</span></span>

<span data-ttu-id="3c239-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3c239-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3c239-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="3c239-124">Remarks</span></span>

<span data-ttu-id="3c239-125">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3c239-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3c239-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c239-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c239-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3c239-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c239-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3c239-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c239-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3c239-129">Schema Name</span></span>  <br/> |<span data-ttu-id="3c239-130">Schéma type</span><span class="sxs-lookup"><span data-stu-id="3c239-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="3c239-131">Validation File</span><span class="sxs-lookup"><span data-stu-id="3c239-131">Validation File</span></span>  <br/> |<span data-ttu-id="3c239-132">types. xsd</span><span class="sxs-lookup"><span data-stu-id="3c239-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c239-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3c239-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3c239-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3c239-134">See also</span></span>

- [<span data-ttu-id="3c239-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3c239-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

