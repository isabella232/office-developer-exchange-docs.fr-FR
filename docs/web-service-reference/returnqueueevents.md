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
description: L’élément ReturnQueueEvents indique que la personne qui exécute la tâche est dotée d’un rôle privilégié.
ms.openlocfilehash: 9d07bc8c3d32f1cd532febaf4ae04e4a2d31d243
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466590"
---
# <a name="returnqueueevents"></a><span data-ttu-id="59e5a-103">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="59e5a-103">ReturnQueueEvents</span></span>

<span data-ttu-id="59e5a-104">L’élément **ReturnQueueEvents** indique que la personne qui exécute la tâche est dotée d’un rôle privilégié.</span><span class="sxs-lookup"><span data-stu-id="59e5a-104">The **ReturnQueueEvents** element indicates that the person who is running the task is in a privileged role.</span></span> 
  
```XML
<ReturnQueueEvents>true | false</ReturnQueueEvents>
```

 <span data-ttu-id="59e5a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="59e5a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59e5a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="59e5a-106">Attributes and elements</span></span>

<span data-ttu-id="59e5a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="59e5a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59e5a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="59e5a-108">Attributes</span></span>

<span data-ttu-id="59e5a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="59e5a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59e5a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="59e5a-110">Child elements</span></span>

<span data-ttu-id="59e5a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59e5a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="59e5a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="59e5a-112">Parent elements</span></span>

|<span data-ttu-id="59e5a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59e5a-113">**Element**</span></span>|<span data-ttu-id="59e5a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="59e5a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59e5a-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="59e5a-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="59e5a-116">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) afin de récupérer le rapport de suivi complet des messages pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="59e5a-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="59e5a-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="59e5a-117">Text value</span></span>

<span data-ttu-id="59e5a-118">Une valeur de texte qui représente une valeur Boolean est requise.</span><span class="sxs-lookup"><span data-stu-id="59e5a-118">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="59e5a-119">La valeur **true** indique que la personne qui exécute la tâche est dotée d’un rôle privilégié ; la valeur **false** indique que la personne qui exécute la tâche ne dispose pas d’un rôle privilégié.</span><span class="sxs-lookup"><span data-stu-id="59e5a-119">A value of **true** indicates that the person who is running the task is in a privileged role; a value of **false** indicates that the person who is running the task is not in a privileged role.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="59e5a-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="59e5a-120">Remarks</span></span>

<span data-ttu-id="59e5a-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="59e5a-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59e5a-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="59e5a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59e5a-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="59e5a-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="59e5a-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="59e5a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="59e5a-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="59e5a-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="59e5a-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="59e5a-126">Validation File</span></span>  <br/> |<span data-ttu-id="59e5a-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="59e5a-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="59e5a-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="59e5a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="59e5a-129">False</span><span class="sxs-lookup"><span data-stu-id="59e5a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59e5a-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59e5a-130">See also</span></span>



[<span data-ttu-id="59e5a-131">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="59e5a-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="59e5a-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="59e5a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

