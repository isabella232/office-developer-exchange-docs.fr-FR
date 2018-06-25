---
title: EmailAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: L’élément EmailAddressAttributedValue spécifie une instance d’un tableau des adresses de messagerie et leurs attributions associées.
ms.openlocfilehash: 3bcbb5c0a2bc9a2dc24516b5fc62e6e3363a360b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756117"
---
# <a name="emailaddressattributedvalue"></a><span data-ttu-id="d7cc8-103">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="d7cc8-103">EmailAddressAttributedValue</span></span>

<span data-ttu-id="d7cc8-104">L’élément **EmailAddressAttributedValue** spécifie une instance d’un tableau des adresses de messagerie et leurs attributions associées.</span><span class="sxs-lookup"><span data-stu-id="d7cc8-104">The **EmailAddressAttributedValue** element specifies an instance of an array of email addresses and their associated attributions.</span></span> 
  
```XML
<EmailAddressAttributedValue>
    <Value></Value>
    <Attributions></Attributions>
<EmailAddressAttributedValue>
```

 <span data-ttu-id="d7cc8-105">**EmailAddressAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="d7cc8-105">**EmailAddressAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7cc8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d7cc8-106">Attributes and elements</span></span>

<span data-ttu-id="d7cc8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d7cc8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7cc8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d7cc8-108">Attributes</span></span>

<span data-ttu-id="d7cc8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d7cc8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7cc8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d7cc8-110">Child elements</span></span>

|<span data-ttu-id="d7cc8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d7cc8-111">**Element**</span></span>|<span data-ttu-id="d7cc8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d7cc8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7cc8-113">Valeur (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d7cc8-113">Value (EmailAddressType)</span></span>](value-emailaddresstype.md) <br/> |<span data-ttu-id="d7cc8-114">Spécifie que la valeur d’une **adresse électronique** associé à un tableau des attributions.</span><span class="sxs-lookup"><span data-stu-id="d7cc8-114">Specifies the value of an **EmailAddress** associated with an attributions array.</span></span>  <br/> |
|[<span data-ttu-id="d7cc8-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="d7cc8-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="d7cc8-116">Spécifie un tableau des affectations pour sa **valeur** de l’élément associé.</span><span class="sxs-lookup"><span data-stu-id="d7cc8-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d7cc8-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d7cc8-117">Parent elements</span></span>

|<span data-ttu-id="d7cc8-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d7cc8-118">**Element**</span></span>|<span data-ttu-id="d7cc8-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="d7cc8-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7cc8-120">Emails1</span><span class="sxs-lookup"><span data-stu-id="d7cc8-120">Emails1</span></span>](emails1.md) <br/> |<span data-ttu-id="d7cc8-121">Spécifie un tableau de valeurs de messagerie et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="d7cc8-121">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
|[<span data-ttu-id="d7cc8-122">Emails2</span><span class="sxs-lookup"><span data-stu-id="d7cc8-122">Emails2</span></span>](emails2.md) <br/> |<span data-ttu-id="d7cc8-123">Spécifie un tableau de valeurs de messagerie et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="d7cc8-123">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
|[<span data-ttu-id="d7cc8-124">Emails3</span><span class="sxs-lookup"><span data-stu-id="d7cc8-124">Emails3</span></span>](emails3.md) <br/> |<span data-ttu-id="d7cc8-125">Spécifie un tableau de valeurs de messagerie et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="d7cc8-125">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d7cc8-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="d7cc8-126">Remarks</span></span>

<span data-ttu-id="d7cc8-127">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d7cc8-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d7cc8-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7cc8-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7cc8-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d7cc8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7cc8-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d7cc8-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d7cc8-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d7cc8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="d7cc8-132">Schéma type</span><span class="sxs-lookup"><span data-stu-id="d7cc8-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="d7cc8-133">Validation File</span><span class="sxs-lookup"><span data-stu-id="d7cc8-133">Validation File</span></span>  <br/> |<span data-ttu-id="d7cc8-134">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d7cc8-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d7cc8-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d7cc8-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d7cc8-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d7cc8-136">See also</span></span>



- [<span data-ttu-id="d7cc8-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d7cc8-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

