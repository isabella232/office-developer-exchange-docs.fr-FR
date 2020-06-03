---
title: MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22244afb-99ec-41b4-8f73-3fbccd56d1ab
description: L’élément MarkAllItemsAsRead contient la demande pour marquer tous les éléments d’un dossier comme étant lus.
ms.openlocfilehash: 0338b2a1eed503b7e8fb0ec8b4a8ebcf12b6dbd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530887"
---
# <a name="markallitemsasread"></a><span data-ttu-id="772df-103">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="772df-103">MarkAllItemsAsRead</span></span>

<span data-ttu-id="772df-104">L’élément **MarkAllItemsAsRead** contient la demande pour marquer tous les éléments d’un dossier comme étant lus.</span><span class="sxs-lookup"><span data-stu-id="772df-104">The **MarkAllItemsAsRead** element contains the request to mark all the items in a folder as read.</span></span> 
  
```XML
<MarkAllItemsAsRead>
   <ReadFlag/>
   <SuppressReadReceipts/>
   <FolderIds/>
</MarkAllItemsAsRead>
```

 <span data-ttu-id="772df-105">**MarkAllItemsAsReadType**</span><span class="sxs-lookup"><span data-stu-id="772df-105">**MarkAllItemsAsReadType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="772df-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="772df-106">Attributes and elements</span></span>

<span data-ttu-id="772df-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="772df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="772df-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="772df-108">Attributes</span></span>

<span data-ttu-id="772df-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="772df-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="772df-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="772df-110">Child elements</span></span>

<span data-ttu-id="772df-111">[ReadFlag](readflag.md)  |  [SuppressReadReceipts](suppressreadreceipts.md)  |  [FolderIds](folderids.md)</span><span class="sxs-lookup"><span data-stu-id="772df-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="772df-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="772df-112">Parent elements</span></span>

<span data-ttu-id="772df-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="772df-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="772df-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="772df-114">Remarks</span></span>

<span data-ttu-id="772df-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="772df-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="772df-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="772df-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="772df-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="772df-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="772df-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="772df-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="772df-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="772df-119">Schema name</span></span>  <br/> |<span data-ttu-id="772df-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="772df-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="772df-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="772df-121">Validation file</span></span>  <br/> |<span data-ttu-id="772df-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="772df-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="772df-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="772df-123">Can be empty</span></span>  <br/> ||
   

