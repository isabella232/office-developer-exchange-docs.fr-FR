---
title: ReadFlag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d91aa89-9f9f-4877-846d-aaf48bbeec7c
description: L’élément ReadFlag indique l’état de lecture pour définir des éléments dans un dossier.
ms.openlocfilehash: f3156a51fbdd3372dd28f2065499d26a50b3d497
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828954"
---
# <a name="readflag"></a><span data-ttu-id="875c9-103">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="875c9-103">ReadFlag</span></span>

<span data-ttu-id="875c9-104">L’élément **ReadFlag** indique l’état de lecture pour définir des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="875c9-104">The **ReadFlag** element indicates the read state to set on items in a folder.</span></span> 
  
```XML
<ReadFlag>true | false</ReadFlag>
```

 <span data-ttu-id="875c9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="875c9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="875c9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="875c9-106">Attributes and elements</span></span>

<span data-ttu-id="875c9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="875c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="875c9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="875c9-108">Attributes</span></span>

<span data-ttu-id="875c9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="875c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="875c9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="875c9-110">Child elements</span></span>

<span data-ttu-id="875c9-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="875c9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="875c9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="875c9-112">Parent elements</span></span>

[<span data-ttu-id="875c9-113">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="875c9-113">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
  
## <a name="text-value"></a><span data-ttu-id="875c9-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="875c9-114">Text value</span></span>

<span data-ttu-id="875c9-115">Une valeur de texte de **la valeur true** pour l’élément **ReadFlag** indique que les éléments dans le dossier seront marqués comme lu.</span><span class="sxs-lookup"><span data-stu-id="875c9-115">A text value of **true** for the **ReadFlag** element indicates that the items in the folder will be marked as read.</span></span> <span data-ttu-id="875c9-116">La valeur **false** indique que les éléments dans le dossier seront marqués comme non lus.</span><span class="sxs-lookup"><span data-stu-id="875c9-116">A value of **false** indicates that the items in the folder will be marked as unread.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="875c9-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="875c9-117">Remarks</span></span>

<span data-ttu-id="875c9-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="875c9-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="875c9-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="875c9-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="875c9-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="875c9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="875c9-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="875c9-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="875c9-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="875c9-122">Schema name</span></span>  <br/> |<span data-ttu-id="875c9-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="875c9-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="875c9-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="875c9-124">Validation file</span></span>  <br/> |<span data-ttu-id="875c9-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="875c9-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="875c9-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="875c9-126">Can be empty</span></span>  <br/> ||
   

