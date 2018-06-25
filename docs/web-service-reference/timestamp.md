---
title: Horodatage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeStamp
api_type:
- schema
ms.assetid: 5eae859a-5a74-4bf6-b196-d1b2fd38501a
description: L’élément d’horodatage représente l’horodatage d’un événement de boîte aux lettres.
ms.openlocfilehash: d020d9a4cf3a128d26e0ff2b83be9f3deb024339
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838767"
---
# <a name="timestamp"></a><span data-ttu-id="585be-103">Horodatage</span><span class="sxs-lookup"><span data-stu-id="585be-103">TimeStamp</span></span>

<span data-ttu-id="585be-104">L’élément **d’horodatage** représente l’horodatage d’un événement de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="585be-104">The **Timestamp** element represents the timestamp of a mailbox event.</span></span> 
  
```xml
<TimeStamp/>
```

 <span data-ttu-id="585be-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="585be-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="585be-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="585be-106">Attributes and elements</span></span>

<span data-ttu-id="585be-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="585be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="585be-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="585be-108">Attributes</span></span>

<span data-ttu-id="585be-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="585be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="585be-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="585be-110">Child elements</span></span>

<span data-ttu-id="585be-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="585be-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="585be-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="585be-112">Parent elements</span></span>

|<span data-ttu-id="585be-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="585be-113">**Element**</span></span>|<span data-ttu-id="585be-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="585be-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="585be-115">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="585be-115">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="585be-116">Représente un événement où un élément ou un dossier est copié.</span><span class="sxs-lookup"><span data-stu-id="585be-116">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="585be-117">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="585be-117">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="585be-118">Représente un événement dans lequel un élément ou un dossier est créé.</span><span class="sxs-lookup"><span data-stu-id="585be-118">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="585be-119">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="585be-119">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="585be-120">Représente un événement de suppression d’un élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="585be-120">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="585be-121">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="585be-121">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="585be-122">Représente un événement où un élément ou un dossier est modifié.</span><span class="sxs-lookup"><span data-stu-id="585be-122">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="585be-123">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="585be-123">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="585be-124">Représente un événement où un élément ou un dossier est déplacé à partir du dossier parent d’un vers un autre dossier parent.</span><span class="sxs-lookup"><span data-stu-id="585be-124">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="585be-125">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="585be-125">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="585be-126">Représente un événement déclenché par un nouvel élément de messagerie dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="585be-126">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="585be-127">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="585be-127">Text value</span></span>

<span data-ttu-id="585be-128">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="585be-128">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="585be-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="585be-129">Remarks</span></span>

<span data-ttu-id="585be-130">Cet élément est principalement disponible pour une utilisation dans la détermination de client de la fréquence des événements.</span><span class="sxs-lookup"><span data-stu-id="585be-130">This element is primarily available for use in client determination of event frequency.</span></span> <span data-ttu-id="585be-131">Il n’est pas présent dans [StatusEvent](statusevent.md).</span><span class="sxs-lookup"><span data-stu-id="585be-131">This is not present in [StatusEvent](statusevent.md).</span></span>
  
<span data-ttu-id="585be-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="585be-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="585be-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="585be-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="585be-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="585be-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="585be-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="585be-135">Schema name</span></span>  <br/> |<span data-ttu-id="585be-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="585be-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="585be-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="585be-137">Validation file</span></span>  <br/> |<span data-ttu-id="585be-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="585be-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="585be-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="585be-139">Can be empty</span></span>  <br/> |<span data-ttu-id="585be-140">False</span><span class="sxs-lookup"><span data-stu-id="585be-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="585be-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="585be-141">See also</span></span>



[<span data-ttu-id="585be-142">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="585be-142">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="585be-143">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="585be-143">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="585be-144">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="585be-144">Unsubscribe operation</span></span>](unsubscribe-operation.md)

