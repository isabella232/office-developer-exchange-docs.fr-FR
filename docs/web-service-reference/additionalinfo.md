---
title: AdditionalInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 50bebbab-2fef-4a27-a5a9-32d7200820b6
description: L’élément AdditionalInfo spécifie des informations supplémentaires sur l’état de la suspension d’une boîte aux lettres.
ms.openlocfilehash: 1911ff3ac0baf7a8854c0609e08959a54cc27b6d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455820"
---
# <a name="additionalinfo"></a><span data-ttu-id="7fe08-103">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="7fe08-103">AdditionalInfo</span></span>

<span data-ttu-id="7fe08-104">L’élément **AdditionalInfo** spécifie des informations supplémentaires sur l’état de la suspension d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7fe08-104">The **AdditionalInfo** element specifies additional information about the hold status of a mailbox.</span></span> 
  
```XML
<AdditionalInfo></AdditionalInfo>
```

 <span data-ttu-id="7fe08-105">**XS : String**</span><span class="sxs-lookup"><span data-stu-id="7fe08-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7fe08-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7fe08-106">Attributes and elements</span></span>

<span data-ttu-id="7fe08-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7fe08-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7fe08-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7fe08-108">Attributes</span></span>

<span data-ttu-id="7fe08-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7fe08-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7fe08-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7fe08-110">Child elements</span></span>

<span data-ttu-id="7fe08-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7fe08-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7fe08-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7fe08-112">Parent elements</span></span>

|<span data-ttu-id="7fe08-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7fe08-113">**Element**</span></span>|<span data-ttu-id="7fe08-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7fe08-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7fe08-115">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="7fe08-115">MailboxHoldStatus</span></span>](mailboxholdstatus.md) <br/> |<span data-ttu-id="7fe08-116">Spécifie l’état de conservation de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7fe08-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="7fe08-117">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="7fe08-117">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md) <br/> |<span data-ttu-id="7fe08-118">Spécifie le détail d’un élément qui ne peut pas être indexé.</span><span class="sxs-lookup"><span data-stu-id="7fe08-118">Specifies detail for an item that cannot be indexed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7fe08-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="7fe08-119">Text value</span></span>

<span data-ttu-id="7fe08-120">La valeur de texte de l’élément AdditionalInfo est des informations supplémentaires sur l’état de la suspension d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7fe08-120">The text value of the AdditionalInfo element is additional information about the hold status of a mailbox.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7fe08-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="7fe08-121">Remarks</span></span>

<span data-ttu-id="7fe08-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7fe08-122">This element is optional.</span></span>
  
<span data-ttu-id="7fe08-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7fe08-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7fe08-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7fe08-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7fe08-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7fe08-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7fe08-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7fe08-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7fe08-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7fe08-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7fe08-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="7fe08-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="7fe08-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="7fe08-129">Validation File</span></span>  <br/> |<span data-ttu-id="7fe08-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="7fe08-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7fe08-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7fe08-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7fe08-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7fe08-132">See also</span></span>

- [<span data-ttu-id="7fe08-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7fe08-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

