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
description: L’élément FolderIds contient un tableau des identificateurs de dossier utilisés pour identifier les dossiers à copier, déplacer, obtenir, supprimer ou surveiller les notifications d’événement.
ms.openlocfilehash: ff0476f72c7da088bd2b39f58ab560dcc82197e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530992"
---
# <a name="folderids"></a><span data-ttu-id="da6dc-103">FolderIds</span><span class="sxs-lookup"><span data-stu-id="da6dc-103">FolderIds</span></span>

<span data-ttu-id="da6dc-104">L’élément **FolderIds** contient un tableau des identificateurs de dossier utilisés pour identifier les dossiers à copier, déplacer, obtenir, supprimer ou surveiller les notifications d’événement.</span><span class="sxs-lookup"><span data-stu-id="da6dc-104">The **FolderIds** element contains an array of folder identifiers that are used to identify folders to copy, move, get, delete, or monitor for event notifications.</span></span> 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 <span data-ttu-id="da6dc-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="da6dc-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da6dc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="da6dc-106">Attributes and elements</span></span>

<span data-ttu-id="da6dc-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="da6dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da6dc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="da6dc-108">Attributes</span></span>

<span data-ttu-id="da6dc-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="da6dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da6dc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="da6dc-110">Child elements</span></span>

|<span data-ttu-id="da6dc-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="da6dc-111">**Element**</span></span>|<span data-ttu-id="da6dc-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="da6dc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da6dc-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="da6dc-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="da6dc-114">Contient l’identificateur et la clé de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="da6dc-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="da6dc-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="da6dc-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="da6dc-116">Identifie les dossiers Microsoft Exchange Server qui peuvent être référencés par nom.</span><span class="sxs-lookup"><span data-stu-id="da6dc-116">Identifies Microsoft Exchange Server folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="da6dc-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="da6dc-117">Parent elements</span></span>

|<span data-ttu-id="da6dc-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="da6dc-118">**Element**</span></span>|<span data-ttu-id="da6dc-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="da6dc-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da6dc-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="da6dc-120">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="da6dc-121">Définit une demande d’obtention d’un dossier à partir de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="da6dc-121">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="da6dc-122">Voici l’expression XPath de cet élément :`/GetFolder`</span><span class="sxs-lookup"><span data-stu-id="da6dc-122">The following is the XPath expression to this element:  `/GetFolder`</span></span> <br/> |
|[<span data-ttu-id="da6dc-123">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="da6dc-123">DeleteFolder</span></span>](deletefolder.md) <br/> |<span data-ttu-id="da6dc-124">Définit une demande de suppression de dossiers de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="da6dc-124">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="da6dc-125">Voici l’expression XPath de cet élément :`/DeleteFolder`</span><span class="sxs-lookup"><span data-stu-id="da6dc-125">The following is the XPath expression to this element:  `/DeleteFolder`</span></span> <br/> |
|[<span data-ttu-id="da6dc-126">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="da6dc-126">EmptyFolder</span></span>](emptyfolder.md) <br/> |<span data-ttu-id="da6dc-127">Définit une demande de suppression de dossiers de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="da6dc-127">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="da6dc-128">Voici l’expression XPath de cet élément :`/EmptyFolder`</span><span class="sxs-lookup"><span data-stu-id="da6dc-128">The following is the XPath expression to this element:  `/EmptyFolder`</span></span> <br/> |
|[<span data-ttu-id="da6dc-129">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="da6dc-129">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="da6dc-130">Définit une demande de déplacement d’un dossier dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="da6dc-130">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="da6dc-131">Voici l’expression XPath de cet élément :`/MoveFolder`</span><span class="sxs-lookup"><span data-stu-id="da6dc-131">The following is the XPath expression to this element:  `/MoveFolder`</span></span> <br/> |
|[<span data-ttu-id="da6dc-132">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="da6dc-132">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="da6dc-133">Définit une demande de copie d’un dossier dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="da6dc-133">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="da6dc-134">Voici l’expression XPath de cet élément :`/CopyFolder`</span><span class="sxs-lookup"><span data-stu-id="da6dc-134">The following is the XPath expression to this element:  `/CopyFolder`</span></span> <br/> |
|[<span data-ttu-id="da6dc-135">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="da6dc-135">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="da6dc-136">Représente un abonnement à un abonnement de notification d’événement basé sur un type de message.</span><span class="sxs-lookup"><span data-stu-id="da6dc-136">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="da6dc-137">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="da6dc-137">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="da6dc-138">Représente un abonnement à un abonnement de notification d’événement basé sur l’extraction.</span><span class="sxs-lookup"><span data-stu-id="da6dc-138">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="da6dc-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="da6dc-139">Remarks</span></span>

<span data-ttu-id="da6dc-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="da6dc-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da6dc-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="da6dc-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da6dc-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="da6dc-142">Namespace</span></span>  <br/> |<span data-ttu-id="da6dc-143">https://schemas.microsoft.com/exchange/services/2006/messages et https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="da6dc-143">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="da6dc-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="da6dc-144">Schema Name</span></span>  <br/> |<span data-ttu-id="da6dc-145">Schéma des messages ; Schéma de types</span><span class="sxs-lookup"><span data-stu-id="da6dc-145">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="da6dc-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="da6dc-146">Validation File</span></span>  <br/> |<span data-ttu-id="da6dc-147">Messages. xsd ; Types. xsd</span><span class="sxs-lookup"><span data-stu-id="da6dc-147">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da6dc-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="da6dc-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="da6dc-149">False</span><span class="sxs-lookup"><span data-stu-id="da6dc-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da6dc-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="da6dc-150">See also</span></span>



[<span data-ttu-id="da6dc-151">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="da6dc-151">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="da6dc-152">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="da6dc-152">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="da6dc-153">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="da6dc-153">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="da6dc-154">CopyFolder, opération</span><span class="sxs-lookup"><span data-stu-id="da6dc-154">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="da6dc-155">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="da6dc-155">Subscribe operation</span></span>](subscribe-operation.md)

