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
description: L’élément Operations contient un tableau d’opérations de règle qui peuvent être effectuées sur une boîte de réception.
ms.openlocfilehash: 4bbec4ad6424f802bb6781a870d65f23705e88c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462485"
---
# <a name="operations"></a><span data-ttu-id="92390-103">Opérations</span><span class="sxs-lookup"><span data-stu-id="92390-103">Operations</span></span>

<span data-ttu-id="92390-104">L’élément **Operations** contient un tableau d’opérations de règle qui peuvent être effectuées sur une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="92390-104">The **Operations** element contains an array of rule operations that can be performed on an Inbox.</span></span> 
  
[<span data-ttu-id="92390-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="92390-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 <span data-ttu-id="92390-106">**ArrayOfRuleOperationsType**</span><span class="sxs-lookup"><span data-stu-id="92390-106">**ArrayOfRuleOperationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92390-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="92390-107">Attributes and elements</span></span>

<span data-ttu-id="92390-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="92390-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92390-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="92390-109">Attributes</span></span>

<span data-ttu-id="92390-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="92390-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92390-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="92390-111">Child elements</span></span>

|<span data-ttu-id="92390-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="92390-112">**Element**</span></span>|<span data-ttu-id="92390-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="92390-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92390-114">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="92390-114">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="92390-115">Représente une opération de création d’une nouvelle règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="92390-115">Represents an operation to create a new Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="92390-116">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="92390-116">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="92390-117">Représente une opération de mise à jour d’une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="92390-117">Represents an operation to update an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="92390-118">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="92390-118">DeleteRuleOperation</span></span>](deleteruleoperation.md) <br/> |<span data-ttu-id="92390-119">Représente une opération de suppression d’une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="92390-119">Represents an operation to delete an Inbox rule.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92390-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="92390-120">Parent elements</span></span>

|<span data-ttu-id="92390-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="92390-121">**Element**</span></span>|<span data-ttu-id="92390-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="92390-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92390-123">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="92390-123">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="92390-124">Définit une demande de mise à jour des règles de boîte de réception dans une boîte aux lettres dans le magasin du serveur.</span><span class="sxs-lookup"><span data-stu-id="92390-124">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="92390-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="92390-125">Remarks</span></span>

<span data-ttu-id="92390-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="92390-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92390-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="92390-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92390-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="92390-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92390-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="92390-129">Schema Name</span></span>  <br/> |<span data-ttu-id="92390-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="92390-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="92390-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="92390-131">Validation File</span></span>  <br/> |<span data-ttu-id="92390-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="92390-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92390-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="92390-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="92390-134">False</span><span class="sxs-lookup"><span data-stu-id="92390-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92390-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="92390-135">See also</span></span>



[<span data-ttu-id="92390-136">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="92390-136">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="92390-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="92390-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

