---
title: CreateFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 282576cb-a921-49f7-8748-64158fd50c41
description: L’élément CreateFolderPath est utilisé pour créer un chemin d’accès du dossier et inclut un Id du dossier parent et un chemin d’accès relatif.
ms.openlocfilehash: bfe31d894cfaa0f36da2d1d0045f723e0d261759
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755701"
---
# <a name="createfolderpath"></a><span data-ttu-id="81bfd-103">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="81bfd-103">CreateFolderPath</span></span>

<span data-ttu-id="81bfd-104">L’élément **CreateFolderPath** est utilisé pour créer un chemin d’accès du dossier et inclut un Id du dossier parent et un chemin d’accès relatif.</span><span class="sxs-lookup"><span data-stu-id="81bfd-104">The **CreateFolderPath** element is used to create a folder path and includes a parent folder Id and a relative folder path.</span></span> 
  
```XML
<CreateFolderPath>
   <ParentFolderId/>
   <RelativeFolderPath/>
</CreateFolderPath>
```

 <span data-ttu-id="81bfd-105">**CreateFolderPathType**</span><span class="sxs-lookup"><span data-stu-id="81bfd-105">**CreateFolderPathType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81bfd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="81bfd-106">Attributes and elements</span></span>

<span data-ttu-id="81bfd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="81bfd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81bfd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="81bfd-108">Attributes</span></span>

<span data-ttu-id="81bfd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="81bfd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81bfd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="81bfd-110">Child elements</span></span>

<span data-ttu-id="81bfd-111">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [RelativeFolderPath](relativefolderpath.md)</span><span class="sxs-lookup"><span data-stu-id="81bfd-111">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [RelativeFolderPath](relativefolderpath.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="81bfd-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="81bfd-112">Parent elements</span></span>

<span data-ttu-id="81bfd-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="81bfd-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="81bfd-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="81bfd-114">Remarks</span></span>

<span data-ttu-id="81bfd-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="81bfd-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="81bfd-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="81bfd-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81bfd-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="81bfd-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81bfd-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="81bfd-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="81bfd-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="81bfd-119">Schema name</span></span>  <br/> |<span data-ttu-id="81bfd-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="81bfd-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="81bfd-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="81bfd-121">Validation file</span></span>  <br/> |<span data-ttu-id="81bfd-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="81bfd-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="81bfd-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="81bfd-123">Can be empty</span></span>  <br/> |<span data-ttu-id="81bfd-124">false</span><span class="sxs-lookup"><span data-stu-id="81bfd-124">false</span></span>  <br/> |
   

