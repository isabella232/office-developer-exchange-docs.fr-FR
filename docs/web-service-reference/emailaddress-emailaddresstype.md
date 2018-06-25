---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: L’élément EmailAddress spécifie l’adresse SMTP entièrement résolu pour la boîte aux lettres de site ou le personnage associé.
ms.openlocfilehash: c31a37fc0dbdcc2b501b82346a17a0a3b4775556
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756100"
---
# <a name="emailaddress-emailaddresstype"></a><span data-ttu-id="ad566-103">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ad566-103">EmailAddress (EmailAddressType)</span></span>

<span data-ttu-id="ad566-104">L’élément **EmailAddress** Spécifie l’adresse SMTP entièrement résolu pour la boîte aux lettres de site ou le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="ad566-104">The **EmailAddress** element specifies the fully resolved SMTP address for the site mailbox or the associated persona.</span></span> 
  
```xml
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
</EmailAddress>
```

 <span data-ttu-id="ad566-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="ad566-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad566-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad566-106">Attributes and elements</span></span>

<span data-ttu-id="ad566-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad566-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad566-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad566-108">Attributes</span></span>

<span data-ttu-id="ad566-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad566-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad566-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad566-110">Child elements</span></span>

|<span data-ttu-id="ad566-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad566-111">**Element**</span></span>|<span data-ttu-id="ad566-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad566-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad566-113">Name (chaîne)</span><span class="sxs-lookup"><span data-stu-id="ad566-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="ad566-114">Spécifie un nom d’affinement de recherche ou la clé ou le nom d’un utilisateur de messagerie.</span><span class="sxs-lookup"><span data-stu-id="ad566-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="ad566-115">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="ad566-115">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="ad566-116">Définit l’adresse SMTP principale d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad566-116">Defines the primary SMTP address of a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="ad566-117">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ad566-117">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md) <br/> |<span data-ttu-id="ad566-118">Spécifie le type de routage d’une adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="ad566-118">Specifies the routing type of an email address.</span></span>  <br/> |
|[<span data-ttu-id="ad566-119">MailboxType</span><span class="sxs-lookup"><span data-stu-id="ad566-119">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="ad566-120">Représente le type de boîte aux lettres qui est représenté par l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="ad566-120">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="ad566-121">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="ad566-121">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ad566-122">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad566-122">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad566-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad566-123">Parent elements</span></span>

|<span data-ttu-id="ad566-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad566-124">**Element**</span></span>|<span data-ttu-id="ad566-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad566-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad566-126">Personnage</span><span class="sxs-lookup"><span data-stu-id="ad566-126">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="ad566-127">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="ad566-127">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad566-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ad566-128">Text value</span></span>

<span data-ttu-id="ad566-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad566-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ad566-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="ad566-130">Remarks</span></span>

<span data-ttu-id="ad566-131">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ad566-131">This element is optional.</span></span>
  
<span data-ttu-id="ad566-132">L’élément **EmailAddress** est applicable pour les clients qui ciblent Exchange Online et les versions de Microsoft Exchange Server commençant par Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ad566-132">The **EmailAddress** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ad566-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad566-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad566-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad566-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad566-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad566-135">Schema Name</span></span>  <br/> |<span data-ttu-id="ad566-136">Schéma type</span><span class="sxs-lookup"><span data-stu-id="ad566-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="ad566-137">Validation File</span><span class="sxs-lookup"><span data-stu-id="ad566-137">Validation File</span></span>  <br/> |<span data-ttu-id="ad566-138">types.xsd</span><span class="sxs-lookup"><span data-stu-id="ad566-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad566-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad566-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ad566-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad566-140">See also</span></span>

- [<span data-ttu-id="ad566-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ad566-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

