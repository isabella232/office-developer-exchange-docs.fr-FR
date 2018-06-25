---
title: ExchangeStoreId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5acceb42-a757-4c74-ab1c-b1abf7bf1e0a
description: L’élément ExchangeStoreId Spécifie l’identificateur de groupe (IM) de messagerie instantanée.
ms.openlocfilehash: 815e9c2f368558ea38efce3671dbdc33d4d97168
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756245"
---
# <a name="exchangestoreid"></a><span data-ttu-id="f8ec4-103">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="f8ec4-103">ExchangeStoreId</span></span>

<span data-ttu-id="f8ec4-104">L’élément **ExchangeStoreId** Spécifie l’identificateur de groupe (IM) de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="f8ec4-104">The **ExchangeStoreId** element specifies the instant messaging (IM) group identifier.</span></span> 
  
```XML
<ExchangeStoreId Id="" ChangeKey=""/>
```

 <span data-ttu-id="f8ec4-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="f8ec4-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8ec4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f8ec4-106">Attributes and elements</span></span>

<span data-ttu-id="f8ec4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f8ec4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8ec4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f8ec4-108">Attributes</span></span>

|<span data-ttu-id="f8ec4-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="f8ec4-109">**Attribute**</span></span>|<span data-ttu-id="f8ec4-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="f8ec4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f8ec4-111">ID</span><span class="sxs-lookup"><span data-stu-id="f8ec4-111">Id</span></span>  <br/> |<span data-ttu-id="f8ec4-112">La valeur de texte de l’attribut **Id** est l’identificateur du groupe.</span><span class="sxs-lookup"><span data-stu-id="f8ec4-112">The text value of the **Id** attribute is the identifier of the group.</span></span>  <br/> |
|<span data-ttu-id="f8ec4-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="f8ec4-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="f8ec4-114">La valeur de texte de l’attribut **ChangeKey** est la clé de modification du groupe.</span><span class="sxs-lookup"><span data-stu-id="f8ec4-114">The text value of the **ChangeKey** attribute is the change key of the group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f8ec4-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f8ec4-115">Child elements</span></span>

<span data-ttu-id="f8ec4-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f8ec4-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f8ec4-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f8ec4-117">Parent elements</span></span>

|<span data-ttu-id="f8ec4-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f8ec4-118">**Element**</span></span>|<span data-ttu-id="f8ec4-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="f8ec4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8ec4-120">ImGroup</span><span class="sxs-lookup"><span data-stu-id="f8ec4-120">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="f8ec4-121">Représente un groupe de messagerie instantané.</span><span class="sxs-lookup"><span data-stu-id="f8ec4-121">Represents an instant messaging group.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f8ec4-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="f8ec4-122">Remarks</span></span>

<span data-ttu-id="f8ec4-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f8ec4-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f8ec4-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8ec4-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8ec4-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f8ec4-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8ec4-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f8ec4-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f8ec4-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f8ec4-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f8ec4-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="f8ec4-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="f8ec4-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="f8ec4-129">Validation File</span></span>  <br/> |<span data-ttu-id="f8ec4-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="f8ec4-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f8ec4-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f8ec4-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f8ec4-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f8ec4-132">See also</span></span>



- [<span data-ttu-id="f8ec4-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f8ec4-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

