---
title: SentOnlyToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentOnlyToMe
api_type:
- schema
ms.assetid: b6d4dea5-812d-4b29-917d-071ebd7ddd92
description: L’élément SentOnlyToMe indique si le propriétaire de la boîte aux lettres doit être le seul à la propriété ToRecipients des messages entrants afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: 91c31069652a35dc7a38ad6b6e1512cc07d67a98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829353"
---
# <a name="sentonlytome"></a><span data-ttu-id="3c471-103">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="3c471-103">SentOnlyToMe</span></span>

<span data-ttu-id="3c471-104">L’élément **SentOnlyToMe** indique si le propriétaire de la boîte aux lettres doit être le seul à la propriété **ToRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="3c471-104">The **SentOnlyToMe** element indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentOnlyToMe/>true | false</SentOnlyToMe>
```

 <span data-ttu-id="3c471-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3c471-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c471-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3c471-106">Attributes and elements</span></span>

<span data-ttu-id="3c471-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3c471-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c471-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3c471-108">Attributes</span></span>

<span data-ttu-id="3c471-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3c471-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c471-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3c471-110">Child elements</span></span>

<span data-ttu-id="3c471-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3c471-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3c471-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3c471-112">Parent elements</span></span>

|<span data-ttu-id="3c471-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3c471-113">**Element**</span></span>|<span data-ttu-id="3c471-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3c471-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c471-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="3c471-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="3c471-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="3c471-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="3c471-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="3c471-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="3c471-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="3c471-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3c471-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3c471-119">Text value</span></span>

<span data-ttu-id="3c471-120">Une valeur de texte de **la valeur true** indique que le propriétaire de la boîte aux lettres doit être le seul à la propriété **ToRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="3c471-120">A text value of **true** indicates that the owner of the mailbox must be the only one in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="3c471-121">La valeur **false** indique que le propriétaire de la boîte aux lettres ne doit pas être le seul à la propriété **ToRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="3c471-121">A value of **false** indicates that the owner of the mailbox must not be the only one in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3c471-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="3c471-122">Remarks</span></span>

<span data-ttu-id="3c471-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c471-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c471-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3c471-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c471-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3c471-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3c471-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3c471-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3c471-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3c471-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3c471-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3c471-128">Validation File</span></span>  <br/> |<span data-ttu-id="3c471-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3c471-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3c471-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3c471-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c471-131">True</span><span class="sxs-lookup"><span data-stu-id="3c471-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c471-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3c471-132">See also</span></span>



- [<span data-ttu-id="3c471-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3c471-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

