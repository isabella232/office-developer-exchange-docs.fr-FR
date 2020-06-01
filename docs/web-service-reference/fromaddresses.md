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
description: L’élément FromAddresses indique les adresses de messagerie à partir desquelles les messages entrants doivent être envoyés afin que la condition ou l’exception s’applique.
ms.openlocfilehash: 4fbb44d02f5010c4395cf691cb6160da4dbb6930
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459538"
---
# <a name="fromaddresses"></a><span data-ttu-id="a3078-103">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="a3078-103">FromAddresses</span></span>

<span data-ttu-id="a3078-104">L’élément **FromAddresses** indique les adresses de messagerie à partir desquelles les messages entrants doivent être envoyés afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="a3078-104">The **FromAddresses** element indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span> 
  
```XML
<FromAddresses>
   <Address/>
</FromAddresses>
```

 <span data-ttu-id="a3078-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="a3078-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3078-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a3078-106">Attributes and elements</span></span>

<span data-ttu-id="a3078-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a3078-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3078-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a3078-108">Attributes</span></span>

<span data-ttu-id="a3078-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a3078-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3078-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a3078-110">Child elements</span></span>

|<span data-ttu-id="a3078-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a3078-111">**Element**</span></span>|<span data-ttu-id="a3078-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a3078-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3078-113">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a3078-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="a3078-114">Représente une adresse de messagerie entièrement résolu.</span><span class="sxs-lookup"><span data-stu-id="a3078-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3078-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a3078-115">Parent elements</span></span>

|<span data-ttu-id="a3078-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a3078-116">**Element**</span></span>|<span data-ttu-id="a3078-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="a3078-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3078-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="a3078-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="a3078-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="a3078-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="a3078-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="a3078-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="a3078-121">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="a3078-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a3078-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a3078-122">Text value</span></span>

<span data-ttu-id="a3078-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a3078-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a3078-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="a3078-124">Remarks</span></span>

<span data-ttu-id="a3078-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3078-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3078-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a3078-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3078-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a3078-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a3078-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a3078-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a3078-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a3078-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a3078-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a3078-130">Validation File</span></span>  <br/> |<span data-ttu-id="a3078-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a3078-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a3078-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a3078-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3078-133">True</span><span class="sxs-lookup"><span data-stu-id="a3078-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3078-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a3078-134">See also</span></span>



- [<span data-ttu-id="a3078-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a3078-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

