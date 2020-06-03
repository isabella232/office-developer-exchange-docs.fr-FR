---
title: BusinessAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 828f8f62-7abf-44d4-8d58-f706d595a812
description: L’élément BusinessAddresses spécifie un tableau d’adresses professionnelles et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: d314d0de679f8eabc51dc9ee3b2e9a57cd0b8da1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465925"
---
# <a name="businessaddresses"></a><span data-ttu-id="c901f-103">BusinessAddresses</span><span class="sxs-lookup"><span data-stu-id="c901f-103">BusinessAddresses</span></span>

<span data-ttu-id="c901f-104">L’élément **BusinessAddresses** spécifie un tableau d’adresses professionnelles et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="c901f-104">The **BusinessAddresses** element specifies an array of business addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessAddresses>
    <PostalAddressAttributedValue></PostalAddressAttributedValue>
</BusinessAddresses
```

 <span data-ttu-id="c901f-105">**ArrayOfPostalAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="c901f-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c901f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c901f-106">Attributes and elements</span></span>

<span data-ttu-id="c901f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c901f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c901f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c901f-108">Attributes</span></span>

<span data-ttu-id="c901f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c901f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c901f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c901f-110">Child elements</span></span>

|<span data-ttu-id="c901f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c901f-111">**Element**</span></span>|<span data-ttu-id="c901f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c901f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c901f-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="c901f-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="c901f-114">Spécifie une instance d’un tableau d’adresses postales et leurs attributions associées.</span><span class="sxs-lookup"><span data-stu-id="c901f-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c901f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c901f-115">Parent elements</span></span>

|<span data-ttu-id="c901f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c901f-116">**Element**</span></span>|<span data-ttu-id="c901f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c901f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c901f-118">Persona</span><span class="sxs-lookup"><span data-stu-id="c901f-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="c901f-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="c901f-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c901f-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="c901f-120">Remarks</span></span>

<span data-ttu-id="c901f-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c901f-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c901f-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c901f-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c901f-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c901f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c901f-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c901f-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c901f-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c901f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c901f-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="c901f-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="c901f-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="c901f-127">Validation File</span></span>  <br/> |<span data-ttu-id="c901f-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="c901f-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c901f-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c901f-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c901f-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c901f-130">See also</span></span>



- [<span data-ttu-id="c901f-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c901f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

