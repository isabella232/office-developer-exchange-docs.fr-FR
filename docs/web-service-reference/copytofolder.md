---
title: CopyToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyToFolder
api_type:
- schema
ms.assetid: 6fd8a6b8-d813-43ff-991b-0e9e782fe00e
description: L’élément CopyToFolder Spécifie l’identificateur du dossier e-mail éléments peuvent être copiés.
ms.openlocfilehash: b641c23b7aed11ae85157e2ed01cfa9d61d07e0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755670"
---
# <a name="copytofolder"></a><span data-ttu-id="02a05-103">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="02a05-103">CopyToFolder</span></span>

<span data-ttu-id="02a05-104">L’élément **CopyToFolder** Spécifie l’identificateur du dossier e-mail éléments peuvent être copiés.</span><span class="sxs-lookup"><span data-stu-id="02a05-104">The **CopyToFolder** element specifies the identifier of the folder that email items can be copied to.</span></span> 
  
```XML
<CopyToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</CopyToFolder>
```

 <span data-ttu-id="02a05-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="02a05-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02a05-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="02a05-106">Attributes and elements</span></span>

<span data-ttu-id="02a05-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="02a05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02a05-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="02a05-108">Attributes</span></span>

<span data-ttu-id="02a05-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="02a05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02a05-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="02a05-110">Child elements</span></span>

|<span data-ttu-id="02a05-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="02a05-111">**Element**</span></span>|<span data-ttu-id="02a05-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="02a05-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02a05-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="02a05-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="02a05-114">Contient l’identificateur d’un dossier de destination pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="02a05-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="02a05-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="02a05-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="02a05-116">Identifie un dossier nommé pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="02a05-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02a05-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="02a05-117">Parent elements</span></span>

|<span data-ttu-id="02a05-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="02a05-118">**Element**</span></span>|<span data-ttu-id="02a05-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="02a05-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02a05-120">Actions</span><span class="sxs-lookup"><span data-stu-id="02a05-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="02a05-121">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="02a05-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="02a05-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="02a05-122">Text value</span></span>

<span data-ttu-id="02a05-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="02a05-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="02a05-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="02a05-124">Remarks</span></span>

<span data-ttu-id="02a05-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="02a05-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02a05-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="02a05-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02a05-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="02a05-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="02a05-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="02a05-128">Schema Name</span></span>  <br/> |<span data-ttu-id="02a05-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="02a05-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="02a05-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="02a05-130">Validation File</span></span>  <br/> |<span data-ttu-id="02a05-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="02a05-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02a05-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="02a05-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="02a05-133">True</span><span class="sxs-lookup"><span data-stu-id="02a05-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02a05-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="02a05-134">See also</span></span>



[<span data-ttu-id="02a05-135">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="02a05-135">MoveToFolder</span></span>](movetofolder.md)


- [<span data-ttu-id="02a05-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="02a05-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

