---
title: RelativeFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54e3ba52-08a6-4d48-8a44-6fd5fdbffb25
description: L’élément RelativeFolderPath contient un tableau des dossiers qui indiquent le chemin d’accès de dossier relatif du chemin du dossier à créer.
ms.openlocfilehash: f568d282e47a41c0aaf6d70ef383e5ef3e2b54bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829051"
---
# <a name="relativefolderpath"></a><span data-ttu-id="a8dc9-103">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="a8dc9-103">RelativeFolderPath</span></span>

<span data-ttu-id="a8dc9-104">L’élément **RelativeFolderPath** contient un tableau des dossiers qui indiquent le chemin d’accès de dossier relatif du chemin du dossier à créer.</span><span class="sxs-lookup"><span data-stu-id="a8dc9-104">The **RelativeFolderPath** element contains an array of folders that indicate the relative folder path of the folder path to be created.</span></span> 
  
```XML
<RelativeFolderPath>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</RelativeFolderPath>
```

 <span data-ttu-id="a8dc9-105">**NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="a8dc9-105">**NonEmptyArrayOfFoldersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8dc9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a8dc9-106">Attributes and elements</span></span>

<span data-ttu-id="a8dc9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a8dc9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8dc9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a8dc9-108">Attributes</span></span>

<span data-ttu-id="a8dc9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a8dc9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8dc9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a8dc9-110">Child elements</span></span>

<span data-ttu-id="a8dc9-111">[Dossier](folder.md) | [CalendarFolder](calendarfolder.md) | [ContactsFolder](contactsfolder.md) | [SearchFolder](searchfolder.md) | [dossier tâches](tasksfolder.md)</span><span class="sxs-lookup"><span data-stu-id="a8dc9-111">[Folder](folder.md) | [CalendarFolder](calendarfolder.md) | [ContactsFolder](contactsfolder.md) | [SearchFolder](searchfolder.md) | [TasksFolder](tasksfolder.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8dc9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a8dc9-112">Parent elements</span></span>

[<span data-ttu-id="a8dc9-113">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="a8dc9-113">CreateFolderPath</span></span>](createfolderpath.md)
  
## <a name="remarks"></a><span data-ttu-id="a8dc9-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="a8dc9-114">Remarks</span></span>

<span data-ttu-id="a8dc9-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a8dc9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a8dc9-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8dc9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8dc9-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a8dc9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8dc9-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a8dc9-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a8dc9-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a8dc9-119">Schema name</span></span>  <br/> |<span data-ttu-id="a8dc9-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a8dc9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a8dc9-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a8dc9-121">Validation file</span></span>  <br/> |<span data-ttu-id="a8dc9-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a8dc9-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a8dc9-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a8dc9-123">Can be empty</span></span>  <br/> ||
   

