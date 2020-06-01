---
title: ExchangeStoreId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5acceb42-a757-4c74-ab1c-b1abf7bf1e0a
description: L’élément ExchangeStoreId spécifie l’identificateur de groupe de messagerie instantanée.
ms.openlocfilehash: c1b1e1830987449eeb7ea186d00743ea9cc75a77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456989"
---
# <a name="exchangestoreid"></a><span data-ttu-id="50b20-103">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="50b20-103">ExchangeStoreId</span></span>

<span data-ttu-id="50b20-104">L’élément **ExchangeStoreId** spécifie l’identificateur de groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="50b20-104">The **ExchangeStoreId** element specifies the instant messaging (IM) group identifier.</span></span> 
  
```XML
<ExchangeStoreId Id="" ChangeKey=""/>
```

 <span data-ttu-id="50b20-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="50b20-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50b20-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="50b20-106">Attributes and elements</span></span>

<span data-ttu-id="50b20-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="50b20-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50b20-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="50b20-108">Attributes</span></span>

|<span data-ttu-id="50b20-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="50b20-109">**Attribute**</span></span>|<span data-ttu-id="50b20-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="50b20-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="50b20-111">ID</span><span class="sxs-lookup"><span data-stu-id="50b20-111">Id</span></span>  <br/> |<span data-ttu-id="50b20-112">La valeur de texte de l’attribut **ID** est l’identificateur du groupe.</span><span class="sxs-lookup"><span data-stu-id="50b20-112">The text value of the **Id** attribute is the identifier of the group.</span></span>  <br/> |
|<span data-ttu-id="50b20-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="50b20-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="50b20-114">La valeur de texte de l’attribut **ChangeKey** est la clé de modification du groupe.</span><span class="sxs-lookup"><span data-stu-id="50b20-114">The text value of the **ChangeKey** attribute is the change key of the group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="50b20-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="50b20-115">Child elements</span></span>

<span data-ttu-id="50b20-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="50b20-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="50b20-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="50b20-117">Parent elements</span></span>

|<span data-ttu-id="50b20-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="50b20-118">**Element**</span></span>|<span data-ttu-id="50b20-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="50b20-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50b20-120">Imgroup</span><span class="sxs-lookup"><span data-stu-id="50b20-120">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="50b20-121">Représente un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="50b20-121">Represents an instant messaging group.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50b20-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="50b20-122">Remarks</span></span>

<span data-ttu-id="50b20-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="50b20-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="50b20-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="50b20-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50b20-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="50b20-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50b20-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="50b20-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="50b20-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="50b20-127">Schema Name</span></span>  <br/> |<span data-ttu-id="50b20-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="50b20-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="50b20-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="50b20-129">Validation File</span></span>  <br/> |<span data-ttu-id="50b20-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="50b20-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="50b20-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="50b20-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="50b20-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="50b20-132">See also</span></span>



- [<span data-ttu-id="50b20-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="50b20-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

