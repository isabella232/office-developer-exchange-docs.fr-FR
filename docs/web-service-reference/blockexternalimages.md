---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: L’élément BlockExternalImages spécifie si les images externes sont bloquées dans les corps de texte HTML.
ms.openlocfilehash: 73342316024ebe476a0e35f14157befc80edcf83
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527403"
---
# <a name="blockexternalimages"></a><span data-ttu-id="3c5a3-103">BlockExternalImages</span><span class="sxs-lookup"><span data-stu-id="3c5a3-103">BlockExternalImages</span></span>

<span data-ttu-id="3c5a3-104">L’élément **BlockExternalImages** spécifie si les images externes sont bloquées dans les corps de texte html.</span><span class="sxs-lookup"><span data-stu-id="3c5a3-104">The **BlockExternalImages** element specifies whether external images are blocked in HTML text bodies.</span></span> 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 <span data-ttu-id="3c5a3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3c5a3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c5a3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3c5a3-106">Attributes and elements</span></span>

<span data-ttu-id="3c5a3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3c5a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c5a3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3c5a3-108">Attributes</span></span>

<span data-ttu-id="3c5a3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3c5a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c5a3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3c5a3-110">Child elements</span></span>

<span data-ttu-id="3c5a3-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3c5a3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3c5a3-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3c5a3-112">Parent elements</span></span>

|<span data-ttu-id="3c5a3-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3c5a3-113">**Element**</span></span>|<span data-ttu-id="3c5a3-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3c5a3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c5a3-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="3c5a3-115">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="3c5a3-116">Identifie les propriétés de dossier à inclure dans la réponse GetFolder, FindFolder ou Opérationsyncfolderhierarchy.</span><span class="sxs-lookup"><span data-stu-id="3c5a3-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span>  <br/> |
|[<span data-ttu-id="3c5a3-117">ItemShape</span><span class="sxs-lookup"><span data-stu-id="3c5a3-117">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="3c5a3-118">Identifie les propriétés d’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="3c5a3-118">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3c5a3-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="3c5a3-119">Text value</span></span>

<span data-ttu-id="3c5a3-120">Une valeur de texte de **true** pour l’élément **BlockExternalImages** indique que les images externes sont bloquées dans les corps HTML.</span><span class="sxs-lookup"><span data-stu-id="3c5a3-120">A text value of **true** for **BlockExternalImages** element indicates that external images are blocked in HTML bodies.</span></span> <span data-ttu-id="3c5a3-121">La valeur **false** indique que les images externes sont autorisées.</span><span class="sxs-lookup"><span data-stu-id="3c5a3-121">A value of **false** indicates that external images are allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3c5a3-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="3c5a3-122">Remarks</span></span>

<span data-ttu-id="3c5a3-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3c5a3-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3c5a3-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c5a3-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c5a3-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3c5a3-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c5a3-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3c5a3-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c5a3-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3c5a3-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3c5a3-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="3c5a3-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="3c5a3-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="3c5a3-129">Validation File</span></span>  <br/> |<span data-ttu-id="3c5a3-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="3c5a3-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c5a3-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3c5a3-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3c5a3-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3c5a3-132">See also</span></span>



- [<span data-ttu-id="3c5a3-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3c5a3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

