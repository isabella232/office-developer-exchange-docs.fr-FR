---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: L’élément AddBlankTargetToLinks indique que l’attribut cible des liens HTML sont définies pour ouvrir une nouvelle fenêtre.
ms.openlocfilehash: 8a47e44d89bcc84bc0e8b61d45f18ff3182f7870
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755158"
---
# <a name="addblanktargettolinks"></a><span data-ttu-id="bf4af-103">AddBlankTargetToLinks</span><span class="sxs-lookup"><span data-stu-id="bf4af-103">AddBlankTargetToLinks</span></span>

<span data-ttu-id="bf4af-104">L’élément **AddBlankTargetToLinks** indique que l’attribut cible des liens HTML sont définies pour ouvrir une nouvelle fenêtre.</span><span class="sxs-lookup"><span data-stu-id="bf4af-104">The **AddBlankTargetToLinks** element specifies that the target attribute in HTML links are set to open a new window.</span></span> 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

<span data-ttu-id="bf4af-105">**xs : Boolean**</span><span class="sxs-lookup"><span data-stu-id="bf4af-105">**xs:Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bf4af-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bf4af-106">Attributes and elements</span></span>

<span data-ttu-id="bf4af-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bf4af-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf4af-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bf4af-108">Attributes</span></span>

<span data-ttu-id="bf4af-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bf4af-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf4af-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bf4af-110">Child elements</span></span>

<span data-ttu-id="bf4af-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bf4af-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bf4af-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bf4af-112">Parent elements</span></span>

|<span data-ttu-id="bf4af-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bf4af-113">**Element**</span></span>|<span data-ttu-id="bf4af-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="bf4af-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf4af-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="bf4af-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="bf4af-116">Identifie les propriétés de l’élément et le contenu à inclure dans une **GetItem**, **FindItem**, **GetConversationItems** ou une réponse **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="bf4af-116">Identifies the item properties and content to include in a **GetItem**, **FindItem**, **GetConversationItems** or **SyncFolderItems** response.</span></span><br/><br/>  <span data-ttu-id="bf4af-117">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="bf4af-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bf4af-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bf4af-118">Text value</span></span>

<span data-ttu-id="bf4af-119">Une valeur de texte de **la valeur true** pour l’élément **AddBlankTargetToLinks** indique que tous les liens HTML seront définies pour ouvrir une nouvelle fenêtre.</span><span class="sxs-lookup"><span data-stu-id="bf4af-119">A text value of **true** for the **AddBlankTargetToLinks** element indicates that all HTML links will be set to open a new window.</span></span> <span data-ttu-id="bf4af-120">La valeur **false** indique que les liens HTML seront ouvre dans la fenêtre active.</span><span class="sxs-lookup"><span data-stu-id="bf4af-120">A value of **false** indicates that HTML links will open in the current window.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bf4af-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="bf4af-121">Remarks</span></span>

<span data-ttu-id="bf4af-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="bf4af-122">This element is optional.</span></span>
  
<span data-ttu-id="bf4af-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bf4af-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bf4af-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf4af-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf4af-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bf4af-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf4af-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bf4af-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf4af-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bf4af-127">Schema Name</span></span>  <br/> |<span data-ttu-id="bf4af-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="bf4af-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="bf4af-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="bf4af-129">Validation File</span></span>  <br/> |<span data-ttu-id="bf4af-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="bf4af-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf4af-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bf4af-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bf4af-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bf4af-132">See also</span></span>

- [<span data-ttu-id="bf4af-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bf4af-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

