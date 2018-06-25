---
title: Attributions (ArrayOfPersonaAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f61d843c-bca5-4c88-9667-fd03d2a963a1
description: L’élément Attributions spécifie un tableau des informations d’attribution pour une ou plusieurs contacts ou les destinataires Active Directory dans le personnage associé.
ms.openlocfilehash: 52fecb4e4381d5e9dbbaf7134fa18068ba15f6ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755348"
---
# <a name="attributions-arrayofpersonaattributionstype"></a><span data-ttu-id="f73ed-103">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="f73ed-103">Attributions (ArrayOfPersonaAttributionsType)</span></span>

<span data-ttu-id="f73ed-104">L’élément **Attributions** spécifie un tableau des informations d’attribution pour une ou plusieurs contacts ou les destinataires Active Directory dans le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="f73ed-104">The **Attributions** element specifies an array of attribution information for one or more of the contacts or Active Directory recipients aggregated into the associated persona.</span></span> 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attributions>
```

 <span data-ttu-id="f73ed-105">**ArrayOfPersonaAttributionsType**</span><span class="sxs-lookup"><span data-stu-id="f73ed-105">**ArrayOfPersonaAttributionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f73ed-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f73ed-106">Attributes and elements</span></span>

<span data-ttu-id="f73ed-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f73ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f73ed-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f73ed-108">Attributes</span></span>

<span data-ttu-id="f73ed-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f73ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f73ed-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f73ed-110">Child elements</span></span>

|<span data-ttu-id="f73ed-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f73ed-111">**Element**</span></span>|<span data-ttu-id="f73ed-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f73ed-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f73ed-113">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="f73ed-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="f73ed-114">Spécifie une instance d’un tableau d’attributs pour un élément **PersonaType** .</span><span class="sxs-lookup"><span data-stu-id="f73ed-114">Specifies an instance in an array of attributes for a **PersonaType** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f73ed-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f73ed-115">Parent elements</span></span>

|<span data-ttu-id="f73ed-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f73ed-116">**Element**</span></span>|<span data-ttu-id="f73ed-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="f73ed-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f73ed-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="f73ed-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="f73ed-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="f73ed-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f73ed-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="f73ed-120">Remarks</span></span>

<span data-ttu-id="f73ed-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f73ed-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f73ed-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f73ed-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f73ed-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f73ed-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f73ed-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f73ed-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f73ed-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f73ed-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f73ed-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="f73ed-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="f73ed-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="f73ed-127">Validation File</span></span>  <br/> |<span data-ttu-id="f73ed-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="f73ed-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f73ed-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f73ed-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f73ed-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f73ed-130">See also</span></span>

- [<span data-ttu-id="f73ed-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f73ed-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

