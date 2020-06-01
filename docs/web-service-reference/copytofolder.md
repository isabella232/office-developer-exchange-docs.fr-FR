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
description: L’élément CopyToFolder, spécifie l’identificateur du dossier dans lequel les éléments de courrier électronique peuvent être copiés.
ms.openlocfilehash: 7cdda0f9769f909255c9b76f78ac7094a8dfc8f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463173"
---
# <a name="copytofolder"></a><span data-ttu-id="5ff1c-103">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="5ff1c-103">CopyToFolder</span></span>

<span data-ttu-id="5ff1c-104">L’élément **CopyToFolder,** spécifie l’identificateur du dossier dans lequel les éléments de courrier électronique peuvent être copiés.</span><span class="sxs-lookup"><span data-stu-id="5ff1c-104">The **CopyToFolder** element specifies the identifier of the folder that email items can be copied to.</span></span> 
  
```XML
<CopyToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</CopyToFolder>
```

 <span data-ttu-id="5ff1c-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="5ff1c-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ff1c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5ff1c-106">Attributes and elements</span></span>

<span data-ttu-id="5ff1c-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5ff1c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ff1c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5ff1c-108">Attributes</span></span>

<span data-ttu-id="5ff1c-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5ff1c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ff1c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5ff1c-110">Child elements</span></span>

|<span data-ttu-id="5ff1c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5ff1c-111">**Element**</span></span>|<span data-ttu-id="5ff1c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ff1c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ff1c-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="5ff1c-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="5ff1c-114">Contient l’identificateur d’un dossier de destination pour un élément ou un dossier copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="5ff1c-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="5ff1c-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="5ff1c-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="5ff1c-116">Identifie un dossier de destination nommé pour un élément ou un dossier copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="5ff1c-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5ff1c-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5ff1c-117">Parent elements</span></span>

|<span data-ttu-id="5ff1c-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5ff1c-118">**Element**</span></span>|<span data-ttu-id="5ff1c-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ff1c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ff1c-120">Actions</span><span class="sxs-lookup"><span data-stu-id="5ff1c-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="5ff1c-121">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="5ff1c-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5ff1c-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5ff1c-122">Text value</span></span>

<span data-ttu-id="5ff1c-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5ff1c-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5ff1c-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="5ff1c-124">Remarks</span></span>

<span data-ttu-id="5ff1c-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5ff1c-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ff1c-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5ff1c-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ff1c-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5ff1c-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5ff1c-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5ff1c-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5ff1c-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="5ff1c-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5ff1c-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5ff1c-130">Validation File</span></span>  <br/> |<span data-ttu-id="5ff1c-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5ff1c-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5ff1c-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5ff1c-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ff1c-133">True</span><span class="sxs-lookup"><span data-stu-id="5ff1c-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ff1c-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5ff1c-134">See also</span></span>



[<span data-ttu-id="5ff1c-135">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="5ff1c-135">MoveToFolder</span></span>](movetofolder.md)


- [<span data-ttu-id="5ff1c-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5ff1c-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

