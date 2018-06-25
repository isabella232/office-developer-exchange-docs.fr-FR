---
title: IsArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b89d8a78-5c18-4547-aaf4-4b16a93190a7
description: L’élément IsArchive indique une valeur de type Boolean qui indique si la boîte aux lettres est une boîte aux lettres d’archive.
ms.openlocfilehash: 417afd1afc25e5872d1f511feff34494fe6b7b62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827990"
---
# <a name="isarchive"></a><span data-ttu-id="96089-103">IsArchive</span><span class="sxs-lookup"><span data-stu-id="96089-103">IsArchive</span></span>

<span data-ttu-id="96089-104">L’élément **IsArchive** indique une valeur de type Boolean qui indique si la boîte aux lettres est une boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="96089-104">The **IsArchive** element specifies a Boolean value that indicates whether the mailbox is an archive mailbox.</span></span> 
  
```XML
<IsArchive>true | false</IsArchive>
```

 <span data-ttu-id="96089-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="96089-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96089-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="96089-106">Attributes and elements</span></span>

<span data-ttu-id="96089-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="96089-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96089-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="96089-108">Attributes</span></span>

<span data-ttu-id="96089-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="96089-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96089-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="96089-110">Child elements</span></span>

<span data-ttu-id="96089-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="96089-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96089-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="96089-112">Parent elements</span></span>

<span data-ttu-id="96089-113">[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)</span><span class="sxs-lookup"><span data-stu-id="96089-113">[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="96089-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="96089-114">Text value</span></span>

<span data-ttu-id="96089-115">Une valeur de texte de **la valeur true** pour l’élément **IsArchive** indique que la boîte aux lettres cible est une boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="96089-115">A text value of **true** for the **IsArchive** element indicates that the target mailbox is an archive mailbox.</span></span> <span data-ttu-id="96089-116">La valeur **false** indique que la boîte aux lettres cible n’est pas une boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="96089-116">A value of **false** indicates that the target mailbox is not an archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="96089-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="96089-117">Remarks</span></span>

<span data-ttu-id="96089-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="96089-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="96089-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="96089-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96089-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="96089-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96089-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="96089-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="96089-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="96089-122">Schema Name</span></span>  <br/> |<span data-ttu-id="96089-123">Schéma type</span><span class="sxs-lookup"><span data-stu-id="96089-123">Type schema</span></span>  <br/> |
|<span data-ttu-id="96089-124">Validation File</span><span class="sxs-lookup"><span data-stu-id="96089-124">Validation File</span></span>  <br/> |<span data-ttu-id="96089-125">types.xsd</span><span class="sxs-lookup"><span data-stu-id="96089-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="96089-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="96089-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="96089-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="96089-127">See also</span></span>



- [<span data-ttu-id="96089-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="96089-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

