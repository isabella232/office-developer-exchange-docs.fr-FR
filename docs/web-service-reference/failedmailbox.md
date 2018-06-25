---
title: FailedMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: L’élément FailedMailbox Spécifie le message d’erreur pour une boîte aux lettres ayant échoué sur la recherche.
ms.openlocfilehash: a4f5cd975eba121dd1d8d918b638d34f907588a8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756348"
---
# <a name="failedmailbox"></a><span data-ttu-id="c8e47-103">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="c8e47-103">FailedMailbox</span></span>

<span data-ttu-id="c8e47-104">L’élément **FailedMailbox** Spécifie le message d’erreur pour une boîte aux lettres ayant échoué sur la recherche.</span><span class="sxs-lookup"><span data-stu-id="c8e47-104">The **FailedMailbox** element specifies the error message for a mailbox that failed on search.</span></span> 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 <span data-ttu-id="c8e47-105">**FailedSearchMailboxType**</span><span class="sxs-lookup"><span data-stu-id="c8e47-105">**FailedSearchMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8e47-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c8e47-106">Attributes and elements</span></span>

<span data-ttu-id="c8e47-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c8e47-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8e47-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c8e47-108">Attributes</span></span>

<span data-ttu-id="c8e47-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c8e47-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8e47-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c8e47-110">Child elements</span></span>

|<span data-ttu-id="c8e47-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c8e47-111">**Element**</span></span>|<span data-ttu-id="c8e47-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c8e47-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8e47-113">Boîte aux lettres (chaîne)</span><span class="sxs-lookup"><span data-stu-id="c8e47-113">Mailbox (string)</span></span>](mailbox-string.md) <br/> |<span data-ttu-id="c8e47-114">Contient un identificateur pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c8e47-114">Contains an identifier for the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c8e47-115">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="c8e47-115">ErrorCode (int)</span></span>](errorcode-int.md) <br/> |<span data-ttu-id="c8e47-116">Spécifie le code d’erreur de la boîte aux lettres qui ont échoué à la recherche.</span><span class="sxs-lookup"><span data-stu-id="c8e47-116">Specifies the error code of the mailbox that failed the search.</span></span>  <br/> |
|[<span data-ttu-id="c8e47-117">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="c8e47-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="c8e47-118">Représente la raison de l’erreur de validation.</span><span class="sxs-lookup"><span data-stu-id="c8e47-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="c8e47-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="c8e47-119">IsArchive</span></span>](isarchive.md) <br/> |<span data-ttu-id="c8e47-120">Spécifie une valeur de type Boolean qui indique si la boîte aux lettres est une archive.</span><span class="sxs-lookup"><span data-stu-id="c8e47-120">Specifies a Boolean value that indicates whether the mailbox is an archive.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c8e47-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c8e47-121">Parent elements</span></span>

|<span data-ttu-id="c8e47-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c8e47-122">**Element**</span></span>|<span data-ttu-id="c8e47-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="c8e47-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8e47-124">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="c8e47-124">FailedMailboxes</span></span>](failedmailboxes.md) <br/> |<span data-ttu-id="c8e47-125">Spécifie un tableau de boîtes aux lettres ayant échoués.</span><span class="sxs-lookup"><span data-stu-id="c8e47-125">Specifies an array of failed mailboxes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c8e47-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="c8e47-126">Remarks</span></span>

<span data-ttu-id="c8e47-127">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c8e47-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c8e47-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c8e47-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8e47-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c8e47-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8e47-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c8e47-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c8e47-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c8e47-131">Schema Name</span></span>  <br/> |<span data-ttu-id="c8e47-132">Schéma type</span><span class="sxs-lookup"><span data-stu-id="c8e47-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="c8e47-133">Validation File</span><span class="sxs-lookup"><span data-stu-id="c8e47-133">Validation File</span></span>  <br/> |<span data-ttu-id="c8e47-134">types.xsd</span><span class="sxs-lookup"><span data-stu-id="c8e47-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c8e47-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c8e47-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c8e47-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c8e47-136">See also</span></span>



- [<span data-ttu-id="c8e47-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c8e47-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

