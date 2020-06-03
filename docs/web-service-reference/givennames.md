---
title: GivenNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 64d86c24-07b8-448d-ad37-47f104777df3
description: L’élément GivenNames spécifie un tableau de valeurs de nom données et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: c76d69344b59fb56377a13b9ea4a588acc382013
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530126"
---
# <a name="givennames"></a><span data-ttu-id="ac072-103">GivenNames</span><span class="sxs-lookup"><span data-stu-id="ac072-103">GivenNames</span></span>

<span data-ttu-id="ac072-104">L’élément **GivenNames** spécifie un tableau de valeurs de nom données et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="ac072-104">The **GivenNames** element specifies an array of given name values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```xml
<GivenNames>
    <StringAttributedValue/>
</GivenNames>
```

 <span data-ttu-id="ac072-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="ac072-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac072-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ac072-106">Attributes and elements</span></span>

<span data-ttu-id="ac072-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ac072-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac072-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ac072-108">Attributes</span></span>

<span data-ttu-id="ac072-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ac072-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac072-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ac072-110">Child elements</span></span>

|<span data-ttu-id="ac072-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ac072-111">**Element**</span></span>|<span data-ttu-id="ac072-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ac072-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac072-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="ac072-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="ac072-114">Spécifie une instance dans un tableau d’attributs associés à un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="ac072-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ac072-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ac072-115">Parent elements</span></span>

|<span data-ttu-id="ac072-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ac072-116">**Element**</span></span>|<span data-ttu-id="ac072-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ac072-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac072-118">Persona</span><span class="sxs-lookup"><span data-stu-id="ac072-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="ac072-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="ac072-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ac072-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="ac072-120">Remarks</span></span>

<span data-ttu-id="ac072-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ac072-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ac072-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac072-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac072-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ac072-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac072-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ac072-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ac072-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ac072-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ac072-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="ac072-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="ac072-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="ac072-127">Validation File</span></span>  <br/> |<span data-ttu-id="ac072-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="ac072-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ac072-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ac072-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ac072-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ac072-130">See also</span></span>



- [<span data-ttu-id="ac072-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ac072-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

