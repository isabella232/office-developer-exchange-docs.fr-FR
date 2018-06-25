---
title: FolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: L’élément FolderIds contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers pour copier, déplacer, obtenir, supprimer ou contrôler les notifications d’événements.
ms.openlocfilehash: 911a74ca778ee988c270c16c67620a40656d82d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756449"
---
# <a name="folderids"></a><span data-ttu-id="464f3-103">FolderIds</span><span class="sxs-lookup"><span data-stu-id="464f3-103">FolderIds</span></span>

<span data-ttu-id="464f3-104">L’élément **FolderIds** contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers pour copier, déplacer, obtenir, supprimer ou contrôler les notifications d’événements.</span><span class="sxs-lookup"><span data-stu-id="464f3-104">The **FolderIds** element contains an array of folder identifiers that are used to identify folders to copy, move, get, delete, or monitor for event notifications.</span></span> 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 <span data-ttu-id="464f3-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="464f3-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="464f3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="464f3-106">Attributes and elements</span></span>

<span data-ttu-id="464f3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="464f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="464f3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="464f3-108">Attributes</span></span>

<span data-ttu-id="464f3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="464f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="464f3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="464f3-110">Child elements</span></span>

|<span data-ttu-id="464f3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="464f3-111">**Element**</span></span>|<span data-ttu-id="464f3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="464f3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="464f3-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="464f3-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="464f3-114">Contient la clé d’identificateur et de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="464f3-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="464f3-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="464f3-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="464f3-116">Identifie les dossiers Microsoft Exchange Server qui peuvent être référencés par un nom.</span><span class="sxs-lookup"><span data-stu-id="464f3-116">Identifies Microsoft Exchange Server folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="464f3-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="464f3-117">Parent elements</span></span>

|<span data-ttu-id="464f3-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="464f3-118">**Element**</span></span>|<span data-ttu-id="464f3-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="464f3-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="464f3-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="464f3-120">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="464f3-121">Définit une demande pour obtenir un dossier à partir de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="464f3-121">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="464f3-122">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/GetFolder`</span><span class="sxs-lookup"><span data-stu-id="464f3-122">The following is the XPath expression to this element:  `/GetFolder`</span></span> <br/> |
|[<span data-ttu-id="464f3-123">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="464f3-123">DeleteFolder</span></span>](deletefolder.md) <br/> |<span data-ttu-id="464f3-124">Définit une demande pour supprimer des dossiers de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="464f3-124">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="464f3-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/DeleteFolder`</span><span class="sxs-lookup"><span data-stu-id="464f3-125">The following is the XPath expression to this element:  `/DeleteFolder`</span></span> <br/> |
|[<span data-ttu-id="464f3-126">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="464f3-126">EmptyFolder</span></span>](emptyfolder.md) <br/> |<span data-ttu-id="464f3-127">Définit une demande pour supprimer des dossiers de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="464f3-127">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="464f3-128">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/EmptyFolder`</span><span class="sxs-lookup"><span data-stu-id="464f3-128">The following is the XPath expression to this element:  `/EmptyFolder`</span></span> <br/> |
|[<span data-ttu-id="464f3-129">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="464f3-129">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="464f3-130">Définit une demande de déplacement d’un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="464f3-130">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="464f3-131">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/MoveFolder`</span><span class="sxs-lookup"><span data-stu-id="464f3-131">The following is the XPath expression to this element:  `/MoveFolder`</span></span> <br/> |
|[<span data-ttu-id="464f3-132">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="464f3-132">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="464f3-133">Définit une demande pour copier un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="464f3-133">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="464f3-134">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/CopyFolder`</span><span class="sxs-lookup"><span data-stu-id="464f3-134">The following is the XPath expression to this element:  `/CopyFolder`</span></span> <br/> |
|[<span data-ttu-id="464f3-135">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="464f3-135">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="464f3-136">Représente un abonnement à un abonnement de notification push d’événements.</span><span class="sxs-lookup"><span data-stu-id="464f3-136">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="464f3-137">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="464f3-137">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="464f3-138">Représente un abonnement à un abonnement de notification d’événement de type pull.</span><span class="sxs-lookup"><span data-stu-id="464f3-138">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="464f3-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="464f3-139">Remarks</span></span>

<span data-ttu-id="464f3-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="464f3-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="464f3-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="464f3-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="464f3-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="464f3-142">Namespace</span></span>  <br/> |<span data-ttu-id="464f3-143">http://schemas.microsoft.com/exchange/services/2006/messages et http://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="464f3-143">http://schemas.microsoft.com/exchange/services/2006/messages and http://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="464f3-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="464f3-144">Schema Name</span></span>  <br/> |<span data-ttu-id="464f3-145">Schéma des messages ; Schéma de types</span><span class="sxs-lookup"><span data-stu-id="464f3-145">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="464f3-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="464f3-146">Validation File</span></span>  <br/> |<span data-ttu-id="464f3-147">Messages.xsd ; Types.xsd</span><span class="sxs-lookup"><span data-stu-id="464f3-147">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="464f3-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="464f3-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="464f3-149">False</span><span class="sxs-lookup"><span data-stu-id="464f3-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="464f3-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="464f3-150">See also</span></span>



[<span data-ttu-id="464f3-151">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="464f3-151">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="464f3-152">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="464f3-152">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="464f3-153">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="464f3-153">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="464f3-154">Opération CopyFolder</span><span class="sxs-lookup"><span data-stu-id="464f3-154">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="464f3-155">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="464f3-155">Subscribe operation</span></span>](subscribe-operation.md)

