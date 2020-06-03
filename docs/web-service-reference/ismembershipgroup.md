---
title: IsMembershipGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: L’élément IsMembershipGroup spécifie une valeur booléenne qui indique si l’entité est un groupe de distribution ou une boîte aux lettres.
ms.openlocfilehash: ed79961c6d13ab226c0b489103ef3d2c4a08668d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459285"
---
# <a name="ismembershipgroup"></a><span data-ttu-id="1f571-103">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="1f571-103">IsMembershipGroup</span></span>

<span data-ttu-id="1f571-104">L’élément **IsMembershipGroup** spécifie une valeur booléenne qui indique si l’entité est un groupe de distribution ou une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1f571-104">The **IsMembershipGroup** element specifies a Boolean value that indicates whether the entity is a distribution group or a mailbox.</span></span> 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
```

 <span data-ttu-id="1f571-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1f571-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f571-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1f571-106">Attributes and elements</span></span>

<span data-ttu-id="1f571-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1f571-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f571-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1f571-108">Attributes</span></span>

<span data-ttu-id="1f571-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1f571-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f571-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1f571-110">Child elements</span></span>

<span data-ttu-id="1f571-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1f571-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1f571-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1f571-112">Parent elements</span></span>

|<span data-ttu-id="1f571-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1f571-113">**Element**</span></span>|<span data-ttu-id="1f571-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f571-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f571-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="1f571-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="1f571-116">Spécifie une boîte aux lettres renvoyée à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="1f571-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1f571-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="1f571-117">Text value</span></span>

<span data-ttu-id="1f571-118">Une valeur de texte de **true** pour l’élément **IsMembershipGroup** indique que l’entité est un groupe de distribution ou une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1f571-118">A text value of **true** for the **IsMembershipGroup** element indicates that the entity is a distribution group or a mailbox.</span></span> <span data-ttu-id="1f571-119">La valeur false indique que l’entité n’est pas un groupe de distribution ou une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1f571-119">A value of false indicates that the entity is not a distribution group or a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1f571-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="1f571-120">Remarks</span></span>

<span data-ttu-id="1f571-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1f571-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1f571-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f571-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f571-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1f571-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f571-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1f571-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f571-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1f571-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1f571-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="1f571-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="1f571-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="1f571-127">Validation File</span></span>  <br/> |<span data-ttu-id="1f571-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="1f571-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f571-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1f571-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1f571-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1f571-130">See also</span></span>



- [<span data-ttu-id="1f571-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1f571-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

