---
title: ReadFlag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d91aa89-9f9f-4877-846d-aaf48bbeec7c
description: L’élément ReadFlag indique l’état de lecture à définir sur les éléments d’un dossier.
ms.openlocfilehash: 1d3b9f3fe199ed2e63bdb632135120a5f89f4d1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529895"
---
# <a name="readflag"></a><span data-ttu-id="f002c-103">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="f002c-103">ReadFlag</span></span>

<span data-ttu-id="f002c-104">L’élément **ReadFlag** indique l’état de lecture à définir sur les éléments d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="f002c-104">The **ReadFlag** element indicates the read state to set on items in a folder.</span></span> 
  
```XML
<ReadFlag>true | false</ReadFlag>
```

 <span data-ttu-id="f002c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f002c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f002c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f002c-106">Attributes and elements</span></span>

<span data-ttu-id="f002c-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f002c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f002c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f002c-108">Attributes</span></span>

<span data-ttu-id="f002c-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f002c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f002c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f002c-110">Child elements</span></span>

<span data-ttu-id="f002c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f002c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f002c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f002c-112">Parent elements</span></span>

[<span data-ttu-id="f002c-113">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="f002c-113">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
  
## <a name="text-value"></a><span data-ttu-id="f002c-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f002c-114">Text value</span></span>

<span data-ttu-id="f002c-115">Une valeur de texte de **true** pour l’élément **ReadFlag** indique que les éléments dans le dossier seront marqués comme lus.</span><span class="sxs-lookup"><span data-stu-id="f002c-115">A text value of **true** for the **ReadFlag** element indicates that the items in the folder will be marked as read.</span></span> <span data-ttu-id="f002c-116">La valeur **false** indique que les éléments du dossier seront marqués comme non lus.</span><span class="sxs-lookup"><span data-stu-id="f002c-116">A value of **false** indicates that the items in the folder will be marked as unread.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f002c-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="f002c-117">Remarks</span></span>

<span data-ttu-id="f002c-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f002c-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f002c-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f002c-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f002c-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f002c-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f002c-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f002c-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f002c-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f002c-122">Schema name</span></span>  <br/> |<span data-ttu-id="f002c-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f002c-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f002c-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f002c-124">Validation file</span></span>  <br/> |<span data-ttu-id="f002c-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f002c-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f002c-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f002c-126">Can be empty</span></span>  <br/> ||
   

