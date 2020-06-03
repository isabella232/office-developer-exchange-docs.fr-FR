---
title: Anniversaires
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5a84c19e-57cd-448e-af4f-c8005fd5f2a2
description: L’élément birthdays spécifie un tableau d’anniversaires, stockés sous forme de chaînes et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: aa85febd84c32ae87e0822ce47fd99f445b6fe9e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462758"
---
# <a name="birthdays"></a><span data-ttu-id="59158-103">Anniversaires</span><span class="sxs-lookup"><span data-stu-id="59158-103">Birthdays</span></span>

<span data-ttu-id="59158-104">L’élément **birthdays** spécifie un tableau d’anniversaires, stockés sous forme de chaînes et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="59158-104">The **Birthdays** element specifies an array of birthdays, stored as strings, and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Birthdays>
   <StringAttributedValue/>
</Birthdays>
```

 <span data-ttu-id="59158-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="59158-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59158-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="59158-106">Attributes and elements</span></span>

<span data-ttu-id="59158-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="59158-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59158-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="59158-108">Attributes</span></span>

<span data-ttu-id="59158-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="59158-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59158-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="59158-110">Child elements</span></span>

|<span data-ttu-id="59158-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59158-111">**Element**</span></span>|<span data-ttu-id="59158-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="59158-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59158-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="59158-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="59158-114">Spécifie une instance dans un tableau d’attributs associés à un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="59158-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59158-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="59158-115">Parent elements</span></span>

|<span data-ttu-id="59158-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59158-116">**Element**</span></span>|<span data-ttu-id="59158-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="59158-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59158-118">Persona</span><span class="sxs-lookup"><span data-stu-id="59158-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="59158-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="59158-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="59158-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="59158-120">Remarks</span></span>

<span data-ttu-id="59158-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="59158-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="59158-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="59158-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59158-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="59158-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59158-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="59158-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59158-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="59158-125">Schema Name</span></span>  <br/> |<span data-ttu-id="59158-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="59158-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="59158-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="59158-127">Validation File</span></span>  <br/> |<span data-ttu-id="59158-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="59158-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="59158-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="59158-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="59158-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59158-130">See also</span></span>



- [<span data-ttu-id="59158-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="59158-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

