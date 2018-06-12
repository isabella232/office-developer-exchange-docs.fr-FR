---
title: Opérations
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Operations
api_type:
- schema
ms.assetid: d8cd41b1-28ae-4c95-9ff6-8b25c8e18306
description: L’élément opérations contient un tableau des opérations de règle qui peuvent être effectuées sur une boîte de réception.
ms.openlocfilehash: 1030703d5e496be391d557e99e1420f9fddfdb36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828655"
---
# <a name="operations"></a><span data-ttu-id="04299-103">Opérations</span><span class="sxs-lookup"><span data-stu-id="04299-103">Operations</span></span>

<span data-ttu-id="04299-104">L’élément **opérations** contient un tableau des opérations de règle qui peuvent être effectuées sur une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="04299-104">The **Operations** element contains an array of rule operations that can be performed on an Inbox.</span></span> 
  
[<span data-ttu-id="04299-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="04299-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 <span data-ttu-id="04299-106">**ArrayOfRuleOperationsType**</span><span class="sxs-lookup"><span data-stu-id="04299-106">**ArrayOfRuleOperationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04299-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="04299-107">Attributes and elements</span></span>

<span data-ttu-id="04299-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="04299-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04299-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="04299-109">Attributes</span></span>

<span data-ttu-id="04299-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="04299-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04299-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="04299-111">Child elements</span></span>

|<span data-ttu-id="04299-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04299-112">**Element**</span></span>|<span data-ttu-id="04299-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="04299-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04299-114">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="04299-114">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="04299-115">Représente une opération pour créer une nouvelle règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="04299-115">Represents an operation to create a new Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="04299-116">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="04299-116">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="04299-117">Représente une opération de mise à jour d’une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="04299-117">Represents an operation to update an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="04299-118">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="04299-118">DeleteRuleOperation</span></span>](deleteruleoperation.md) <br/> |<span data-ttu-id="04299-119">Représente une opération pour supprimer une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="04299-119">Represents an operation to delete an Inbox rule.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04299-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="04299-120">Parent elements</span></span>

|<span data-ttu-id="04299-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04299-121">**Element**</span></span>|<span data-ttu-id="04299-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="04299-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04299-123">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="04299-123">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="04299-124">Définit une demande pour mettre à jour les règles de boîte de réception dans une boîte aux lettres dans le magasin du serveur.</span><span class="sxs-lookup"><span data-stu-id="04299-124">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="04299-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="04299-125">Remarks</span></span>

<span data-ttu-id="04299-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="04299-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04299-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="04299-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04299-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="04299-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04299-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="04299-129">Schema Name</span></span>  <br/> |<span data-ttu-id="04299-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="04299-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="04299-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="04299-131">Validation File</span></span>  <br/> |<span data-ttu-id="04299-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="04299-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04299-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="04299-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="04299-134">False</span><span class="sxs-lookup"><span data-stu-id="04299-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04299-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="04299-135">See also</span></span>



[<span data-ttu-id="04299-136">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="04299-136">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="04299-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="04299-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

