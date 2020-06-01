---
title: Entrée (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: b028c5c7-3494-4ecd-96d1-78783daa660f
description: L’élément Entry représente une adresse de messagerie unique pour un contact.
ms.openlocfilehash: 766d67cda10b02c07a7677e541fddfc38a4285cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459643"
---
# <a name="entry-emailaddress"></a><span data-ttu-id="7a303-103">Entrée (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="7a303-103">Entry (EmailAddress)</span></span>

<span data-ttu-id="7a303-104">L’élément **entry** représente une adresse de messagerie unique pour un contact.</span><span class="sxs-lookup"><span data-stu-id="7a303-104">The **Entry** element represents a single e-mail address for a contact.</span></span> 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

<span data-ttu-id="7a303-105">**EmailAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="7a303-105">**EmailAddressDictionaryEntryType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7a303-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7a303-106">Attributes and elements</span></span>

<span data-ttu-id="7a303-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7a303-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a303-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7a303-108">Attributes</span></span>

|<span data-ttu-id="7a303-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7a303-109">**Attribute**</span></span>|<span data-ttu-id="7a303-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a303-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7a303-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="7a303-111">**Key**</span></span> <br/> | <span data-ttu-id="7a303-112">Identifie l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="7a303-112">Identifies the e-mail address.</span></span><br/><br/><span data-ttu-id="7a303-113">Les valeurs possibles pour cet attribut sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="7a303-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="7a303-114">- EmailAddress1</span><span class="sxs-lookup"><span data-stu-id="7a303-114">-  EmailAddress1</span></span>  <br/><span data-ttu-id="7a303-115">- EmailAddress2</span><span class="sxs-lookup"><span data-stu-id="7a303-115">-  EmailAddress2</span></span>  <br/><span data-ttu-id="7a303-116">- EmailAddress3</span><span class="sxs-lookup"><span data-stu-id="7a303-116">-  EmailAddress3</span></span> <br/><br/>  <span data-ttu-id="7a303-117">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="7a303-117">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="7a303-118">**Name**</span><span class="sxs-lookup"><span data-stu-id="7a303-118">**Name**</span></span> <br/> |<span data-ttu-id="7a303-119">Définit le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7a303-119">Defines the name of the mailbox user.</span></span> <span data-ttu-id="7a303-120">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7a303-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="7a303-121">**RoutingType**</span><span class="sxs-lookup"><span data-stu-id="7a303-121">**RoutingType**</span></span> <br/> |<span data-ttu-id="7a303-122">Définit le routage utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7a303-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="7a303-123">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="7a303-123">The default is SMTP.</span></span> <span data-ttu-id="7a303-124">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7a303-124">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="7a303-125">**MailboxType**</span><span class="sxs-lookup"><span data-stu-id="7a303-125">**MailboxType**</span></span> <br/> |<span data-ttu-id="7a303-126">Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7a303-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="7a303-127">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7a303-127">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7a303-128">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7a303-128">Child elements</span></span>

<span data-ttu-id="7a303-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7a303-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7a303-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7a303-130">Parent elements</span></span>

|<span data-ttu-id="7a303-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7a303-131">**Element**</span></span>|<span data-ttu-id="7a303-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a303-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a303-133">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="7a303-133">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="7a303-134">Représente une collection d'adresses de messagerie pour un contact.</span><span class="sxs-lookup"><span data-stu-id="7a303-134">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a303-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="7a303-135">Remarks</span></span>

<span data-ttu-id="7a303-136">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7a303-136">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7a303-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a303-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a303-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7a303-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a303-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7a303-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a303-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7a303-140">Schema name</span></span>  <br/> |<span data-ttu-id="7a303-141">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7a303-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a303-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7a303-142">Validation file</span></span>  <br/> |<span data-ttu-id="7a303-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7a303-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a303-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7a303-144">Can be empty</span></span>  <br/> |<span data-ttu-id="7a303-145">False</span><span class="sxs-lookup"><span data-stu-id="7a303-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a303-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7a303-146">See also</span></span>

- [<span data-ttu-id="7a303-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7a303-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

