---
title: ReturnQueueEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReturnQueueEvents
api_type:
- schema
ms.assetid: 69d22417-320c-4c6f-9fb4-2020f2480bb2
description: L’élément ReturnQueueEvents indique que la personne qui exécute la tâche est dans un rôle de privilège.
ms.openlocfilehash: 02f4ca86ffa14117105ec186ae039065cb626670
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829233"
---
# <a name="returnqueueevents"></a><span data-ttu-id="f91a5-103">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="f91a5-103">ReturnQueueEvents</span></span>

<span data-ttu-id="f91a5-104">L’élément **ReturnQueueEvents** indique que la personne qui exécute la tâche est dans un rôle de privilège.</span><span class="sxs-lookup"><span data-stu-id="f91a5-104">The **ReturnQueueEvents** element indicates that the person who is running the task is in a privileged role.</span></span> 
  
```XML
<ReturnQueueEvents>true | false</ReturnQueueEvents>
```

 <span data-ttu-id="f91a5-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f91a5-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f91a5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f91a5-106">Attributes and elements</span></span>

<span data-ttu-id="f91a5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f91a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f91a5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f91a5-108">Attributes</span></span>

<span data-ttu-id="f91a5-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f91a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f91a5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f91a5-110">Child elements</span></span>

<span data-ttu-id="f91a5-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f91a5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f91a5-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f91a5-112">Parent elements</span></span>

|<span data-ttu-id="f91a5-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f91a5-113">**Element**</span></span>|<span data-ttu-id="f91a5-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f91a5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f91a5-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f91a5-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="f91a5-116">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) récupérer le message complet suivi du rapport pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="f91a5-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f91a5-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f91a5-117">Text value</span></span>

<span data-ttu-id="f91a5-118">Une valeur de texte qui représente une valeur Boolean est requise.</span><span class="sxs-lookup"><span data-stu-id="f91a5-118">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="f91a5-119">La valeur **true** indique que la personne qui exécute la tâche est dans un rôle de privilège ; la valeur **false** indique que la personne qui exécute la tâche n’est pas un rôle de privilège.</span><span class="sxs-lookup"><span data-stu-id="f91a5-119">A value of **true** indicates that the person who is running the task is in a privileged role; a value of **false** indicates that the person who is running the task is not in a privileged role.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f91a5-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="f91a5-120">Remarks</span></span>

<span data-ttu-id="f91a5-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f91a5-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f91a5-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f91a5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f91a5-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f91a5-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f91a5-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f91a5-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f91a5-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f91a5-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f91a5-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f91a5-126">Validation File</span></span>  <br/> |<span data-ttu-id="f91a5-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f91a5-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f91a5-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f91a5-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="f91a5-129">False</span><span class="sxs-lookup"><span data-stu-id="f91a5-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f91a5-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f91a5-130">See also</span></span>



[<span data-ttu-id="f91a5-131">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f91a5-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="f91a5-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f91a5-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

