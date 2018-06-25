---
title: NotSentToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NotSentToMe
api_type:
- schema
ms.assetid: 7cb63269-622c-4198-9a21-f5a021bf6901
description: L’élément NotSentToMe indique si le propriétaire de la boîte aux lettres ne doit pas être dans la propriété ToRecipients des messages entrants afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: 917648f811855961877d1aba4924573e95e3962a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828555"
---
# <a name="notsenttome"></a><span data-ttu-id="91e99-103">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="91e99-103">NotSentToMe</span></span>

<span data-ttu-id="91e99-104">L’élément **NotSentToMe** indique si le propriétaire de la boîte aux lettres ne doit pas être dans la propriété **ToRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="91e99-104">The **NotSentToMe** element indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
```xml
<NotSentToMe>true | false</NotSentToMe>
```

 <span data-ttu-id="91e99-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="91e99-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91e99-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="91e99-106">Attributes and elements</span></span>

<span data-ttu-id="91e99-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="91e99-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91e99-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="91e99-108">Attributes</span></span>

<span data-ttu-id="91e99-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="91e99-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91e99-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="91e99-110">Child elements</span></span>

<span data-ttu-id="91e99-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="91e99-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91e99-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="91e99-112">Parent elements</span></span>

|<span data-ttu-id="91e99-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="91e99-113">**Element**</span></span>|<span data-ttu-id="91e99-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="91e99-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91e99-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="91e99-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="91e99-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="91e99-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="91e99-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="91e99-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="91e99-118">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="91e99-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91e99-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="91e99-119">Text value</span></span>

<span data-ttu-id="91e99-120">Une valeur de texte de **la valeur true** indique que le propriétaire de la boîte aux lettres ne doit pas être dans la propriété **ToRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="91e99-120">A text value of **true** indicates that the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="91e99-121">La valeur **false** indique que le propriétaire de la boîte aux lettres doit être dans la propriété **ToRecipients** du message entrant afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="91e99-121">A value of **false** indicates that the owner of the mailbox must be in the **ToRecipients** property of the incoming message in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="91e99-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="91e99-122">Remarks</span></span>

<span data-ttu-id="91e99-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="91e99-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91e99-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="91e99-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91e99-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="91e99-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="91e99-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="91e99-126">Schema Name</span></span>  <br/> |<span data-ttu-id="91e99-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="91e99-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="91e99-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="91e99-128">Validation File</span></span>  <br/> |<span data-ttu-id="91e99-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="91e99-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="91e99-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="91e99-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="91e99-131">True</span><span class="sxs-lookup"><span data-stu-id="91e99-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91e99-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="91e99-132">See also</span></span>



- [<span data-ttu-id="91e99-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="91e99-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

