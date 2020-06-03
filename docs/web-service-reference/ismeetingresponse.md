---
title: IsMeetingResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeetingResponse
api_type:
- schema
ms.assetid: 85090943-81c6-4fbe-a2db-007dced6a4cf
description: L’élément IsMeetngResponsequest indique si les messages entrants doivent être une réponse à une demande de réunion afin que la condition ou l’exception s’applique.
ms.openlocfilehash: 40714b7e926768f55207d870b79f21f07163bb37
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465932"
---
# <a name="ismeetingresponse"></a><span data-ttu-id="eebb1-103">IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="eebb1-103">IsMeetingResponse</span></span>

<span data-ttu-id="eebb1-104">L’élément **IsMeetngResponsequest** indique si les messages entrants doivent être une réponse à une demande de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="eebb1-104">The **IsMeetngResponsequest** element indicates whether incoming messages must be a meeting response in order for the condition or exception to apply.</span></span> 
  
```XML
<IsMeetingResponse/>true | false</IsMeetingResponse>
```

 <span data-ttu-id="eebb1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="eebb1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eebb1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="eebb1-106">Attributes and elements</span></span>

<span data-ttu-id="eebb1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="eebb1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eebb1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="eebb1-108">Attributes</span></span>

<span data-ttu-id="eebb1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="eebb1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eebb1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="eebb1-110">Child elements</span></span>

<span data-ttu-id="eebb1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="eebb1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eebb1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="eebb1-112">Parent elements</span></span>

|<span data-ttu-id="eebb1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eebb1-113">**Element**</span></span>|<span data-ttu-id="eebb1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="eebb1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eebb1-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="eebb1-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="eebb1-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="eebb1-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="eebb1-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="eebb1-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="eebb1-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="eebb1-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eebb1-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="eebb1-119">Text value</span></span>

<span data-ttu-id="eebb1-120">Une valeur de texte **true** indique que le message doit être une réponse à une demande de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="eebb1-120">A text value of **true** indicates that the message must be a meeting response in order for the condition or exception to apply.</span></span> <span data-ttu-id="eebb1-121">Une valeur de texte **false** indique que le message ne doit pas être une réponse de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="eebb1-121">A text value of **false** indicates that the message must not be a meeting response in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="eebb1-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="eebb1-122">Remarks</span></span>

<span data-ttu-id="eebb1-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="eebb1-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eebb1-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="eebb1-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eebb1-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="eebb1-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="eebb1-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="eebb1-126">Schema Name</span></span>  <br/> |<span data-ttu-id="eebb1-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="eebb1-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="eebb1-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="eebb1-128">Validation File</span></span>  <br/> |<span data-ttu-id="eebb1-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="eebb1-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eebb1-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="eebb1-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="eebb1-131">True</span><span class="sxs-lookup"><span data-stu-id="eebb1-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eebb1-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="eebb1-132">See also</span></span>



- [<span data-ttu-id="eebb1-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="eebb1-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

