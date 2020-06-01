---
title: CreateFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 282576cb-a921-49f7-8748-64158fd50c41
description: L’élément CreateFolderPath est utilisé pour créer un chemin d’accès de dossier et inclut un ID de dossier parent et un chemin d’accès de dossier relatif.
ms.openlocfilehash: e6ce6c9b6e12a6a0fb6792b63368a79c87d06f07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457535"
---
# <a name="createfolderpath"></a><span data-ttu-id="03d82-103">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="03d82-103">CreateFolderPath</span></span>

<span data-ttu-id="03d82-104">L’élément **CreateFolderPath** est utilisé pour créer un chemin d’accès de dossier et inclut un ID de dossier parent et un chemin d’accès de dossier relatif.</span><span class="sxs-lookup"><span data-stu-id="03d82-104">The **CreateFolderPath** element is used to create a folder path and includes a parent folder Id and a relative folder path.</span></span> 
  
```XML
<CreateFolderPath>
   <ParentFolderId/>
   <RelativeFolderPath/>
</CreateFolderPath>
```

 <span data-ttu-id="03d82-105">**CreateFolderPathType**</span><span class="sxs-lookup"><span data-stu-id="03d82-105">**CreateFolderPathType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03d82-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="03d82-106">Attributes and elements</span></span>

<span data-ttu-id="03d82-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="03d82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03d82-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="03d82-108">Attributes</span></span>

<span data-ttu-id="03d82-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="03d82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03d82-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="03d82-110">Child elements</span></span>

<span data-ttu-id="03d82-111">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  |  [RelativeFolderPath](relativefolderpath.md)</span><span class="sxs-lookup"><span data-stu-id="03d82-111">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [RelativeFolderPath](relativefolderpath.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03d82-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="03d82-112">Parent elements</span></span>

<span data-ttu-id="03d82-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="03d82-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="03d82-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="03d82-114">Remarks</span></span>

<span data-ttu-id="03d82-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="03d82-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="03d82-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="03d82-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03d82-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="03d82-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03d82-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="03d82-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="03d82-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="03d82-119">Schema name</span></span>  <br/> |<span data-ttu-id="03d82-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="03d82-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="03d82-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="03d82-121">Validation file</span></span>  <br/> |<span data-ttu-id="03d82-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="03d82-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="03d82-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="03d82-123">Can be empty</span></span>  <br/> |<span data-ttu-id="03d82-124">false</span><span class="sxs-lookup"><span data-stu-id="03d82-124">false</span></span>  <br/> |
   

