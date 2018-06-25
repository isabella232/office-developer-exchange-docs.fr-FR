---
title: IsEncrypted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEncrypted
api_type:
- schema
ms.assetid: 68a30e92-c2b1-4af5-bb16-ba38afb80c43
description: L’élément IsEncrypted indique si les messages entrants doivent être chiffré afin que l’exception ou la condition à appliquer S/MIME.
ms.openlocfilehash: 582a1f197d4ee6b60af91b1a178d79163b50052c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828003"
---
# <a name="isencrypted"></a><span data-ttu-id="beedc-103">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="beedc-103">IsEncrypted</span></span>

<span data-ttu-id="beedc-104">L’élément **IsEncrypted** indique si les messages entrants doivent être chiffré afin que l’exception ou la condition à appliquer S/MIME.</span><span class="sxs-lookup"><span data-stu-id="beedc-104">The **IsEncrypted** element indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span> 
  
```XML
<IsEncrypted>true | false</IsEncrypted>
```

 <span data-ttu-id="beedc-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="beedc-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="beedc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="beedc-106">Attributes and elements</span></span>

<span data-ttu-id="beedc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="beedc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="beedc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="beedc-108">Attributes</span></span>

<span data-ttu-id="beedc-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="beedc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="beedc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="beedc-110">Child elements</span></span>

<span data-ttu-id="beedc-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="beedc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="beedc-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="beedc-112">Parent elements</span></span>

|<span data-ttu-id="beedc-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="beedc-113">**Element**</span></span>|<span data-ttu-id="beedc-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="beedc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="beedc-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="beedc-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="beedc-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="beedc-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="beedc-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="beedc-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="beedc-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="beedc-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="beedc-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="beedc-119">Text value</span></span>

<span data-ttu-id="beedc-120">Une valeur de texte de **la valeur true** indique que le message doit être S/MIME chiffré afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="beedc-120">A text value of **true** indicates that the message must be S/MIME encrypted in order for the condition or exception to apply.</span></span> <span data-ttu-id="beedc-121">La valeur **false** indique que le message n’a pas être S/MIME afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="beedc-121">A value of **false** indicates that the message does not have to be S/MIME in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="beedc-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="beedc-122">Remarks</span></span>

<span data-ttu-id="beedc-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="beedc-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="beedc-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="beedc-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="beedc-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="beedc-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="beedc-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="beedc-126">Schema Name</span></span>  <br/> |<span data-ttu-id="beedc-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="beedc-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="beedc-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="beedc-128">Validation File</span></span>  <br/> |<span data-ttu-id="beedc-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="beedc-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="beedc-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="beedc-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="beedc-131">True</span><span class="sxs-lookup"><span data-stu-id="beedc-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="beedc-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="beedc-132">See also</span></span>



- [<span data-ttu-id="beedc-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="beedc-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

