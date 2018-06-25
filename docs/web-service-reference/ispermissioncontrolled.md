---
title: IsPermissionControlled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsPermissionControlled
api_type:
- schema
ms.assetid: a2fd0340-f31f-4389-a1cd-7e93b40bb3c6
description: L’élément IsPermissionControlled indique si les messages entrants doivent être sous contrôlée de l’autorisation (protégés par RMS) afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: fdd9910b8c35d9d57e724d6fec57d203f38f0359
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828088"
---
# <a name="ispermissioncontrolled"></a><span data-ttu-id="86f68-103">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="86f68-103">IsPermissionControlled</span></span>

<span data-ttu-id="86f68-104">L’élément **IsPermissionControlled** indique si les messages entrants doivent être sous contrôlée de l’autorisation (protégés par RMS) afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="86f68-104">The **IsPermissionControlled** element indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply.</span></span> 
  
```XML
<IsPermissionControlled>true | false</IsPermissionControlled>
```

 <span data-ttu-id="86f68-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="86f68-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86f68-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="86f68-106">Attributes and elements</span></span>

<span data-ttu-id="86f68-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="86f68-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86f68-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="86f68-108">Attributes</span></span>

<span data-ttu-id="86f68-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="86f68-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86f68-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="86f68-110">Child elements</span></span>

<span data-ttu-id="86f68-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="86f68-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="86f68-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="86f68-112">Parent elements</span></span>

|<span data-ttu-id="86f68-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="86f68-113">**Element**</span></span>|<span data-ttu-id="86f68-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="86f68-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86f68-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="86f68-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="86f68-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="86f68-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="86f68-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="86f68-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="86f68-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="86f68-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="86f68-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="86f68-119">Text value</span></span>

<span data-ttu-id="86f68-120">Une valeur de texte de **la valeur true** indique que le message doit être RMS protégé afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="86f68-120">A text value of **true** indicates that the message must be RMS protected in order for the condition or exception to apply.</span></span> <span data-ttu-id="86f68-121">La valeur **false** indique que le message ne doit pas être RMS protégé afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="86f68-121">A value of **false** indicates that the message must not be RMS protected in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="86f68-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="86f68-122">Remarks</span></span>

<span data-ttu-id="86f68-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="86f68-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86f68-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="86f68-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86f68-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="86f68-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="86f68-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="86f68-126">Schema Name</span></span>  <br/> |<span data-ttu-id="86f68-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="86f68-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="86f68-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="86f68-128">Validation File</span></span>  <br/> |<span data-ttu-id="86f68-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="86f68-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="86f68-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="86f68-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="86f68-131">True</span><span class="sxs-lookup"><span data-stu-id="86f68-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86f68-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="86f68-132">See also</span></span>



- [<span data-ttu-id="86f68-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="86f68-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

