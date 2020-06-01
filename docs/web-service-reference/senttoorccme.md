---
title: SentToOrCcMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentToOrCcMe
api_type:
- schema
ms.assetid: ca43e05d-df37-485b-9276-34678025f2b7
description: L’élément SentToOrCcMe indique si le propriétaire de la boîte aux lettres doit se trouver dans une propriété ToRecipients ou CcRecipients des messages entrants afin que la condition ou l’exception s’applique.
ms.openlocfilehash: 906e5d9fd405b9aa6f772bcedbd1869b5023a05e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462079"
---
# <a name="senttoorccme"></a><span data-ttu-id="ba839-103">SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="ba839-103">SentToOrCcMe</span></span>

<span data-ttu-id="ba839-104">L’élément **SentToOrCcMe** indique si le propriétaire de la boîte aux lettres doit se trouver dans une propriété **ToRecipients** ou **CCRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="ba839-104">The **SentToOrCcMe** element indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToOrCcMe>true | false</SentToOrCcMe>
```

 <span data-ttu-id="ba839-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ba839-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba839-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ba839-106">Attributes and elements</span></span>

<span data-ttu-id="ba839-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ba839-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba839-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ba839-108">Attributes</span></span>

<span data-ttu-id="ba839-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ba839-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba839-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ba839-110">Child elements</span></span>

<span data-ttu-id="ba839-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba839-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba839-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ba839-112">Parent elements</span></span>

|<span data-ttu-id="ba839-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ba839-113">**Element**</span></span>|<span data-ttu-id="ba839-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba839-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba839-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="ba839-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="ba839-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="ba839-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="ba839-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="ba839-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="ba839-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="ba839-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ba839-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ba839-119">Text value</span></span>

<span data-ttu-id="ba839-120">Une valeur de texte **true** indique que le propriétaire de la boîte aux lettres doit se trouver dans la propriété **ToRecipients** ou **CCRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="ba839-120">A text value of **true** indicates that the owner of the mailbox must be in the **ToRecipients** or **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="ba839-121">La valeur **false** indique que le propriétaire de la boîte aux lettres ne doit pas se trouver dans la propriété **ToRecipients** ou **CCRecipients** des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="ba839-121">A value of **false** indicates that the owner of the mailbox must not be in the **ToRecipients** or **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ba839-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="ba839-122">Remarks</span></span>

<span data-ttu-id="ba839-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba839-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba839-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ba839-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba839-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ba839-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ba839-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ba839-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ba839-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ba839-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ba839-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ba839-128">Validation File</span></span>  <br/> |<span data-ttu-id="ba839-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ba839-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ba839-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ba839-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba839-131">True</span><span class="sxs-lookup"><span data-stu-id="ba839-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba839-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ba839-132">See also</span></span>



- [<span data-ttu-id="ba839-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba839-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

