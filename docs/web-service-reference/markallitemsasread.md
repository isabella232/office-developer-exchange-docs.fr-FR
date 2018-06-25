---
title: MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22244afb-99ec-41b4-8f73-3fbccd56d1ab
description: L’élément MarkAllItemsAsRead contient la demande pour marquer tous les éléments dans un dossier comme lus.
ms.openlocfilehash: 9d7eb8eb7194cb5d77e909dc08abfb70e2385d56
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828346"
---
# <a name="markallitemsasread"></a><span data-ttu-id="b22bf-103">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="b22bf-103">MarkAllItemsAsRead</span></span>

<span data-ttu-id="b22bf-104">L’élément **MarkAllItemsAsRead** contient la demande pour marquer tous les éléments dans un dossier comme lus.</span><span class="sxs-lookup"><span data-stu-id="b22bf-104">The **MarkAllItemsAsRead** element contains the request to mark all the items in a folder as read.</span></span> 
  
```XML
<MarkAllItemsAsRead>
   <ReadFlag/>
   <SuppressReadReceipts/>
   <FolderIds/>
</MarkAllItemsAsRead>
```

 <span data-ttu-id="b22bf-105">**MarkAllItemsAsReadType**</span><span class="sxs-lookup"><span data-stu-id="b22bf-105">**MarkAllItemsAsReadType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b22bf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b22bf-106">Attributes and elements</span></span>

<span data-ttu-id="b22bf-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b22bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b22bf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b22bf-108">Attributes</span></span>

<span data-ttu-id="b22bf-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b22bf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b22bf-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b22bf-110">Child elements</span></span>

<span data-ttu-id="b22bf-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span><span class="sxs-lookup"><span data-stu-id="b22bf-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b22bf-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b22bf-112">Parent elements</span></span>

<span data-ttu-id="b22bf-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b22bf-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b22bf-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="b22bf-114">Remarks</span></span>

<span data-ttu-id="b22bf-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b22bf-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b22bf-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b22bf-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b22bf-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b22bf-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b22bf-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b22bf-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b22bf-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b22bf-119">Schema name</span></span>  <br/> |<span data-ttu-id="b22bf-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b22bf-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b22bf-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b22bf-121">Validation file</span></span>  <br/> |<span data-ttu-id="b22bf-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b22bf-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b22bf-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b22bf-123">Can be empty</span></span>  <br/> ||
   

