---
title: AssistantPhoneNumbers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd9ac1-7db3-44ea-9117-18488dddde15
description: L’élément AssistantPhoneNumbers spécifie un tableau de numéros de téléphone de l’Assistant et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: a72c8d646750b5d7cf9ebca13a51f4df84bf7bdb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464482"
---
# <a name="assistantphonenumbers"></a><span data-ttu-id="6b617-103">AssistantPhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="6b617-103">AssistantPhoneNumbers</span></span>

<span data-ttu-id="6b617-104">L’élément **AssistantPhoneNumbers** spécifie un tableau de numéros de téléphone de l’Assistant et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="6b617-104">The **AssistantPhoneNumbers** element specifies an array of assistant phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantPhoneNumbers>
    <PhoneNumberAttributedValue></PhoneNumberAttributedValue>
</AssistantPhoneNumbers>
```

 <span data-ttu-id="6b617-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="6b617-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b617-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6b617-106">Attributes and elements</span></span>

<span data-ttu-id="6b617-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6b617-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b617-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6b617-108">Attributes</span></span>

<span data-ttu-id="6b617-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6b617-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b617-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6b617-110">Child elements</span></span>

|<span data-ttu-id="6b617-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6b617-111">**Element**</span></span>|<span data-ttu-id="6b617-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="6b617-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b617-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="6b617-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="6b617-114">Spécifie une instance d’un tableau de numéros de téléphone et leurs attributions associées.</span><span class="sxs-lookup"><span data-stu-id="6b617-114">Specifies an instance of an array of phone numbers and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b617-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6b617-115">Parent elements</span></span>

|<span data-ttu-id="6b617-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6b617-116">**Element**</span></span>|<span data-ttu-id="6b617-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="6b617-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b617-118">Persona</span><span class="sxs-lookup"><span data-stu-id="6b617-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="6b617-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="6b617-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6b617-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="6b617-120">Remarks</span></span>

<span data-ttu-id="6b617-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6b617-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6b617-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b617-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b617-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6b617-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b617-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6b617-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b617-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6b617-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6b617-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="6b617-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="6b617-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="6b617-127">Validation File</span></span>  <br/> |<span data-ttu-id="6b617-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="6b617-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b617-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6b617-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6b617-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6b617-130">See also</span></span>

- [<span data-ttu-id="6b617-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6b617-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

