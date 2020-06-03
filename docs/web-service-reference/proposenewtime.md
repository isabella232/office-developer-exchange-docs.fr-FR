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
ms.openlocfilehash: 76f590db760826aa2cd26938947a9b0e02a603f7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465540"
---
# <a name="proposenewtime"></a><span data-ttu-id="6b351-103">ProposeNewTime</span><span class="sxs-lookup"><span data-stu-id="6b351-103">ProposeNewTime</span></span>

<span data-ttu-id="6b351-104">L’élément **ProposeNewTime** spécifie un objet de réponse qui indique que le participant à la réunion peut proposer une nouvelle heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="6b351-104">The **ProposeNewTime** element specifies a response object that indicates that the meeting attendee can propose a new meeting time.</span></span> 
  
```XML
<ProposeNewTime ObjectName=""></ProposeNewTime>
```

 <span data-ttu-id="6b351-105">**ProposeNewTimeType**</span><span class="sxs-lookup"><span data-stu-id="6b351-105">**ProposeNewTimeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b351-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6b351-106">Attributes and elements</span></span>

<span data-ttu-id="6b351-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6b351-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b351-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6b351-108">Attributes</span></span>

****

|<span data-ttu-id="6b351-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="6b351-109">**Attribute**</span></span>|<span data-ttu-id="6b351-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="6b351-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6b351-111">ObjectName</span><span class="sxs-lookup"><span data-stu-id="6b351-111">ObjectName</span></span>  <br/> |<span data-ttu-id="6b351-112">Nom de l’objet de la réponse.</span><span class="sxs-lookup"><span data-stu-id="6b351-112">The name of the response object.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6b351-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6b351-113">Child elements</span></span>

<span data-ttu-id="6b351-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6b351-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b351-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6b351-115">Parent elements</span></span>

[<span data-ttu-id="6b351-116">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="6b351-116">ResponseObjects</span></span>](responseobjects.md)
  
## <a name="remarks"></a><span data-ttu-id="6b351-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="6b351-117">Remarks</span></span>

<span data-ttu-id="6b351-118">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6b351-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="6b351-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b351-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b351-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6b351-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b351-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6b351-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b351-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6b351-122">Schema Name</span></span>  <br/> |<span data-ttu-id="6b351-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6b351-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="6b351-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6b351-124">Validation File</span></span>  <br/> |<span data-ttu-id="6b351-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6b351-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b351-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6b351-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b351-127">True</span><span class="sxs-lookup"><span data-stu-id="6b351-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b351-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6b351-128">See also</span></span>



[<span data-ttu-id="6b351-129">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="6b351-129">ResponseObjects</span></span>](responseobjects.md)


- [<span data-ttu-id="6b351-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6b351-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

