---
title: MoveFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolder
api_type:
- schema
ms.assetid: f2bb0a73-94d7-4bc7-8902-bd9c69120221
description: L’élément MoveFolder définit une demande de déplacement d’un dossier dans la banque d’informations Exchange.
ms.openlocfilehash: 42a990ced18cc13c7694042df786d33c018f346c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828485"
---
# <a name="movefolder"></a><span data-ttu-id="27124-103">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="27124-103">MoveFolder</span></span>

<span data-ttu-id="27124-104">L’élément **MoveFolder** définit une demande de déplacement d’un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="27124-104">The **MoveFolder** element defines a request to move a folder in the Exchange store.</span></span> 
  
```xml
<MoveFolder>
   <ToFolderId/>
   <FolderIds/>
</MoveFolder>
```

 <span data-ttu-id="27124-105">**MoveFolderType**</span><span class="sxs-lookup"><span data-stu-id="27124-105">**MoveFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27124-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="27124-106">Attributes and elements</span></span>

<span data-ttu-id="27124-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="27124-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27124-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="27124-108">Attributes</span></span>

<span data-ttu-id="27124-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="27124-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27124-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="27124-110">Child elements</span></span>

|<span data-ttu-id="27124-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="27124-111">**Element**</span></span>|<span data-ttu-id="27124-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="27124-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27124-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="27124-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="27124-114">Représente le dossier de destination pour un dossier déplacé.</span><span class="sxs-lookup"><span data-stu-id="27124-114">Represents the destination folder for a moved folder.</span></span>  <br/> |
|[<span data-ttu-id="27124-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="27124-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="27124-116">Contient un tableau de dossiers à déplacer vers le dossier identifié par l’élément [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="27124-116">Contains an array of folders to move to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27124-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="27124-117">Parent elements</span></span>

<span data-ttu-id="27124-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="27124-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="27124-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="27124-119">Remarks</span></span>

<span data-ttu-id="27124-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="27124-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27124-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="27124-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27124-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="27124-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27124-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="27124-123">Schema Name</span></span>  <br/> |<span data-ttu-id="27124-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="27124-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="27124-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="27124-125">Validation File</span></span>  <br/> |<span data-ttu-id="27124-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="27124-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27124-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="27124-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="27124-128">False</span><span class="sxs-lookup"><span data-stu-id="27124-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27124-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="27124-129">See also</span></span>



[<span data-ttu-id="27124-130">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="27124-130">MoveFolder operation</span></span>](movefolder-operation.md)

