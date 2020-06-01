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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465932"
---
# <a name="ismeetingresponse"></a><span data-ttu-id="89c56-103">IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="89c56-103">IsMeetingResponse</span></span>

<span data-ttu-id="89c56-104">L’élément **IsMeetngResponsequest** indique si les messages entrants doivent être une réponse à une demande de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="89c56-104">The **IsMeetngResponsequest** element indicates whether incoming messages must be a meeting response in order for the condition or exception to apply.</span></span> 
  
```XML
<IsMeetingResponse/>true | false</IsMeetingResponse>
```

 <span data-ttu-id="89c56-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="89c56-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89c56-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="89c56-106">Attributes and elements</span></span>

<span data-ttu-id="89c56-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="89c56-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89c56-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="89c56-108">Attributes</span></span>

<span data-ttu-id="89c56-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="89c56-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89c56-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="89c56-110">Child elements</span></span>

<span data-ttu-id="89c56-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="89c56-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="89c56-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="89c56-112">Parent elements</span></span>

|<span data-ttu-id="89c56-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="89c56-113">**Element**</span></span>|<span data-ttu-id="89c56-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="89c56-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89c56-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="89c56-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="89c56-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="89c56-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="89c56-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="89c56-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="89c56-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="89c56-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="89c56-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="89c56-119">Text value</span></span>

<span data-ttu-id="89c56-120">Une valeur de texte **true** indique que le message doit être une réponse à une demande de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="89c56-120">A text value of **true** indicates that the message must be a meeting response in order for the condition or exception to apply.</span></span> <span data-ttu-id="89c56-121">Une valeur de texte **false** indique que le message ne doit pas être une réponse de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="89c56-121">A text value of **false** indicates that the message must not be a meeting response in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="89c56-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="89c56-122">Remarks</span></span>

<span data-ttu-id="89c56-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="89c56-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89c56-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="89c56-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89c56-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="89c56-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89c56-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="89c56-126">Schema Name</span></span>  <br/> |<span data-ttu-id="89c56-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="89c56-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="89c56-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="89c56-128">Validation File</span></span>  <br/> |<span data-ttu-id="89c56-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="89c56-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89c56-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="89c56-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="89c56-131">True</span><span class="sxs-lookup"><span data-stu-id="89c56-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89c56-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="89c56-132">See also</span></span>



- [<span data-ttu-id="89c56-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="89c56-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

