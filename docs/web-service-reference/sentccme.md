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
description: L’élément SentCcMe indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété CcRecipients des messages entrants afin que la condition ou l’exception s’applique.
ms.openlocfilehash: 1fae56a8e7d4e56c56884e5fff051ecd9f138a6d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465477"
---
# <a name="sentccme"></a><span data-ttu-id="5b259-103">SentCcMe</span><span class="sxs-lookup"><span data-stu-id="5b259-103">SentCcMe</span></span>

<span data-ttu-id="5b259-104">L’élément **SentCcMe** indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **CCRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="5b259-104">The **SentCcMe** element indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentCcMe>true | false</SentCcMe>
```

 <span data-ttu-id="5b259-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5b259-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b259-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5b259-106">Attributes and elements</span></span>

<span data-ttu-id="5b259-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5b259-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b259-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5b259-108">Attributes</span></span>

<span data-ttu-id="5b259-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5b259-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b259-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5b259-110">Child elements</span></span>

<span data-ttu-id="5b259-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5b259-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5b259-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5b259-112">Parent elements</span></span>

|<span data-ttu-id="5b259-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5b259-113">**Element**</span></span>|<span data-ttu-id="5b259-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5b259-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b259-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="5b259-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="5b259-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="5b259-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="5b259-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="5b259-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="5b259-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="5b259-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5b259-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="5b259-119">Text value</span></span>

<span data-ttu-id="5b259-120">Une valeur de texte **true** indique que le propriétaire de la boîte aux lettres doit se trouver dans la propriété **CCRecipients** des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="5b259-120">A text value of **true** indicates that the owner of the mailbox must be in the **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="5b259-121">La valeur **false** indique que le propriétaire de la boîte aux lettres ne doit pas se trouver dans la propriété **CCRecipients** des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="5b259-121">A value of **false** indicates that the owner of the mailbox must not be in the **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5b259-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="5b259-122">Remarks</span></span>

<span data-ttu-id="5b259-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b259-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b259-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5b259-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b259-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5b259-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5b259-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5b259-126">Schema Name</span></span>  <br/> |<span data-ttu-id="5b259-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="5b259-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5b259-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5b259-128">Validation File</span></span>  <br/> |<span data-ttu-id="5b259-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5b259-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5b259-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5b259-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b259-131">True</span><span class="sxs-lookup"><span data-stu-id="5b259-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b259-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5b259-132">See also</span></span>



- [<span data-ttu-id="5b259-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5b259-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

