---
title: Passe-temps
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f771b066-e42e-4880-bf18-709ad033d2af
description: L’élément de centres d’intérêt spécifie un tableau de centres d’intérêt et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: 0308269cb4b023c08433d62099fe22759ed498ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827813"
---
# <a name="hobbies"></a><span data-ttu-id="793c7-103">Passe-temps</span><span class="sxs-lookup"><span data-stu-id="793c7-103">Hobbies</span></span>

<span data-ttu-id="793c7-104">L’élément de **centres d’intérêt** spécifie un tableau de centres d’intérêt et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="793c7-104">The **Hobbies** element specifies an array of hobbies and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Hobbies>
    <StringAttributedValue/>
</Hobbies>
```

 <span data-ttu-id="793c7-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="793c7-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="793c7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="793c7-106">Attributes and elements</span></span>

<span data-ttu-id="793c7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="793c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="793c7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="793c7-108">Attributes</span></span>

<span data-ttu-id="793c7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="793c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="793c7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="793c7-110">Child elements</span></span>

|<span data-ttu-id="793c7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="793c7-111">**Element**</span></span>|<span data-ttu-id="793c7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="793c7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="793c7-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="793c7-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="793c7-114">Spécifie une instance d’un tableau d’attributs associés à un élément personnage.</span><span class="sxs-lookup"><span data-stu-id="793c7-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="793c7-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="793c7-115">Parent elements</span></span>

|<span data-ttu-id="793c7-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="793c7-116">**Element**</span></span>|<span data-ttu-id="793c7-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="793c7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="793c7-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="793c7-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="793c7-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="793c7-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="793c7-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="793c7-120">Remarks</span></span>

<span data-ttu-id="793c7-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="793c7-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="793c7-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="793c7-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="793c7-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="793c7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="793c7-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="793c7-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="793c7-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="793c7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="793c7-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="793c7-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="793c7-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="793c7-127">Validation File</span></span>  <br/> |<span data-ttu-id="793c7-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="793c7-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="793c7-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="793c7-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="793c7-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="793c7-130">See also</span></span>



- [<span data-ttu-id="793c7-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="793c7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

