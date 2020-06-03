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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466905"
---
# <a name="addressentity"></a><span data-ttu-id="2c528-103">AddressEntity</span><span class="sxs-lookup"><span data-stu-id="2c528-103">AddressEntity</span></span>

<span data-ttu-id="2c528-104">L’élément **AddressEntity** spécifie une entité d’adresse unique.</span><span class="sxs-lookup"><span data-stu-id="2c528-104">The **AddressEntity** element specifies a single address entity.</span></span> 
  
```XML
<AddressEntity>
    <Address></Address>
    <Position></Position>
</AddressEntity>
```

 <span data-ttu-id="2c528-105">**AddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="2c528-105">**AddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c528-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2c528-106">Attributes and elements</span></span>

<span data-ttu-id="2c528-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2c528-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c528-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2c528-108">Attributes</span></span>

<span data-ttu-id="2c528-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2c528-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c528-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2c528-110">Child elements</span></span>

|<span data-ttu-id="2c528-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2c528-111">**Element**</span></span>|<span data-ttu-id="2c528-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2c528-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c528-113">Address (chaîne)</span><span class="sxs-lookup"><span data-stu-id="2c528-113">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="2c528-114">Spécifie une adresse.</span><span class="sxs-lookup"><span data-stu-id="2c528-114">Specifies an address.</span></span>  <br/> |
|[<span data-ttu-id="2c528-115">Position</span><span class="sxs-lookup"><span data-stu-id="2c528-115">Position</span></span>](position.md) <br/> |<span data-ttu-id="2c528-116">Indique la position dans un message électronique.</span><span class="sxs-lookup"><span data-stu-id="2c528-116">Specifies the position in an email message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2c528-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2c528-117">Parent elements</span></span>

|<span data-ttu-id="2c528-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2c528-118">**Element**</span></span>|<span data-ttu-id="2c528-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="2c528-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c528-120">Adresses (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="2c528-120">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="2c528-121">Spécifie un tableau d’éléments **AddressEntity** .</span><span class="sxs-lookup"><span data-stu-id="2c528-121">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2c528-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2c528-122">Text value</span></span>

<span data-ttu-id="2c528-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2c528-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2c528-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="2c528-124">Remarks</span></span>

<span data-ttu-id="2c528-125">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2c528-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2c528-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c528-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c528-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2c528-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c528-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2c528-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c528-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2c528-129">Schema Name</span></span>  <br/> |<span data-ttu-id="2c528-130">Schéma type</span><span class="sxs-lookup"><span data-stu-id="2c528-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="2c528-131">Validation File</span><span class="sxs-lookup"><span data-stu-id="2c528-131">Validation File</span></span>  <br/> |<span data-ttu-id="2c528-132">types. xsd</span><span class="sxs-lookup"><span data-stu-id="2c528-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c528-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2c528-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2c528-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2c528-134">See also</span></span>

- [<span data-ttu-id="2c528-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2c528-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

