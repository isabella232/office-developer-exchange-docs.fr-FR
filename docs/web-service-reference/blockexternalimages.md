---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: L’élément BlockExternalImages Spécifie si les images externes sont bloqués dans le corps de texte HTML.
ms.openlocfilehash: 41ab2ec7ec1c24ccbbef037ef1e27431c1fe6811
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755388"
---
# <a name="blockexternalimages"></a><span data-ttu-id="248d1-103">BlockExternalImages</span><span class="sxs-lookup"><span data-stu-id="248d1-103">BlockExternalImages</span></span>

<span data-ttu-id="248d1-104">L’élément **BlockExternalImages** Spécifie si les images externes sont bloqués dans le corps de texte HTML.</span><span class="sxs-lookup"><span data-stu-id="248d1-104">The **BlockExternalImages** element specifies whether external images are blocked in HTML text bodies.</span></span> 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 <span data-ttu-id="248d1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="248d1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="248d1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="248d1-106">Attributes and elements</span></span>

<span data-ttu-id="248d1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="248d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="248d1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="248d1-108">Attributes</span></span>

<span data-ttu-id="248d1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="248d1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="248d1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="248d1-110">Child elements</span></span>

<span data-ttu-id="248d1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="248d1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="248d1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="248d1-112">Parent elements</span></span>

|<span data-ttu-id="248d1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="248d1-113">**Element**</span></span>|<span data-ttu-id="248d1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="248d1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="248d1-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="248d1-115">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="248d1-116">Identifie les propriétés du dossier à inclure dans la réponse GetFolder, FindFolder ou SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="248d1-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span>  <br/> |
|[<span data-ttu-id="248d1-117">ItemShape</span><span class="sxs-lookup"><span data-stu-id="248d1-117">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="248d1-118">Identifie les propriétés de l’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="248d1-118">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="248d1-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="248d1-119">Text value</span></span>

<span data-ttu-id="248d1-120">Une valeur de texte de **la valeur true** pour l’élément **BlockExternalImages** indique que des images externes sont bloqués dans le corps HTML.</span><span class="sxs-lookup"><span data-stu-id="248d1-120">A text value of **true** for **BlockExternalImages** element indicates that external images are blocked in HTML bodies.</span></span> <span data-ttu-id="248d1-121">La valeur **false** indique que les images externes sont autorisées.</span><span class="sxs-lookup"><span data-stu-id="248d1-121">A value of **false** indicates that external images are allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="248d1-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="248d1-122">Remarks</span></span>

<span data-ttu-id="248d1-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="248d1-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="248d1-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="248d1-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="248d1-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="248d1-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="248d1-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="248d1-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="248d1-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="248d1-127">Schema Name</span></span>  <br/> |<span data-ttu-id="248d1-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="248d1-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="248d1-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="248d1-129">Validation File</span></span>  <br/> |<span data-ttu-id="248d1-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="248d1-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="248d1-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="248d1-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="248d1-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="248d1-132">See also</span></span>



- [<span data-ttu-id="248d1-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="248d1-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

