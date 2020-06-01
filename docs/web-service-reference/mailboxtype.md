---
title: MailboxType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxType
api_type:
- schema
ms.assetid: 696e5fdb-d8c5-40f0-9e79-885eae65dfa4
description: L’élément MailboxType représente le type de boîte aux lettres représenté par l’adresse de messagerie.
ms.openlocfilehash: 8c322ab8a87730832f5d199698a369656b058a9a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459797"
---
# <a name="mailboxtype"></a><span data-ttu-id="f2c49-103">MailboxType</span><span class="sxs-lookup"><span data-stu-id="f2c49-103">MailboxType</span></span>

<span data-ttu-id="f2c49-104">L’élément **MailboxType** représente le type de boîte aux lettres représenté par l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="f2c49-104">The **MailboxType** element represents the type of mailbox that is represented by the e-mail address.</span></span> 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

<span data-ttu-id="f2c49-105">**MailboxTypeType**</span><span class="sxs-lookup"><span data-stu-id="f2c49-105">**MailboxTypeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f2c49-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f2c49-106">Attributes and elements</span></span>

<span data-ttu-id="f2c49-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f2c49-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2c49-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f2c49-108">Attributes</span></span>

<span data-ttu-id="f2c49-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f2c49-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2c49-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f2c49-110">Child elements</span></span>

<span data-ttu-id="f2c49-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f2c49-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f2c49-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f2c49-112">Parent elements</span></span>

|<span data-ttu-id="f2c49-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f2c49-113">**Element**</span></span>|<span data-ttu-id="f2c49-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f2c49-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2c49-115">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="f2c49-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="f2c49-116">Identifie une adresse de messagerie entièrement résolue.</span><span class="sxs-lookup"><span data-stu-id="f2c49-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="f2c49-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="f2c49-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="f2c49-118">Identifie une liste de salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="f2c49-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f2c49-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f2c49-119">Text value</span></span>

<span data-ttu-id="f2c49-120">Le tableau suivant répertorie les valeurs possibles pour l’élément **MailboxType** .</span><span class="sxs-lookup"><span data-stu-id="f2c49-120">The following table lists the possible values for the **MailboxType** element.</span></span> 
  
|<span data-ttu-id="f2c49-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f2c49-121">**Value**</span></span>|<span data-ttu-id="f2c49-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="f2c49-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f2c49-123">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="f2c49-123">Mailbox</span></span>  <br/> |<span data-ttu-id="f2c49-124">Représente un objet Active Directory à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="f2c49-124">Represents a mail-enabled Active Directory object.</span></span>  <br/> |
|<span data-ttu-id="f2c49-125">PublicDL</span><span class="sxs-lookup"><span data-stu-id="f2c49-125">PublicDL</span></span>  <br/> |<span data-ttu-id="f2c49-126">Représente une liste de distribution publique.</span><span class="sxs-lookup"><span data-stu-id="f2c49-126">Represents a public distribution list.</span></span>  <br/> |
|<span data-ttu-id="f2c49-127">PrivateDL</span><span class="sxs-lookup"><span data-stu-id="f2c49-127">PrivateDL</span></span>  <br/> |<span data-ttu-id="f2c49-128">Représente une liste de distribution privée dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f2c49-128">Represents a private distribution list in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="f2c49-129">Contact</span><span class="sxs-lookup"><span data-stu-id="f2c49-129">Contact</span></span>  <br/> |<span data-ttu-id="f2c49-130">Représente un contact dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f2c49-130">Represents a contact in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="f2c49-131">PublicFolder</span><span class="sxs-lookup"><span data-stu-id="f2c49-131">PublicFolder</span></span>  <br/> |<span data-ttu-id="f2c49-132">Représente un dossier public.</span><span class="sxs-lookup"><span data-stu-id="f2c49-132">Represents a public folder.</span></span>  <br/> |
|<span data-ttu-id="f2c49-133">Inconnu</span><span class="sxs-lookup"><span data-stu-id="f2c49-133">Unknown</span></span>  <br/> |<span data-ttu-id="f2c49-134">Représente un type inconnu de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f2c49-134">Represents an unknown type of mailbox.</span></span>  <br/> |
|<span data-ttu-id="f2c49-135">OneOff</span><span class="sxs-lookup"><span data-stu-id="f2c49-135">OneOff</span></span>  <br/> |<span data-ttu-id="f2c49-136">Représente un membre unique d’une liste de distribution personnelle.</span><span class="sxs-lookup"><span data-stu-id="f2c49-136">Represents a one-off member of a personal distribution list.</span></span>  <br/> |
|<span data-ttu-id="f2c49-137">GroupMailbox</span><span class="sxs-lookup"><span data-stu-id="f2c49-137">GroupMailbox</span></span>  <br/> |<span data-ttu-id="f2c49-138">Représente une boîte aux lettres de groupe.</span><span class="sxs-lookup"><span data-stu-id="f2c49-138">Represents a group mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f2c49-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="f2c49-139">Remarks</span></span>

<span data-ttu-id="f2c49-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2c49-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2c49-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f2c49-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2c49-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f2c49-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2c49-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f2c49-143">Schema Name</span></span>  <br/> |<span data-ttu-id="f2c49-144">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f2c49-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2c49-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f2c49-145">Validation File</span></span>  <br/> |<span data-ttu-id="f2c49-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f2c49-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2c49-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f2c49-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2c49-148">False</span><span class="sxs-lookup"><span data-stu-id="f2c49-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2c49-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f2c49-149">See also</span></span>

- [<span data-ttu-id="f2c49-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f2c49-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

