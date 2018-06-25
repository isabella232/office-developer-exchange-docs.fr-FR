---
title: HomeFaxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 459ddb1c-8cff-4125-b6fa-dc93c183dee8
description: L’élément HomeFaxes spécifie un tableau de télécopie (domicile) nombres et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: dd2cd8bba2c4cc7d08e88787d648e96ea996a251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827840"
---
# <a name="homefaxes"></a><span data-ttu-id="1dd2a-103">HomeFaxes</span><span class="sxs-lookup"><span data-stu-id="1dd2a-103">HomeFaxes</span></span>

<span data-ttu-id="1dd2a-104">L’élément **HomeFaxes** spécifie un tableau de télécopie (domicile) nombres et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="1dd2a-104">The **HomeFaxes** element specifies an array of home fax numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeFaxes>
    <PhoneNumberAttributedValue/>
</HomeFaxes>
```

 <span data-ttu-id="1dd2a-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="1dd2a-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1dd2a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1dd2a-106">Attributes and elements</span></span>

<span data-ttu-id="1dd2a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1dd2a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1dd2a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1dd2a-108">Attributes</span></span>

<span data-ttu-id="1dd2a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1dd2a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1dd2a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1dd2a-110">Child elements</span></span>

|<span data-ttu-id="1dd2a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1dd2a-111">**Element**</span></span>|<span data-ttu-id="1dd2a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1dd2a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dd2a-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="1dd2a-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="1dd2a-114">Contient un numéro de téléphone attribué unique un personnage.</span><span class="sxs-lookup"><span data-stu-id="1dd2a-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1dd2a-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1dd2a-115">Parent elements</span></span>

|<span data-ttu-id="1dd2a-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1dd2a-116">**Element**</span></span>|<span data-ttu-id="1dd2a-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1dd2a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dd2a-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="1dd2a-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="1dd2a-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="1dd2a-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1dd2a-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="1dd2a-120">Remarks</span></span>

<span data-ttu-id="1dd2a-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1dd2a-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1dd2a-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1dd2a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1dd2a-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1dd2a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1dd2a-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1dd2a-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1dd2a-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1dd2a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1dd2a-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="1dd2a-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="1dd2a-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="1dd2a-127">Validation File</span></span>  <br/> |<span data-ttu-id="1dd2a-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="1dd2a-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1dd2a-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1dd2a-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1dd2a-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1dd2a-130">See also</span></span>



- [<span data-ttu-id="1dd2a-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1dd2a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

