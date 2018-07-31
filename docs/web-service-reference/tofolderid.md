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
ms.openlocfilehash: 9d2fd6c177711cfe3a5d3415320440259e2f5289
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353657"
---
# <a name="tofolderid"></a><span data-ttu-id="55b40-103">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="55b40-103">ToFolderId</span></span>

<span data-ttu-id="55b40-104">L’élément **ToFolderId** représente le dossier de destination pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="55b40-104">The **ToFolderId** element represents the destination folder for a copied or moved item or folder.</span></span> 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

```xml
<ToFolderId>
   <DistinguishedFolderId/>
</ToFolderId>
```

<span data-ttu-id="55b40-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="55b40-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="55b40-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="55b40-106">Attributes and elements</span></span>

<span data-ttu-id="55b40-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="55b40-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55b40-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="55b40-108">Attributes</span></span>

<span data-ttu-id="55b40-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="55b40-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55b40-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="55b40-110">Child elements</span></span>

|<span data-ttu-id="55b40-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="55b40-111">**Element**</span></span>|<span data-ttu-id="55b40-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="55b40-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55b40-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="55b40-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="55b40-114">Contient l’identificateur d’un dossier de destination pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="55b40-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="55b40-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="55b40-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="55b40-116">Identifie un dossier nommé pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="55b40-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55b40-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="55b40-117">Parent elements</span></span>

|<span data-ttu-id="55b40-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="55b40-118">**Element**</span></span>|<span data-ttu-id="55b40-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="55b40-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55b40-120">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="55b40-120">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="55b40-121">Définit une demande de déplacement d’un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="55b40-121">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="55b40-122">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="55b40-122">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveFolder` <br/> |
|[<span data-ttu-id="55b40-123">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="55b40-123">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="55b40-124">Définit une demande pour copier un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="55b40-124">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="55b40-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="55b40-125">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyFolder` <br/> |
|[<span data-ttu-id="55b40-126">MoveItem</span><span class="sxs-lookup"><span data-stu-id="55b40-126">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="55b40-127">Définit une demande de déplacement d’un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="55b40-127">Defines a request to move an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="55b40-128">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="55b40-128">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="55b40-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="55b40-129">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="55b40-130">Définit une demande pour copier un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="55b40-130">Defines a request to copy an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="55b40-131">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="55b40-131">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55b40-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="55b40-132">Remarks</span></span>

<span data-ttu-id="55b40-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="55b40-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55b40-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="55b40-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55b40-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="55b40-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="55b40-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="55b40-136">Schema Name</span></span>  <br/> |<span data-ttu-id="55b40-137">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="55b40-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="55b40-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="55b40-138">Validation File</span></span>  <br/> |<span data-ttu-id="55b40-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="55b40-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="55b40-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="55b40-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="55b40-141">False</span><span class="sxs-lookup"><span data-stu-id="55b40-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55b40-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="55b40-142">See also</span></span>

- [<span data-ttu-id="55b40-143">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="55b40-143">MoveFolder operation</span></span>](movefolder-operation.md)  
- [<span data-ttu-id="55b40-144">Opération CopyFolder</span><span class="sxs-lookup"><span data-stu-id="55b40-144">CopyFolder operation</span></span>](copyfolder-operation.md) 
- [<span data-ttu-id="55b40-145">Opération MoveItem</span><span class="sxs-lookup"><span data-stu-id="55b40-145">MoveItem operation</span></span>](moveitem-operation.md) 
- [<span data-ttu-id="55b40-146">Opération CopyItem</span><span class="sxs-lookup"><span data-stu-id="55b40-146">CopyItem operation</span></span>](copyitem-operation.md)

