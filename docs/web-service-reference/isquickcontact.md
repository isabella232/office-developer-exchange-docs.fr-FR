---
title: IsQuickContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1c9542d6-ef72-4743-828a-bb671e783836
description: L'élément IsQuickContact spécifie une valeur de type Boolean qui indique si le contact sous-jacent est un contact rapide.
ms.openlocfilehash: 979dbd3c0358eacd443eed79b258f7dd6bb9bc7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828092"
---
# <a name="isquickcontact"></a><span data-ttu-id="fe8d8-103">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="fe8d8-103">IsQuickContact</span></span>

<span data-ttu-id="fe8d8-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **IsQuickContact** spécifie une valeur de type Boolean qui indique si le contact sous-jacent est un contact rapide.</span><span class="sxs-lookup"><span data-stu-id="fe8d8-104">The **IsQuickContact** element specifies a Boolean value that indicates whether the underlying contact is a quick contact.</span></span> 
  
```XML
<IsQuickContact>true | false</IsQuickContact>
```

 <span data-ttu-id="fe8d8-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="fe8d8-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fe8d8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fe8d8-106">Attributes and elements</span></span>

<span data-ttu-id="fe8d8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fe8d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe8d8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fe8d8-108">Attributes</span></span>

<span data-ttu-id="fe8d8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fe8d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe8d8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fe8d8-110">Child elements</span></span>

<span data-ttu-id="fe8d8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fe8d8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fe8d8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fe8d8-112">Parent elements</span></span>

|<span data-ttu-id="fe8d8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fe8d8-113">**Element**</span></span>|<span data-ttu-id="fe8d8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe8d8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe8d8-115">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="fe8d8-116">Spécifie une instance d'un tableau d'attributs pour un élément **Persona**.</span><span class="sxs-lookup"><span data-stu-id="fe8d8-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fe8d8-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="fe8d8-117">Text value</span></span>

<span data-ttu-id="fe8d8-p101">Une valeur texte **true** pour l'élément **IsQuickContact** indique que le contact est un contact rapide. La valeur **false** indique que le contact n'est pas un contact rapide.</span><span class="sxs-lookup"><span data-stu-id="fe8d8-p101">A text value of **true** for the **IsQuickContact** element indicates that the contact is a quick contact. A value of **false** indicates that the contact is not a quick contact.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fe8d8-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="fe8d8-120">Remarks</span></span>

<span data-ttu-id="fe8d8-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fe8d8-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fe8d8-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe8d8-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe8d8-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fe8d8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe8d8-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fe8d8-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fe8d8-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fe8d8-125">Schema Name</span></span>  <br/> |<span data-ttu-id="fe8d8-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="fe8d8-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="fe8d8-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="fe8d8-127">Validation File</span></span>  <br/> |<span data-ttu-id="fe8d8-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="fe8d8-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="fe8d8-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fe8d8-129">Can Be Empty</span></span>  <br/> |<span data-ttu-id="fe8d8-130">false</span><span class="sxs-lookup"><span data-stu-id="fe8d8-130">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe8d8-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fe8d8-131">See also</span></span>



- [<span data-ttu-id="fe8d8-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fe8d8-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

