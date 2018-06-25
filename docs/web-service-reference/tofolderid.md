---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: L’élément ToFolderId représente le dossier de destination pour un dossier ou un élément copié ou déplacé.
ms.openlocfilehash: a48309f0b7f5c9bf667fc2eb653a0502832bc996
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838734"
---
# <a name="tofolderid"></a><span data-ttu-id="78ec8-103">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="78ec8-103">ToFolderId</span></span>

<span data-ttu-id="78ec8-104">L’élément **ToFolderId** représente le dossier de destination pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="78ec8-104">The **ToFolderId** element represents the destination folder for a copied or moved item or folder.</span></span> 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

 <span data-ttu-id="78ec8-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="78ec8-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78ec8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="78ec8-106">Attributes and elements</span></span>

<span data-ttu-id="78ec8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="78ec8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78ec8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="78ec8-108">Attributes</span></span>

<span data-ttu-id="78ec8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="78ec8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78ec8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="78ec8-110">Child elements</span></span>

|<span data-ttu-id="78ec8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="78ec8-111">**Element**</span></span>|<span data-ttu-id="78ec8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="78ec8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78ec8-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="78ec8-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="78ec8-114">Contient l’identificateur d’un dossier de destination pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="78ec8-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="78ec8-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="78ec8-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="78ec8-116">Identifie un dossier nommé pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="78ec8-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="78ec8-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="78ec8-117">Parent elements</span></span>

|<span data-ttu-id="78ec8-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="78ec8-118">**Element**</span></span>|<span data-ttu-id="78ec8-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="78ec8-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78ec8-120">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="78ec8-120">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="78ec8-121">Définit une demande de déplacement d’un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="78ec8-121">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="78ec8-122">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="78ec8-122">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveFolder` <br/> |
|[<span data-ttu-id="78ec8-123">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="78ec8-123">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="78ec8-124">Définit une demande pour copier un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="78ec8-124">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="78ec8-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="78ec8-125">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyFolder` <br/> |
|[<span data-ttu-id="78ec8-126">MoveItem</span><span class="sxs-lookup"><span data-stu-id="78ec8-126">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="78ec8-127">Définit une demande de déplacement d’un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="78ec8-127">Defines a request to move an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="78ec8-128">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="78ec8-128">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="78ec8-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="78ec8-129">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="78ec8-130">Définit une demande pour copier un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="78ec8-130">Defines a request to copy an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="78ec8-131">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="78ec8-131">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="78ec8-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="78ec8-132">Remarks</span></span>

<span data-ttu-id="78ec8-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="78ec8-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78ec8-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="78ec8-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78ec8-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="78ec8-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="78ec8-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="78ec8-136">Schema Name</span></span>  <br/> |<span data-ttu-id="78ec8-137">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="78ec8-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="78ec8-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="78ec8-138">Validation File</span></span>  <br/> |<span data-ttu-id="78ec8-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="78ec8-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="78ec8-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="78ec8-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="78ec8-141">False</span><span class="sxs-lookup"><span data-stu-id="78ec8-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78ec8-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="78ec8-142">See also</span></span>



[<span data-ttu-id="78ec8-143">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="78ec8-143">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="78ec8-144">Opération CopyFolder</span><span class="sxs-lookup"><span data-stu-id="78ec8-144">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="78ec8-145">Opération MoveItem</span><span class="sxs-lookup"><span data-stu-id="78ec8-145">MoveItem operation</span></span>](moveitem-operation.md)
  
[<span data-ttu-id="78ec8-146">Opération CopyItem</span><span class="sxs-lookup"><span data-stu-id="78ec8-146">CopyItem operation</span></span>](copyitem-operation.md)

