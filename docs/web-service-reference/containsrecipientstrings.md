---
title: ContainsRecipientStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsRecipientStrings
api_type:
- schema
ms.assetid: a7fd13ac-0f13-4610-ac9b-98e27ac3940b
description: L’élément ContainsRecipientStrings indique les chaînes qui doivent apparaître dans les ToRecipients CcRecipients propriétés ou des messages entrants afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: 861aba22c9474caf02f9c50d8a7b65b9cc8a2eda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755585"
---
# <a name="containsrecipientstrings"></a><span data-ttu-id="c52d8-103">ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="c52d8-103">ContainsRecipientStrings</span></span>

<span data-ttu-id="c52d8-104">L’élément **ContainsRecipientStrings** indique les chaînes qui doivent apparaître dans les **ToRecipients** **CcRecipients** propriétés ou des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="c52d8-104">The **ContainsRecipientStrings** element indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsRecipientStrings>
    <String/>
</ContainsRecipientStrings>
```

 <span data-ttu-id="c52d8-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="c52d8-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c52d8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c52d8-106">Attributes and elements</span></span>

<span data-ttu-id="c52d8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c52d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c52d8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c52d8-108">Attributes</span></span>

<span data-ttu-id="c52d8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c52d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c52d8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c52d8-110">Child elements</span></span>

|<span data-ttu-id="c52d8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c52d8-111">**Element**</span></span>|<span data-ttu-id="c52d8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c52d8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c52d8-113">String</span><span class="sxs-lookup"><span data-stu-id="c52d8-113">String</span></span>](string.md) <br/> |<span data-ttu-id="c52d8-114">Représente une chaîne qui doit apparaître dans les **ToRecipients** **CcRecipients** propriétés ou des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="c52d8-114">Represents a string that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c52d8-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c52d8-115">Parent elements</span></span>

|<span data-ttu-id="c52d8-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c52d8-116">**Element**</span></span>|<span data-ttu-id="c52d8-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c52d8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c52d8-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="c52d8-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="c52d8-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="c52d8-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="c52d8-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="c52d8-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="c52d8-121">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="c52d8-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c52d8-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c52d8-122">Text value</span></span>

<span data-ttu-id="c52d8-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c52d8-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c52d8-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="c52d8-124">Remarks</span></span>

<span data-ttu-id="c52d8-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c52d8-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c52d8-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c52d8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c52d8-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c52d8-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c52d8-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c52d8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c52d8-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c52d8-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c52d8-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c52d8-130">Validation File</span></span>  <br/> |<span data-ttu-id="c52d8-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c52d8-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c52d8-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c52d8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c52d8-133">True</span><span class="sxs-lookup"><span data-stu-id="c52d8-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c52d8-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c52d8-134">See also</span></span>



- [<span data-ttu-id="c52d8-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c52d8-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

