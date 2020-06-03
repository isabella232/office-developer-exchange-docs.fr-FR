---
title: Initiales (ArrayOfStringAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 060c0cf1-c632-484c-87f5-f577017a7090
description: L’élément Initials spécifie un tableau de valeurs initiales et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: 16133192fa1d9ef066e46a181f490248a8197e5b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458200"
---
# <a name="initials-arrayofstringattributedvaluestype"></a><span data-ttu-id="2c3cf-103">Initiales (ArrayOfStringAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="2c3cf-103">Initials (ArrayOfStringAttributedValuesType)</span></span>

<span data-ttu-id="2c3cf-104">L’élément **Initials** spécifie un tableau de valeurs initiales et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="2c3cf-104">The **Initials** element specifies an array of initials values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Initials>
    <StringAttributedValue/>
</Initials>
```

 <span data-ttu-id="2c3cf-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="2c3cf-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c3cf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2c3cf-106">Attributes and elements</span></span>

<span data-ttu-id="2c3cf-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2c3cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c3cf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2c3cf-108">Attributes</span></span>

<span data-ttu-id="2c3cf-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2c3cf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c3cf-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2c3cf-110">Child elements</span></span>

|<span data-ttu-id="2c3cf-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2c3cf-111">**Element**</span></span>|<span data-ttu-id="2c3cf-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2c3cf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c3cf-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="2c3cf-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="2c3cf-114">Spécifie une instance dans un tableau d’attributs associés à un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="2c3cf-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2c3cf-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2c3cf-115">Parent elements</span></span>

|<span data-ttu-id="2c3cf-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2c3cf-116">**Element**</span></span>|<span data-ttu-id="2c3cf-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="2c3cf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c3cf-118">Persona</span><span class="sxs-lookup"><span data-stu-id="2c3cf-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="2c3cf-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="2c3cf-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2c3cf-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="2c3cf-120">Remarks</span></span>

<span data-ttu-id="2c3cf-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2c3cf-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2c3cf-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c3cf-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c3cf-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2c3cf-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c3cf-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2c3cf-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c3cf-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2c3cf-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2c3cf-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="2c3cf-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2c3cf-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="2c3cf-127">Validation File</span></span>  <br/> |<span data-ttu-id="2c3cf-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="2c3cf-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c3cf-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2c3cf-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2c3cf-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2c3cf-130">See also</span></span>



- [<span data-ttu-id="2c3cf-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2c3cf-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

