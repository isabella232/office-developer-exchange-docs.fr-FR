---
title: ArchiveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c2172e61-876a-4f76-bc9c-263c8be11429
description: L’élément ArchiveItem contient l’Id du dossier source et un tableau d’ID d’élément pour l’élément associé à archiver.
ms.openlocfilehash: 7f2d79f5a9e6798fafcf64e8b1bb680390800992
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755314"
---
# <a name="archiveitem"></a><span data-ttu-id="c75ef-103">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="c75ef-103">ArchiveItem</span></span>

<span data-ttu-id="c75ef-104">L’élément **ArchiveItem** contient l’Id du dossier source et un tableau d’ID d’élément pour l’élément associé à archiver.</span><span class="sxs-lookup"><span data-stu-id="c75ef-104">The **ArchiveItem** element contains the source folder Id and an array of item Ids for the associated archive item.</span></span> 
  
```XML
<ArchiveItem>
   <ArchiveSourceFolderId/>
   <ItemIds/>
</ArchiveItem>
```

 <span data-ttu-id="c75ef-105">**ArchiveItemType**</span><span class="sxs-lookup"><span data-stu-id="c75ef-105">**ArchiveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c75ef-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c75ef-106">Attributes and elements</span></span>

<span data-ttu-id="c75ef-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c75ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c75ef-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c75ef-108">Attributes</span></span>

<span data-ttu-id="c75ef-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c75ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c75ef-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c75ef-110">Child elements</span></span>

<span data-ttu-id="c75ef-111">[ArchiveSourceFolderId](archivesourcefolderid.md) | [ItemId](itemids.md)</span><span class="sxs-lookup"><span data-stu-id="c75ef-111">[ArchiveSourceFolderId](archivesourcefolderid.md) | [ItemIds](itemids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c75ef-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c75ef-112">Parent elements</span></span>

<span data-ttu-id="c75ef-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c75ef-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c75ef-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="c75ef-114">Remarks</span></span>

<span data-ttu-id="c75ef-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c75ef-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c75ef-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75ef-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c75ef-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c75ef-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c75ef-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c75ef-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c75ef-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c75ef-119">Schema name</span></span>  <br/> |<span data-ttu-id="c75ef-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c75ef-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c75ef-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c75ef-121">Validation file</span></span>  <br/> |<span data-ttu-id="c75ef-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c75ef-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c75ef-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c75ef-123">Can be empty</span></span>  <br/> |<span data-ttu-id="c75ef-124">false</span><span class="sxs-lookup"><span data-stu-id="c75ef-124">false</span></span>  <br/> |
   

