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
description: L’élément d’entrée représente une adresse de messagerie unique pour un contact.
ms.openlocfilehash: 1852584e507c38da030815c37f85f7c4af4e2ba4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756192"
---
# <a name="entry-emailaddress"></a><span data-ttu-id="7013a-103">Entrée (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="7013a-103">Entry (EmailAddress)</span></span>

<span data-ttu-id="7013a-104">L’élément **d’entrée** représente une adresse de messagerie unique pour un contact.</span><span class="sxs-lookup"><span data-stu-id="7013a-104">The **Entry** element represents a single e-mail address for a contact.</span></span> 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

<span data-ttu-id="7013a-105">**EmailAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="7013a-105">**EmailAddressDictionaryEntryType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7013a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7013a-106">Attributes and elements</span></span>

<span data-ttu-id="7013a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7013a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7013a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7013a-108">Attributes</span></span>

|<span data-ttu-id="7013a-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7013a-109">**Attribute**</span></span>|<span data-ttu-id="7013a-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="7013a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7013a-111">**Clé**</span><span class="sxs-lookup"><span data-stu-id="7013a-111">**Key**</span></span> <br/> | <span data-ttu-id="7013a-112">Identifie l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="7013a-112">Identifies the e-mail address.</span></span><br/><br/><span data-ttu-id="7013a-113">Les valeurs possibles de cet attribut sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="7013a-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="7013a-114">-EmailAddress1</span><span class="sxs-lookup"><span data-stu-id="7013a-114">-  EmailAddress1</span></span>  <br/><span data-ttu-id="7013a-115">-EmailAddress2</span><span class="sxs-lookup"><span data-stu-id="7013a-115">-  EmailAddress2</span></span>  <br/><span data-ttu-id="7013a-116">-EmailAddress3</span><span class="sxs-lookup"><span data-stu-id="7013a-116">-  EmailAddress3</span></span> <br/><br/>  <span data-ttu-id="7013a-117">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="7013a-117">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="7013a-118">**Name**</span><span class="sxs-lookup"><span data-stu-id="7013a-118">**Name**</span></span> <br/> |<span data-ttu-id="7013a-119">Définit le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7013a-119">Defines the name of the mailbox user.</span></span> <span data-ttu-id="7013a-120">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7013a-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="7013a-121">**RoutingType**</span><span class="sxs-lookup"><span data-stu-id="7013a-121">**RoutingType**</span></span> <br/> |<span data-ttu-id="7013a-122">Définit le routage est utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7013a-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="7013a-123">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="7013a-123">The default is SMTP.</span></span> <span data-ttu-id="7013a-124">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7013a-124">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="7013a-125">**MailboxType**</span><span class="sxs-lookup"><span data-stu-id="7013a-125">**MailboxType**</span></span> <br/> |<span data-ttu-id="7013a-126">Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7013a-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="7013a-127">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7013a-127">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7013a-128">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7013a-128">Child elements</span></span>

<span data-ttu-id="7013a-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7013a-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7013a-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7013a-130">Parent elements</span></span>

|<span data-ttu-id="7013a-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7013a-131">**Element**</span></span>|<span data-ttu-id="7013a-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="7013a-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7013a-133">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="7013a-133">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="7013a-134">Représente une collection d'adresses de messagerie pour un contact.</span><span class="sxs-lookup"><span data-stu-id="7013a-134">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7013a-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="7013a-135">Remarks</span></span>

<span data-ttu-id="7013a-136">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7013a-136">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7013a-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7013a-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7013a-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7013a-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7013a-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7013a-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7013a-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7013a-140">Schema name</span></span>  <br/> |<span data-ttu-id="7013a-141">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7013a-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="7013a-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7013a-142">Validation file</span></span>  <br/> |<span data-ttu-id="7013a-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7013a-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7013a-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7013a-144">Can be empty</span></span>  <br/> |<span data-ttu-id="7013a-145">False</span><span class="sxs-lookup"><span data-stu-id="7013a-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7013a-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7013a-146">See also</span></span>

- [<span data-ttu-id="7013a-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7013a-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

