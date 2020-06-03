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
description: L’élément IsAutomaticReply indique si les messages entrants doivent être des réponses automatiques afin que la condition ou l’exception s’applique.
ms.openlocfilehash: 7521dbbb458cf7683b52b2fe4fddacd276b40256
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455561"
---
# <a name="isautomaticreply"></a><span data-ttu-id="30a55-103">IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="30a55-103">IsAutomaticReply</span></span>

<span data-ttu-id="30a55-104">L’élément **IsAutomaticReply** indique si les messages entrants doivent être des réponses automatiques afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="30a55-104">The **IsAutomaticReply** element indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span> 
  
```XML
<IsAutomaticReply> true | false</IsAutomaticReply>
```

 <span data-ttu-id="30a55-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="30a55-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30a55-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="30a55-106">Attributes and elements</span></span>

<span data-ttu-id="30a55-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="30a55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30a55-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="30a55-108">Attributes</span></span>

<span data-ttu-id="30a55-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="30a55-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30a55-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="30a55-110">Child elements</span></span>

<span data-ttu-id="30a55-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="30a55-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="30a55-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="30a55-112">Parent elements</span></span>

|<span data-ttu-id="30a55-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="30a55-113">**Element**</span></span>|<span data-ttu-id="30a55-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="30a55-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30a55-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="30a55-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="30a55-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="30a55-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="30a55-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="30a55-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="30a55-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="30a55-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="30a55-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="30a55-119">Text value</span></span>

<span data-ttu-id="30a55-120">Une valeur de texte **true** indique que le message doit être une réponse automatique afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="30a55-120">A text value of **true** indicates that the message must be an automatic reply in order for the condition or exception to apply.</span></span> <span data-ttu-id="30a55-121">La valeur **false** indique que le message ne doit pas être une réponse automatique afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="30a55-121">A value of **false** indicates that the message does not have to be an automatic reply in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="30a55-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="30a55-122">Remarks</span></span>

<span data-ttu-id="30a55-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="30a55-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30a55-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="30a55-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30a55-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="30a55-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="30a55-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="30a55-126">Schema Name</span></span>  <br/> |<span data-ttu-id="30a55-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="30a55-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="30a55-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="30a55-128">Validation File</span></span>  <br/> |<span data-ttu-id="30a55-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="30a55-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30a55-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="30a55-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="30a55-131">True</span><span class="sxs-lookup"><span data-stu-id="30a55-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30a55-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="30a55-132">See also</span></span>



- [<span data-ttu-id="30a55-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="30a55-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

