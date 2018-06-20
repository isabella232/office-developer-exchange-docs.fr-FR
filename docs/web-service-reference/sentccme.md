---
title: SentCcMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentCcMe
api_type:
- schema
ms.assetid: bf5044e4-cbdf-4e24-a16f-b6454a51fcd5
description: L’élément SentCcMe indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété CcRecipients des messages entrants afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: 634a83d477efbe8683255c4fab71e3f7f1ab2191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829354"
---
# <a name="sentccme"></a><span data-ttu-id="6ff06-103">SentCcMe</span><span class="sxs-lookup"><span data-stu-id="6ff06-103">SentCcMe</span></span>

<span data-ttu-id="6ff06-104">L’élément **SentCcMe** indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **CcRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="6ff06-104">The **SentCcMe** element indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentCcMe>true | false</SentCcMe>
```

 <span data-ttu-id="6ff06-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6ff06-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ff06-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6ff06-106">Attributes and elements</span></span>

<span data-ttu-id="6ff06-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6ff06-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ff06-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6ff06-108">Attributes</span></span>

<span data-ttu-id="6ff06-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6ff06-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ff06-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6ff06-110">Child elements</span></span>

<span data-ttu-id="6ff06-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6ff06-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6ff06-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6ff06-112">Parent elements</span></span>

|<span data-ttu-id="6ff06-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6ff06-113">**Element**</span></span>|<span data-ttu-id="6ff06-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="6ff06-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ff06-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="6ff06-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="6ff06-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="6ff06-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="6ff06-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="6ff06-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="6ff06-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="6ff06-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6ff06-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6ff06-119">Text value</span></span>

<span data-ttu-id="6ff06-120">Texte la valeur **true** indique que le propriétaire de la boîte aux lettres doit être dans la propriété **CcRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="6ff06-120">A text value of **true** indicates that the owner of the mailbox must be in the **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="6ff06-121">La valeur **false** indique que le propriétaire de la boîte aux lettres ne doit pas être dans la propriété **CcRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="6ff06-121">A value of **false** indicates that the owner of the mailbox must not be in the **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6ff06-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="6ff06-122">Remarks</span></span>

<span data-ttu-id="6ff06-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ff06-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ff06-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6ff06-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ff06-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6ff06-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6ff06-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6ff06-126">Schema Name</span></span>  <br/> |<span data-ttu-id="6ff06-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6ff06-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6ff06-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6ff06-128">Validation File</span></span>  <br/> |<span data-ttu-id="6ff06-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6ff06-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6ff06-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6ff06-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ff06-131">True</span><span class="sxs-lookup"><span data-stu-id="6ff06-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ff06-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6ff06-132">See also</span></span>



- [<span data-ttu-id="6ff06-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6ff06-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

