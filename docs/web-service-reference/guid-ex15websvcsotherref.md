---
title: Guid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 49dcf69f-bf8d-4be6-a24c-03bbd13f4fe5
description: L’élément Guid Spécifie l’identificateur global unique de la boîte aux lettres.
ms.openlocfilehash: 35307a706523fc5c2916767c7508dec07deb8d09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827799"
---
# <a name="guid"></a><span data-ttu-id="28105-103">Guid</span><span class="sxs-lookup"><span data-stu-id="28105-103">Guid</span></span>

<span data-ttu-id="28105-104">L’élément **Guid** Spécifie l’identificateur global unique de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="28105-104">The **Guid** element specifies the globally unique identifier of the mailbox.</span></span> 
  
```XML
<Guid></Guid>
```

 <span data-ttu-id="28105-105">**GuidType**</span><span class="sxs-lookup"><span data-stu-id="28105-105">**GuidType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28105-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="28105-106">Attributes and elements</span></span>

<span data-ttu-id="28105-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="28105-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28105-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="28105-108">Attributes</span></span>

<span data-ttu-id="28105-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28105-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28105-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="28105-110">Child elements</span></span>

<span data-ttu-id="28105-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28105-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="28105-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="28105-112">Parent elements</span></span>

|<span data-ttu-id="28105-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28105-113">**Element**</span></span>|<span data-ttu-id="28105-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="28105-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28105-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="28105-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="28105-116">Spécifie une boîte aux lettres renvoyé à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="28105-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="28105-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="28105-117">Text value</span></span>

<span data-ttu-id="28105-118">La valeur de texte de l’élément **Guid** est une valeur GUID qui identifie de manière unique une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="28105-118">The text value of the **Guid** element is a GUID value that uniquely identifies a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="28105-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="28105-119">Remarks</span></span>

<span data-ttu-id="28105-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="28105-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="28105-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="28105-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28105-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="28105-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28105-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="28105-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="28105-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="28105-124">Schema Name</span></span>  <br/> |<span data-ttu-id="28105-125">Schéma type</span><span class="sxs-lookup"><span data-stu-id="28105-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="28105-126">Validation File</span><span class="sxs-lookup"><span data-stu-id="28105-126">Validation File</span></span>  <br/> |<span data-ttu-id="28105-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="28105-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="28105-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="28105-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="28105-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="28105-129">See also</span></span>



- [<span data-ttu-id="28105-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="28105-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

