---
title: FromAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FromAddresses
api_type:
- schema
ms.assetid: b219f315-c20a-4633-af3e-94bd3e4526b6
description: L’élément FromAddresses indique les adresses de messagerie à partir de laquelle les messages entrants doivent être envoyés afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: 40ecb1f3e16ad961b8e4c38d5aa9d15f4f74469a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756490"
---
# <a name="fromaddresses"></a><span data-ttu-id="16405-103">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="16405-103">FromAddresses</span></span>

<span data-ttu-id="16405-104">L’élément **FromAddresses** indique les adresses de messagerie à partir de laquelle les messages entrants doivent être envoyés afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="16405-104">The **FromAddresses** element indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span> 
  
```XML
<FromAddresses>
   <Address/>
</FromAddresses>
```

 <span data-ttu-id="16405-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="16405-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16405-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="16405-106">Attributes and elements</span></span>

<span data-ttu-id="16405-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="16405-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16405-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="16405-108">Attributes</span></span>

<span data-ttu-id="16405-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="16405-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16405-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="16405-110">Child elements</span></span>

|<span data-ttu-id="16405-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="16405-111">**Element**</span></span>|<span data-ttu-id="16405-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="16405-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16405-113">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="16405-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="16405-114">Représente une adresse de messagerie entièrement résolu.</span><span class="sxs-lookup"><span data-stu-id="16405-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="16405-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="16405-115">Parent elements</span></span>

|<span data-ttu-id="16405-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="16405-116">**Element**</span></span>|<span data-ttu-id="16405-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="16405-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16405-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="16405-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="16405-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="16405-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="16405-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="16405-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="16405-121">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="16405-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="16405-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="16405-122">Text value</span></span>

<span data-ttu-id="16405-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="16405-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="16405-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="16405-124">Remarks</span></span>

<span data-ttu-id="16405-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="16405-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16405-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="16405-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16405-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="16405-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="16405-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="16405-128">Schema Name</span></span>  <br/> |<span data-ttu-id="16405-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="16405-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="16405-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="16405-130">Validation File</span></span>  <br/> |<span data-ttu-id="16405-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="16405-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="16405-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="16405-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="16405-133">True</span><span class="sxs-lookup"><span data-stu-id="16405-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16405-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="16405-134">See also</span></span>



- [<span data-ttu-id="16405-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="16405-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

