---
title: MoveToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveToFolder
api_type:
- schema
ms.assetid: 991673b9-b627-4848-bfba-59a187b8575f
description: L’élément MoveToFolder Spécifie l’identificateur du dossier vers lequel les éléments de messagerie électronique peuvent être déplacés.
ms.openlocfilehash: 058f008b348d49c932bf334dd3379f02d06154e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828494"
---
# <a name="movetofolder"></a><span data-ttu-id="78773-103">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="78773-103">MoveToFolder</span></span>

<span data-ttu-id="78773-104">L’élément **MoveToFolder** Spécifie l’identificateur du dossier vers lequel les éléments de messagerie électronique peuvent être déplacés.</span><span class="sxs-lookup"><span data-stu-id="78773-104">The **MoveToFolder** element specifies the identifier of the folder to which email items can be moved.</span></span> 
  
```XML
<MoveToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</MoveToFolder>
```

 <span data-ttu-id="78773-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="78773-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78773-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="78773-106">Attributes and elements</span></span>

<span data-ttu-id="78773-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="78773-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78773-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="78773-108">Attributes</span></span>

<span data-ttu-id="78773-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="78773-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78773-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="78773-110">Child elements</span></span>

|<span data-ttu-id="78773-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="78773-111">**Element**</span></span>|<span data-ttu-id="78773-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="78773-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78773-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="78773-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="78773-114">Contient l’identificateur d’un dossier de destination pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="78773-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="78773-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="78773-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="78773-116">Identifie un dossier nommé pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="78773-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="78773-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="78773-117">Parent elements</span></span>

|<span data-ttu-id="78773-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="78773-118">**Element**</span></span>|<span data-ttu-id="78773-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="78773-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78773-120">Actions</span><span class="sxs-lookup"><span data-stu-id="78773-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="78773-121">Représente l’ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies...</span><span class="sxs-lookup"><span data-stu-id="78773-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled..</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="78773-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="78773-122">Text value</span></span>

<span data-ttu-id="78773-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="78773-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="78773-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="78773-124">Remarks</span></span>

<span data-ttu-id="78773-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="78773-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78773-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="78773-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78773-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="78773-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="78773-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="78773-128">Schema Name</span></span>  <br/> |<span data-ttu-id="78773-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="78773-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="78773-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="78773-130">Validation File</span></span>  <br/> |<span data-ttu-id="78773-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="78773-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="78773-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="78773-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="78773-133">True</span><span class="sxs-lookup"><span data-stu-id="78773-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78773-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="78773-134">See also</span></span>



[<span data-ttu-id="78773-135">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="78773-135">CopyToFolder</span></span>](copytofolder.md)


- [<span data-ttu-id="78773-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="78773-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

