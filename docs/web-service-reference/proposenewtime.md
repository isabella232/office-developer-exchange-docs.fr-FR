---
title: ProposeNewTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6d5977ac-484e-4e53-92ba-58a868eb3395
description: L’élément ProposeNewTime spécifie un objet de réponse qui indique que le participant à la réunion peut proposer une nouvelle heure de réunion.
ms.openlocfilehash: 4a0238d94b29993def8009fae62380bb2c02e8b6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828904"
---
# <a name="proposenewtime"></a><span data-ttu-id="9ffca-103">ProposeNewTime</span><span class="sxs-lookup"><span data-stu-id="9ffca-103">ProposeNewTime</span></span>

<span data-ttu-id="9ffca-104">L’élément **ProposeNewTime** spécifie un objet de réponse qui indique que le participant à la réunion peut proposer une nouvelle heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="9ffca-104">The **ProposeNewTime** element specifies a response object that indicates that the meeting attendee can propose a new meeting time.</span></span> 
  
```XML
<ProposeNewTime ObjectName=""></ProposeNewTime>
```

 <span data-ttu-id="9ffca-105">**ProposeNewTimeType**</span><span class="sxs-lookup"><span data-stu-id="9ffca-105">**ProposeNewTimeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ffca-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9ffca-106">Attributes and elements</span></span>

<span data-ttu-id="9ffca-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9ffca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ffca-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9ffca-108">Attributes</span></span>

****

|<span data-ttu-id="9ffca-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="9ffca-109">**Attribute**</span></span>|<span data-ttu-id="9ffca-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="9ffca-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9ffca-111">ObjectName</span><span class="sxs-lookup"><span data-stu-id="9ffca-111">ObjectName</span></span>  <br/> |<span data-ttu-id="9ffca-112">Nom de l’objet de réponse.</span><span class="sxs-lookup"><span data-stu-id="9ffca-112">The name of the response object.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9ffca-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9ffca-113">Child elements</span></span>

<span data-ttu-id="9ffca-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9ffca-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9ffca-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9ffca-115">Parent elements</span></span>

[<span data-ttu-id="9ffca-116">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="9ffca-116">ResponseObjects</span></span>](responseobjects.md)
  
## <a name="remarks"></a><span data-ttu-id="9ffca-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="9ffca-117">Remarks</span></span>

<span data-ttu-id="9ffca-118">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9ffca-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="9ffca-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ffca-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ffca-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9ffca-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ffca-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9ffca-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ffca-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9ffca-122">Schema Name</span></span>  <br/> |<span data-ttu-id="9ffca-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9ffca-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ffca-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9ffca-124">Validation File</span></span>  <br/> |<span data-ttu-id="9ffca-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9ffca-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ffca-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9ffca-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ffca-127">True</span><span class="sxs-lookup"><span data-stu-id="9ffca-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ffca-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9ffca-128">See also</span></span>



[<span data-ttu-id="9ffca-129">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="9ffca-129">ResponseObjects</span></span>](responseobjects.md)


- [<span data-ttu-id="9ffca-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9ffca-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

