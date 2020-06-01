---
title: IsMeetingRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeetingRequest
api_type:
- schema
ms.assetid: 72102a55-fd51-4ec9-abce-9a4ec45b86d2
description: L’élément IsMeetngRequest indique si les messages entrants doivent être une demande de réunion afin que la condition ou l’exception s’applique.
ms.openlocfilehash: 8b4969faaeb7dfa98edbf4fe8747e8b783808313
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465960"
---
# <a name="ismeetingrequest"></a><span data-ttu-id="c20ed-103">IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c20ed-103">IsMeetingRequest</span></span>

<span data-ttu-id="c20ed-104">L’élément **IsMeetngRequest** indique si les messages entrants doivent être une demande de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="c20ed-104">The **IsMeetngRequest** element indicates whether incoming messages must be a meeting request in order for the condition or exception to apply.</span></span> 
  
```XML
<IsMeetingRequest>true | false</IsMeetingRequest>
```

 <span data-ttu-id="c20ed-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c20ed-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c20ed-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c20ed-106">Attributes and elements</span></span>

<span data-ttu-id="c20ed-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c20ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c20ed-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c20ed-108">Attributes</span></span>

<span data-ttu-id="c20ed-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c20ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c20ed-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c20ed-110">Child elements</span></span>

<span data-ttu-id="c20ed-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c20ed-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c20ed-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c20ed-112">Parent elements</span></span>

|<span data-ttu-id="c20ed-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c20ed-113">**Element**</span></span>|<span data-ttu-id="c20ed-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="c20ed-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c20ed-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="c20ed-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="c20ed-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="c20ed-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="c20ed-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="c20ed-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="c20ed-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="c20ed-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c20ed-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="c20ed-119">Text value</span></span>

<span data-ttu-id="c20ed-120">Une valeur de texte **true** indique que le message doit être une demande de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="c20ed-120">A text value of **true** indicates that the message must be a meeting request in order for the condition or exception to apply.</span></span> <span data-ttu-id="c20ed-121">La valeur **false** indique que le message ne doit pas être une demande de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="c20ed-121">A value of **false** indicates that the message must not be a meeting request in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c20ed-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="c20ed-122">Remarks</span></span>

<span data-ttu-id="c20ed-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c20ed-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c20ed-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c20ed-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c20ed-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c20ed-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c20ed-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c20ed-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c20ed-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c20ed-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c20ed-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c20ed-128">Validation File</span></span>  <br/> |<span data-ttu-id="c20ed-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c20ed-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c20ed-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c20ed-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c20ed-131">True</span><span class="sxs-lookup"><span data-stu-id="c20ed-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c20ed-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c20ed-132">See also</span></span>



- [<span data-ttu-id="c20ed-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c20ed-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

