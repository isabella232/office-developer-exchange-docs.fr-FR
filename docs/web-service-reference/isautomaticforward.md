---
title: IsAutomaticForward
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAutomaticForward
api_type:
- schema
ms.assetid: 6876b849-a648-482e-8934-93eb5a0c465f
description: L’élément IsAutomaticForward indique si les messages entrants doivent être des transferts automatiques afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: c2d44d6dce30cbf55e0c7673aaf41b114a3e2cd4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827989"
---
# <a name="isautomaticforward"></a><span data-ttu-id="17ec1-103">IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="17ec1-103">IsAutomaticForward</span></span>

<span data-ttu-id="17ec1-104">L’élément **IsAutomaticForward** indique si les messages entrants doivent être des transferts automatiques afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="17ec1-104">The **IsAutomaticForward** element indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span> 
  
```XML
<IsAutomaticForward/> true | false</IsAutomaticForward>
```

 <span data-ttu-id="17ec1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="17ec1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17ec1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="17ec1-106">Attributes and elements</span></span>

<span data-ttu-id="17ec1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="17ec1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17ec1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="17ec1-108">Attributes</span></span>

<span data-ttu-id="17ec1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="17ec1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17ec1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="17ec1-110">Child elements</span></span>

<span data-ttu-id="17ec1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="17ec1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="17ec1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="17ec1-112">Parent elements</span></span>

|<span data-ttu-id="17ec1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="17ec1-113">**Element**</span></span>|<span data-ttu-id="17ec1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="17ec1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17ec1-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="17ec1-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="17ec1-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="17ec1-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="17ec1-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="17ec1-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="17ec1-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="17ec1-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="17ec1-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="17ec1-119">Text value</span></span>

<span data-ttu-id="17ec1-120">Texte la valeur **true** indique que le message doit être un transfert automatique afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="17ec1-120">A text value of **true** indicates that the message must be an automatic forward in order for the condition or exception to apply.</span></span> <span data-ttu-id="17ec1-121">La valeur **false** indique que le message ne doit pas être un transfert automatique afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="17ec1-121">A value of **false** indicates that the message must not be an automatic forward in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="17ec1-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="17ec1-122">Remarks</span></span>

<span data-ttu-id="17ec1-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="17ec1-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17ec1-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="17ec1-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17ec1-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="17ec1-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="17ec1-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="17ec1-126">Schema Name</span></span>  <br/> |<span data-ttu-id="17ec1-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="17ec1-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="17ec1-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="17ec1-128">Validation File</span></span>  <br/> |<span data-ttu-id="17ec1-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="17ec1-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="17ec1-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="17ec1-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="17ec1-131">True</span><span class="sxs-lookup"><span data-stu-id="17ec1-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17ec1-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="17ec1-132">See also</span></span>



- [<span data-ttu-id="17ec1-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="17ec1-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

