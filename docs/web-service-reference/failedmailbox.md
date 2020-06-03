---
title: FailedMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: L’élément FailedMailbox spécifie le message d’erreur pour une boîte aux lettres qui a échoué lors de la recherche.
ms.openlocfilehash: 404084bc342eb555db61c4216e936bee6ced9c36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461960"
---
# <a name="failedmailbox"></a><span data-ttu-id="b6e84-103">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="b6e84-103">FailedMailbox</span></span>

<span data-ttu-id="b6e84-104">L’élément **FailedMailbox** spécifie le message d’erreur pour une boîte aux lettres qui a échoué lors de la recherche.</span><span class="sxs-lookup"><span data-stu-id="b6e84-104">The **FailedMailbox** element specifies the error message for a mailbox that failed on search.</span></span> 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 <span data-ttu-id="b6e84-105">**FailedSearchMailboxType**</span><span class="sxs-lookup"><span data-stu-id="b6e84-105">**FailedSearchMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6e84-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b6e84-106">Attributes and elements</span></span>

<span data-ttu-id="b6e84-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b6e84-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6e84-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b6e84-108">Attributes</span></span>

<span data-ttu-id="b6e84-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b6e84-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6e84-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b6e84-110">Child elements</span></span>

|<span data-ttu-id="b6e84-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b6e84-111">**Element**</span></span>|<span data-ttu-id="b6e84-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b6e84-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6e84-113">Mailbox (String)</span><span class="sxs-lookup"><span data-stu-id="b6e84-113">Mailbox (string)</span></span>](mailbox-string.md) <br/> |<span data-ttu-id="b6e84-114">Contient un identificateur pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="b6e84-114">Contains an identifier for the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b6e84-115">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="b6e84-115">ErrorCode (int)</span></span>](errorcode-int.md) <br/> |<span data-ttu-id="b6e84-116">Spécifie le code d’erreur de la boîte aux lettres ayant échoué à la recherche.</span><span class="sxs-lookup"><span data-stu-id="b6e84-116">Specifies the error code of the mailbox that failed the search.</span></span>  <br/> |
|[<span data-ttu-id="b6e84-117">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="b6e84-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="b6e84-118">Représente la raison de l’erreur de validation.</span><span class="sxs-lookup"><span data-stu-id="b6e84-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="b6e84-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="b6e84-119">IsArchive</span></span>](isarchive.md) <br/> |<span data-ttu-id="b6e84-120">Spécifie une valeur de type Boolean qui indique si la boîte aux lettres est une archive.</span><span class="sxs-lookup"><span data-stu-id="b6e84-120">Specifies a Boolean value that indicates whether the mailbox is an archive.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b6e84-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b6e84-121">Parent elements</span></span>

|<span data-ttu-id="b6e84-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b6e84-122">**Element**</span></span>|<span data-ttu-id="b6e84-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="b6e84-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6e84-124">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="b6e84-124">FailedMailboxes</span></span>](failedmailboxes.md) <br/> |<span data-ttu-id="b6e84-125">Spécifie un tableau des boîtes aux lettres ayant échoué.</span><span class="sxs-lookup"><span data-stu-id="b6e84-125">Specifies an array of failed mailboxes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b6e84-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="b6e84-126">Remarks</span></span>

<span data-ttu-id="b6e84-127">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b6e84-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b6e84-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6e84-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6e84-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b6e84-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6e84-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b6e84-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6e84-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b6e84-131">Schema Name</span></span>  <br/> |<span data-ttu-id="b6e84-132">Schéma type</span><span class="sxs-lookup"><span data-stu-id="b6e84-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="b6e84-133">Validation File</span><span class="sxs-lookup"><span data-stu-id="b6e84-133">Validation File</span></span>  <br/> |<span data-ttu-id="b6e84-134">types. xsd</span><span class="sxs-lookup"><span data-stu-id="b6e84-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6e84-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b6e84-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b6e84-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b6e84-136">See also</span></span>



- [<span data-ttu-id="b6e84-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b6e84-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

