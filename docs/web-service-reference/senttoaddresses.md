---
title: SentToAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentToAddresses
api_type:
- schema
ms.assetid: 086130d2-93b1-4de1-9553-10ec10322a0c
description: L’élément SentToAddresses indique les adresses de messagerie dont les messages entrants ont été envoyées aux afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: c5a4770ff22e08713e5cf40b9a81191d50a2f437
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829358"
---
# <a name="senttoaddresses"></a><span data-ttu-id="abe2e-103">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="abe2e-103">SentToAddresses</span></span>

<span data-ttu-id="abe2e-104">L’élément **SentToAddresses** indique les adresses de messagerie dont les messages entrants ont été envoyées aux afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="abe2e-104">The **SentToAddresses** element indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToAddresses>
   <Address/>
</SentToAddresses>
```

 <span data-ttu-id="abe2e-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="abe2e-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="abe2e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="abe2e-106">Attributes and elements</span></span>

<span data-ttu-id="abe2e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="abe2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="abe2e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="abe2e-108">Attributes</span></span>

<span data-ttu-id="abe2e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="abe2e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="abe2e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="abe2e-110">Child elements</span></span>

|<span data-ttu-id="abe2e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="abe2e-111">**Element**</span></span>|<span data-ttu-id="abe2e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="abe2e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abe2e-113">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="abe2e-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="abe2e-114">Représente une adresse de messagerie entièrement résolu.</span><span class="sxs-lookup"><span data-stu-id="abe2e-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="abe2e-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="abe2e-115">Parent elements</span></span>

|<span data-ttu-id="abe2e-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="abe2e-116">**Element**</span></span>|<span data-ttu-id="abe2e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="abe2e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abe2e-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="abe2e-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="abe2e-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="abe2e-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="abe2e-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="abe2e-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="abe2e-121">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="abe2e-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="abe2e-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="abe2e-122">Text value</span></span>

<span data-ttu-id="abe2e-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="abe2e-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="abe2e-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="abe2e-124">Remarks</span></span>

<span data-ttu-id="abe2e-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="abe2e-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="abe2e-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="abe2e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="abe2e-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="abe2e-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="abe2e-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="abe2e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="abe2e-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="abe2e-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="abe2e-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="abe2e-130">Validation File</span></span>  <br/> |<span data-ttu-id="abe2e-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="abe2e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="abe2e-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="abe2e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="abe2e-133">True</span><span class="sxs-lookup"><span data-stu-id="abe2e-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="abe2e-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="abe2e-134">See also</span></span>



- [<span data-ttu-id="abe2e-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="abe2e-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

