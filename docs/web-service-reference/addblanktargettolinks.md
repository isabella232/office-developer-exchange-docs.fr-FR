---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: L’élément AddBlankTargetToLinks spécifie que l’attribut cible des liens HTML est configuré pour ouvrir une nouvelle fenêtre.
ms.openlocfilehash: 1d4d36c1f4b98ebee96baea683c40527d2a9ec27
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465042"
---
# <a name="addblanktargettolinks"></a><span data-ttu-id="0de07-103">AddBlankTargetToLinks</span><span class="sxs-lookup"><span data-stu-id="0de07-103">AddBlankTargetToLinks</span></span>

<span data-ttu-id="0de07-104">L’élément **AddBlankTargetToLinks** spécifie que l’attribut cible des liens HTML est configuré pour ouvrir une nouvelle fenêtre.</span><span class="sxs-lookup"><span data-stu-id="0de07-104">The **AddBlankTargetToLinks** element specifies that the target attribute in HTML links are set to open a new window.</span></span> 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

<span data-ttu-id="0de07-105">**XS : Boolean**</span><span class="sxs-lookup"><span data-stu-id="0de07-105">**xs:Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0de07-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0de07-106">Attributes and elements</span></span>

<span data-ttu-id="0de07-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0de07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0de07-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0de07-108">Attributes</span></span>

<span data-ttu-id="0de07-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0de07-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0de07-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0de07-110">Child elements</span></span>

<span data-ttu-id="0de07-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0de07-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0de07-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0de07-112">Parent elements</span></span>

|<span data-ttu-id="0de07-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0de07-113">**Element**</span></span>|<span data-ttu-id="0de07-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0de07-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0de07-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="0de07-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="0de07-116">Identifie les propriétés d’élément et le contenu à inclure dans une réponse **GetItem**, **FindItem**, **GetConversationItems** ou **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="0de07-116">Identifies the item properties and content to include in a **GetItem**, **FindItem**, **GetConversationItems** or **SyncFolderItems** response.</span></span><br/><br/>  <span data-ttu-id="0de07-117">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="0de07-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0de07-118">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0de07-118">Text value</span></span>

<span data-ttu-id="0de07-119">Une valeur de texte de **true** pour l’élément **AddBlankTargetToLinks** indique que tous les liens html seront définis pour ouvrir une nouvelle fenêtre.</span><span class="sxs-lookup"><span data-stu-id="0de07-119">A text value of **true** for the **AddBlankTargetToLinks** element indicates that all HTML links will be set to open a new window.</span></span> <span data-ttu-id="0de07-120">La valeur **false** indique que les liens html s’ouvrent dans la fenêtre active.</span><span class="sxs-lookup"><span data-stu-id="0de07-120">A value of **false** indicates that HTML links will open in the current window.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0de07-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="0de07-121">Remarks</span></span>

<span data-ttu-id="0de07-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="0de07-122">This element is optional.</span></span>
  
<span data-ttu-id="0de07-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0de07-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0de07-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0de07-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0de07-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0de07-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0de07-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0de07-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0de07-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0de07-127">Schema Name</span></span>  <br/> |<span data-ttu-id="0de07-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="0de07-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="0de07-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="0de07-129">Validation File</span></span>  <br/> |<span data-ttu-id="0de07-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="0de07-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0de07-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0de07-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0de07-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0de07-132">See also</span></span>

- [<span data-ttu-id="0de07-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0de07-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

