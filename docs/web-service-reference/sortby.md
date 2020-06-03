---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: L’élément SortBy contient une propriété Item utilisée pour trier le résultat de la recherche.
ms.openlocfilehash: cf2b1e633bc66e526028078833afade363e4c5e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468396"
---
# <a name="sortby"></a><span data-ttu-id="74792-103">SortBy</span><span class="sxs-lookup"><span data-stu-id="74792-103">SortBy</span></span>

<span data-ttu-id="74792-104">L’élément **SortBy** contient une propriété Item utilisée pour trier le résultat de la recherche.</span><span class="sxs-lookup"><span data-stu-id="74792-104">The **SortBy** element contains an item property used for sorting the search result.</span></span> 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 <span data-ttu-id="74792-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="74792-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74792-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="74792-106">Attributes and elements</span></span>

<span data-ttu-id="74792-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="74792-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74792-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="74792-108">Attributes</span></span>

|<span data-ttu-id="74792-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="74792-109">**Attribute**</span></span>|<span data-ttu-id="74792-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="74792-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="74792-111">Commande</span><span class="sxs-lookup"><span data-stu-id="74792-111">Order</span></span>  <br/> |<span data-ttu-id="74792-112">La valeur de texte de l’attribut **Order** est l’ordre de tri.</span><span class="sxs-lookup"><span data-stu-id="74792-112">The text value of the **Order** attribute is the sort order.</span></span> <span data-ttu-id="74792-113">Une valeur de texte **croissant** indique que les résultats sont triés par ordre croissant.</span><span class="sxs-lookup"><span data-stu-id="74792-113">A text value of **Ascending** indicates that the results are in ascending order.</span></span> <span data-ttu-id="74792-114">Une valeur de texte **décroissant** indique que les résultats sont triés par ordre décroissant.</span><span class="sxs-lookup"><span data-stu-id="74792-114">A text value of **Descending** indicates that the results are in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="74792-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="74792-115">Child elements</span></span>

<span data-ttu-id="74792-116">[FieldURI](fielduri.md)  |  [IndexedFieldURI](indexedfielduri.md)</span><span class="sxs-lookup"><span data-stu-id="74792-116">[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="74792-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="74792-117">Parent elements</span></span>

[<span data-ttu-id="74792-118">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="74792-118">SearchMailboxes</span></span>](searchmailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="74792-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="74792-119">Remarks</span></span>

<span data-ttu-id="74792-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="74792-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="74792-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="74792-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74792-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="74792-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74792-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="74792-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74792-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="74792-124">Schema name</span></span>  <br/> |<span data-ttu-id="74792-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="74792-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74792-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="74792-126">Validation file</span></span>  <br/> |<span data-ttu-id="74792-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="74792-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74792-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="74792-128">Can be empty</span></span>  <br/> ||
   

