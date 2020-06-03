---
title: RelativeFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54e3ba52-08a6-4d48-8a44-6fd5fdbffb25
description: L’élément RelativeFolderPath contient un tableau de dossiers qui indiquent le chemin d’accès au dossier relatif du chemin d’accès au dossier à créer.
ms.openlocfilehash: 8a0fc0020943afdbe6cd4c79d51d61337f8dd329
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457157"
---
# <a name="relativefolderpath"></a><span data-ttu-id="815ab-103">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="815ab-103">RelativeFolderPath</span></span>

<span data-ttu-id="815ab-104">L’élément **RelativeFolderPath** contient un tableau de dossiers qui indiquent le chemin d’accès au dossier relatif du chemin d’accès au dossier à créer.</span><span class="sxs-lookup"><span data-stu-id="815ab-104">The **RelativeFolderPath** element contains an array of folders that indicate the relative folder path of the folder path to be created.</span></span> 
  
```XML
<RelativeFolderPath>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</RelativeFolderPath>
```

 <span data-ttu-id="815ab-105">**NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="815ab-105">**NonEmptyArrayOfFoldersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="815ab-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="815ab-106">Attributes and elements</span></span>

<span data-ttu-id="815ab-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="815ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="815ab-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="815ab-108">Attributes</span></span>

<span data-ttu-id="815ab-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="815ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="815ab-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="815ab-110">Child elements</span></span>

<span data-ttu-id="815ab-111">[Folder (dossier](folder.md)  |  ) [CalendarFolder](calendarfolder.md)  |  [ContactsFolder](contactsfolder.md)  |  [SearchFolder](searchfolder.md)  |  [TasksFolder](tasksfolder.md)</span><span class="sxs-lookup"><span data-stu-id="815ab-111">[Folder](folder.md) | [CalendarFolder](calendarfolder.md) | [ContactsFolder](contactsfolder.md) | [SearchFolder](searchfolder.md) | [TasksFolder](tasksfolder.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="815ab-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="815ab-112">Parent elements</span></span>

[<span data-ttu-id="815ab-113">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="815ab-113">CreateFolderPath</span></span>](createfolderpath.md)
  
## <a name="remarks"></a><span data-ttu-id="815ab-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="815ab-114">Remarks</span></span>

<span data-ttu-id="815ab-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="815ab-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="815ab-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="815ab-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="815ab-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="815ab-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="815ab-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="815ab-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="815ab-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="815ab-119">Schema name</span></span>  <br/> |<span data-ttu-id="815ab-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="815ab-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="815ab-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="815ab-121">Validation file</span></span>  <br/> |<span data-ttu-id="815ab-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="815ab-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="815ab-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="815ab-123">Can be empty</span></span>  <br/> ||
   

