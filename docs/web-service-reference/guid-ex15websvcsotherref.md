---
title: Guid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 49dcf69f-bf8d-4be6-a24c-03bbd13f4fe5
description: L’élément GUID spécifie l’identificateur global unique de la boîte aux lettres.
ms.openlocfilehash: 4db66b5ae2c67f64f75c69a3d77cfa2b587775be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530774"
---
# <a name="guid"></a><span data-ttu-id="c2280-103">Guid</span><span class="sxs-lookup"><span data-stu-id="c2280-103">Guid</span></span>

<span data-ttu-id="c2280-104">L’élément **GUID** spécifie l’identificateur global unique de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c2280-104">The **Guid** element specifies the globally unique identifier of the mailbox.</span></span> 
  
```XML
<Guid></Guid>
```

 <span data-ttu-id="c2280-105">**GuidType**</span><span class="sxs-lookup"><span data-stu-id="c2280-105">**GuidType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2280-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c2280-106">Attributes and elements</span></span>

<span data-ttu-id="c2280-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c2280-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2280-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c2280-108">Attributes</span></span>

<span data-ttu-id="c2280-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c2280-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2280-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c2280-110">Child elements</span></span>

<span data-ttu-id="c2280-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c2280-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c2280-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c2280-112">Parent elements</span></span>

|<span data-ttu-id="c2280-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c2280-113">**Element**</span></span>|<span data-ttu-id="c2280-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="c2280-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2280-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="c2280-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="c2280-116">Spécifie une boîte aux lettres renvoyée à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="c2280-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2280-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="c2280-117">Text value</span></span>

<span data-ttu-id="c2280-118">La valeur de texte de l’élément **GUID** est une valeur GUID qui identifie de manière unique une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c2280-118">The text value of the **Guid** element is a GUID value that uniquely identifies a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c2280-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="c2280-119">Remarks</span></span>

<span data-ttu-id="c2280-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c2280-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c2280-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2280-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2280-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c2280-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2280-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c2280-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c2280-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c2280-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c2280-125">Schéma type</span><span class="sxs-lookup"><span data-stu-id="c2280-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="c2280-126">Validation File</span><span class="sxs-lookup"><span data-stu-id="c2280-126">Validation File</span></span>  <br/> |<span data-ttu-id="c2280-127">types. xsd</span><span class="sxs-lookup"><span data-stu-id="c2280-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c2280-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c2280-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c2280-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c2280-129">See also</span></span>



- [<span data-ttu-id="c2280-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c2280-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

