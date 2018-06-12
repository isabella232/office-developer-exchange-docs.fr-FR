---
title: ContainsSenderStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSenderStrings
api_type:
- schema
ms.assetid: 3e16163f-cffe-4c4e-9a2a-00245d25ba96
description: L’élément ContainsSenderStrings indique les chaînes qui doivent apparaître dans la propriété From des messages entrants afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: d174c0d7e2cbfd5b671a825a867d3ee7e24c2f2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755597"
---
# <a name="containssenderstrings"></a><span data-ttu-id="b3196-103">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="b3196-103">ContainsSenderStrings</span></span>

<span data-ttu-id="b3196-104">L’élément **ContainsSenderStrings** indique les chaînes qui doivent apparaître dans la propriété **From** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="b3196-104">The **ContainsSenderStrings** element indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSenderStrings>
    <String/>
</ContainsSenderStrings>
```

 <span data-ttu-id="b3196-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="b3196-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3196-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b3196-106">Attributes and elements</span></span>

<span data-ttu-id="b3196-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b3196-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3196-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b3196-108">Attributes</span></span>

<span data-ttu-id="b3196-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b3196-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3196-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b3196-110">Child elements</span></span>

|<span data-ttu-id="b3196-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b3196-111">**Element**</span></span>|<span data-ttu-id="b3196-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b3196-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3196-113">String</span><span class="sxs-lookup"><span data-stu-id="b3196-113">String</span></span>](string.md) <br/> |<span data-ttu-id="b3196-114">Représente une chaîne qui doit apparaître dans la propriété **From** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="b3196-114">Represents a string that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b3196-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b3196-115">Parent elements</span></span>

|<span data-ttu-id="b3196-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b3196-116">**Element**</span></span>|<span data-ttu-id="b3196-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b3196-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3196-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="b3196-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="b3196-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="b3196-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="b3196-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="b3196-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="b3196-121">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="b3196-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b3196-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b3196-122">Text value</span></span>

<span data-ttu-id="b3196-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b3196-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b3196-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="b3196-124">Remarks</span></span>

<span data-ttu-id="b3196-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3196-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3196-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b3196-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3196-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b3196-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b3196-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b3196-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b3196-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b3196-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b3196-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b3196-130">Validation File</span></span>  <br/> |<span data-ttu-id="b3196-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b3196-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b3196-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b3196-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b3196-133">True</span><span class="sxs-lookup"><span data-stu-id="b3196-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3196-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b3196-134">See also</span></span>



- [<span data-ttu-id="b3196-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b3196-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

