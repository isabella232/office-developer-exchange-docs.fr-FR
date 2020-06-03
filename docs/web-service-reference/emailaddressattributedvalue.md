---
title: EmailAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: L’élément EmailAddressAttributedValue spécifie une instance d’un tableau d’adresses de messagerie et les attributions associées.
ms.openlocfilehash: 09fdd5921cef3d70a6da4b6d4d38f08834c5d482
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530690"
---
# <a name="emailaddressattributedvalue"></a><span data-ttu-id="cf789-103">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="cf789-103">EmailAddressAttributedValue</span></span>

<span data-ttu-id="cf789-104">L’élément **EmailAddressAttributedValue** spécifie une instance d’un tableau d’adresses de messagerie et les attributions associées.</span><span class="sxs-lookup"><span data-stu-id="cf789-104">The **EmailAddressAttributedValue** element specifies an instance of an array of email addresses and their associated attributions.</span></span> 
  
```XML
<EmailAddressAttributedValue>
    <Value></Value>
    <Attributions></Attributions>
<EmailAddressAttributedValue>
```

 <span data-ttu-id="cf789-105">**EmailAddressAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="cf789-105">**EmailAddressAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf789-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cf789-106">Attributes and elements</span></span>

<span data-ttu-id="cf789-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cf789-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf789-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cf789-108">Attributes</span></span>

<span data-ttu-id="cf789-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cf789-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf789-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cf789-110">Child elements</span></span>

|<span data-ttu-id="cf789-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cf789-111">**Element**</span></span>|<span data-ttu-id="cf789-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf789-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf789-113">Valeur (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="cf789-113">Value (EmailAddressType)</span></span>](value-emailaddresstype.md) <br/> |<span data-ttu-id="cf789-114">Spécifie la valeur d’un **EmailAddress** associé à un tableau d’attributions.</span><span class="sxs-lookup"><span data-stu-id="cf789-114">Specifies the value of an **EmailAddress** associated with an attributions array.</span></span>  <br/> |
|[<span data-ttu-id="cf789-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="cf789-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="cf789-116">Spécifie un tableau des attributions de l’élément **value** associé.</span><span class="sxs-lookup"><span data-stu-id="cf789-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf789-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cf789-117">Parent elements</span></span>

|<span data-ttu-id="cf789-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cf789-118">**Element**</span></span>|<span data-ttu-id="cf789-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf789-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf789-120">Emails1</span><span class="sxs-lookup"><span data-stu-id="cf789-120">Emails1</span></span>](emails1.md) <br/> |<span data-ttu-id="cf789-121">Spécifie un tableau de valeurs de messagerie et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="cf789-121">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
|[<span data-ttu-id="cf789-122">Emails2</span><span class="sxs-lookup"><span data-stu-id="cf789-122">Emails2</span></span>](emails2.md) <br/> |<span data-ttu-id="cf789-123">Spécifie un tableau de valeurs de messagerie et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="cf789-123">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
|[<span data-ttu-id="cf789-124">Emails3</span><span class="sxs-lookup"><span data-stu-id="cf789-124">Emails3</span></span>](emails3.md) <br/> |<span data-ttu-id="cf789-125">Spécifie un tableau de valeurs de messagerie et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="cf789-125">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cf789-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="cf789-126">Remarks</span></span>

<span data-ttu-id="cf789-127">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cf789-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cf789-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf789-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf789-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cf789-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf789-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cf789-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf789-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cf789-131">Schema Name</span></span>  <br/> |<span data-ttu-id="cf789-132">Schéma type</span><span class="sxs-lookup"><span data-stu-id="cf789-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="cf789-133">Validation File</span><span class="sxs-lookup"><span data-stu-id="cf789-133">Validation File</span></span>  <br/> |<span data-ttu-id="cf789-134">types. xsd</span><span class="sxs-lookup"><span data-stu-id="cf789-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf789-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cf789-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cf789-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cf789-136">See also</span></span>



- [<span data-ttu-id="cf789-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cf789-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

