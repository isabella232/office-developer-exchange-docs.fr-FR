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
description: L’élément MoveFolder définit une demande de déplacement d’un dossier dans la Banque d’Exchange.
ms.openlocfilehash: d2fe33a6d7893d45fa116a1516fcc6ab2dea3bcf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457290"
---
# <a name="movefolder"></a><span data-ttu-id="624e6-103">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="624e6-103">MoveFolder</span></span>

<span data-ttu-id="624e6-104">L’élément **MoveFolder** définit une demande de déplacement d’un dossier dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="624e6-104">The **MoveFolder** element defines a request to move a folder in the Exchange store.</span></span> 
  
```xml
<MoveFolder>
   <ToFolderId/>
   <FolderIds/>
</MoveFolder>
```

 <span data-ttu-id="624e6-105">**MoveFolderType**</span><span class="sxs-lookup"><span data-stu-id="624e6-105">**MoveFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="624e6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="624e6-106">Attributes and elements</span></span>

<span data-ttu-id="624e6-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="624e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="624e6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="624e6-108">Attributes</span></span>

<span data-ttu-id="624e6-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="624e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="624e6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="624e6-110">Child elements</span></span>

|<span data-ttu-id="624e6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="624e6-111">**Element**</span></span>|<span data-ttu-id="624e6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="624e6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="624e6-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="624e6-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="624e6-114">Représente le dossier de destination d’un dossier déplacé.</span><span class="sxs-lookup"><span data-stu-id="624e6-114">Represents the destination folder for a moved folder.</span></span>  <br/> |
|[<span data-ttu-id="624e6-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="624e6-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="624e6-116">Contient un tableau de dossiers à déplacer vers le dossier identifié par l’élément [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="624e6-116">Contains an array of folders to move to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="624e6-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="624e6-117">Parent elements</span></span>

<span data-ttu-id="624e6-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="624e6-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="624e6-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="624e6-119">Remarks</span></span>

<span data-ttu-id="624e6-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="624e6-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="624e6-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="624e6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="624e6-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="624e6-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="624e6-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="624e6-123">Schema Name</span></span>  <br/> |<span data-ttu-id="624e6-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="624e6-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="624e6-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="624e6-125">Validation File</span></span>  <br/> |<span data-ttu-id="624e6-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="624e6-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="624e6-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="624e6-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="624e6-128">False</span><span class="sxs-lookup"><span data-stu-id="624e6-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="624e6-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="624e6-129">See also</span></span>



[<span data-ttu-id="624e6-130">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="624e6-130">MoveFolder operation</span></span>](movefolder-operation.md)

