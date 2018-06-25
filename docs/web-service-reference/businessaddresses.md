---
title: BusinessAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 828f8f62-7abf-44d4-8d58-f706d595a812
description: L’élément BusinessAddresses spécifie un tableau d’adresses d’entreprise et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: bc7ad948572c24f913ae02abb9e8fc5a7b1e0b0d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755423"
---
# <a name="businessaddresses"></a><span data-ttu-id="8c3e1-103">BusinessAddresses</span><span class="sxs-lookup"><span data-stu-id="8c3e1-103">BusinessAddresses</span></span>

<span data-ttu-id="8c3e1-104">L’élément **BusinessAddresses** spécifie un tableau d’adresses d’entreprise et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="8c3e1-104">The **BusinessAddresses** element specifies an array of business addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessAddresses>
    <PostalAddressAttributedValue></PostalAddressAttributedValue>
</BusinessAddresses
```

 <span data-ttu-id="8c3e1-105">**ArrayOfPostalAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="8c3e1-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8c3e1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8c3e1-106">Attributes and elements</span></span>

<span data-ttu-id="8c3e1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8c3e1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c3e1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8c3e1-108">Attributes</span></span>

<span data-ttu-id="8c3e1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8c3e1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8c3e1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8c3e1-110">Child elements</span></span>

|<span data-ttu-id="8c3e1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8c3e1-111">**Element**</span></span>|<span data-ttu-id="8c3e1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8c3e1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c3e1-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="8c3e1-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="8c3e1-114">Spécifie une instance d’un tableau d’adresses postales et leurs attributions associées.</span><span class="sxs-lookup"><span data-stu-id="8c3e1-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8c3e1-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8c3e1-115">Parent elements</span></span>

|<span data-ttu-id="8c3e1-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8c3e1-116">**Element**</span></span>|<span data-ttu-id="8c3e1-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="8c3e1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c3e1-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="8c3e1-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="8c3e1-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="8c3e1-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8c3e1-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="8c3e1-120">Remarks</span></span>

<span data-ttu-id="8c3e1-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8c3e1-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8c3e1-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8c3e1-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8c3e1-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8c3e1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8c3e1-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8c3e1-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8c3e1-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8c3e1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8c3e1-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="8c3e1-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="8c3e1-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="8c3e1-127">Validation File</span></span>  <br/> |<span data-ttu-id="8c3e1-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="8c3e1-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8c3e1-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8c3e1-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8c3e1-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8c3e1-130">See also</span></span>



- [<span data-ttu-id="8c3e1-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8c3e1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

