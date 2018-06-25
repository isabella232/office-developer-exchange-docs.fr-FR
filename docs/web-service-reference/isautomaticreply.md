---
title: IsAutomaticReply
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAutomaticReply
api_type:
- schema
ms.assetid: 280e9baf-199d-422c-8fdf-1d0751a3e77d
description: L’élément IsAutomaticReply indique si les messages entrants doivent être des réponses automatiques afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: 3f26b947313b8c53f70e2a89b9a6bdd17840a055
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827995"
---
# <a name="isautomaticreply"></a><span data-ttu-id="1ea9e-103">IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="1ea9e-103">IsAutomaticReply</span></span>

<span data-ttu-id="1ea9e-104">L’élément **IsAutomaticReply** indique si les messages entrants doivent être des réponses automatiques afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-104">The **IsAutomaticReply** element indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span> 
  
```XML
<IsAutomaticReply> true | false</IsAutomaticReply>
```

 <span data-ttu-id="1ea9e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1ea9e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ea9e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1ea9e-106">Attributes and elements</span></span>

<span data-ttu-id="1ea9e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ea9e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1ea9e-108">Attributes</span></span>

<span data-ttu-id="1ea9e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ea9e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1ea9e-110">Child elements</span></span>

<span data-ttu-id="1ea9e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1ea9e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1ea9e-112">Parent elements</span></span>

|<span data-ttu-id="1ea9e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1ea9e-113">**Element**</span></span>|<span data-ttu-id="1ea9e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1ea9e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ea9e-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="1ea9e-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="1ea9e-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="1ea9e-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="1ea9e-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="1ea9e-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1ea9e-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1ea9e-119">Text value</span></span>

<span data-ttu-id="1ea9e-120">Texte la valeur **true** indique que le message doit être une réponse automatique afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-120">A text value of **true** indicates that the message must be an automatic reply in order for the condition or exception to apply.</span></span> <span data-ttu-id="1ea9e-121">La valeur **false** indique que le message n’a pas à une réponse automatique afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-121">A value of **false** indicates that the message does not have to be an automatic reply in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1ea9e-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="1ea9e-122">Remarks</span></span>

<span data-ttu-id="1ea9e-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ea9e-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1ea9e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ea9e-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1ea9e-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1ea9e-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1ea9e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="1ea9e-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1ea9e-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1ea9e-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1ea9e-128">Validation File</span></span>  <br/> |<span data-ttu-id="1ea9e-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1ea9e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1ea9e-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1ea9e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ea9e-131">True</span><span class="sxs-lookup"><span data-stu-id="1ea9e-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ea9e-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1ea9e-132">See also</span></span>



- [<span data-ttu-id="1ea9e-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1ea9e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

