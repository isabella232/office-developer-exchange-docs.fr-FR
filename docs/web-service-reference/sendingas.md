---
title: SendingAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendingAs
api_type:
- schema
ms.assetid: b43ce19f-9ab0-4946-acb2-c5aafead9d35
description: L’élément SendingAs représente une adresse de messagerie qu’un utilisateur tente d’envoyer en tant que.
ms.openlocfilehash: a5468ddb8facf99038d319252f7e1c780a888ca1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829338"
---
# <a name="sendingas"></a><span data-ttu-id="566b4-103">SendingAs</span><span class="sxs-lookup"><span data-stu-id="566b4-103">SendingAs</span></span>

<span data-ttu-id="566b4-104">L’élément **SendingAs** représente une adresse de messagerie qu’un utilisateur tente d’envoyer en tant que.</span><span class="sxs-lookup"><span data-stu-id="566b4-104">The **SendingAs** element represents an e-mail address that a user is trying to send as.</span></span> 
  
```XML
<SendingAs>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</SendingAs>
```

 <span data-ttu-id="566b4-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="566b4-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="566b4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="566b4-106">Attributes and elements</span></span>

<span data-ttu-id="566b4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="566b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="566b4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="566b4-108">Attributes</span></span>

<span data-ttu-id="566b4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="566b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="566b4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="566b4-110">Child elements</span></span>

|<span data-ttu-id="566b4-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="566b4-111">**Element**</span></span>|<span data-ttu-id="566b4-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="566b4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="566b4-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="566b4-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="566b4-114">Représente le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="566b4-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="566b4-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="566b4-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="566b4-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="566b4-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="566b4-117">Définit l’adresse SMTP Simple Mail Transfer Protocol () principal d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="566b4-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="566b4-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="566b4-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="566b4-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="566b4-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="566b4-120">Définit le type d’adresse pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="566b4-120">Defines the address type for the mailbox.</span></span> <span data-ttu-id="566b4-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="566b4-121">The default is SMTP.</span></span> <span data-ttu-id="566b4-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="566b4-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="566b4-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="566b4-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="566b4-124">Représente le type de boîte aux lettres qui est représenté par un utilisateur de messagerie.</span><span class="sxs-lookup"><span data-stu-id="566b4-124">Represents the type of mailbox that is represented by an e-mail user.</span></span> <span data-ttu-id="566b4-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="566b4-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="566b4-126">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="566b4-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="566b4-127">Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires à partir du dossier de Contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="566b4-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="566b4-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="566b4-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="566b4-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="566b4-129">Parent elements</span></span>

|<span data-ttu-id="566b4-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="566b4-130">**Element**</span></span>|<span data-ttu-id="566b4-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="566b4-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="566b4-132">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="566b4-132">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="566b4-133">Contient les destinataires et les types de conseils de messagerie à récupérer.</span><span class="sxs-lookup"><span data-stu-id="566b4-133">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="566b4-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="566b4-134">Text value</span></span>

<span data-ttu-id="566b4-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="566b4-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="566b4-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="566b4-136">Remarks</span></span>

<span data-ttu-id="566b4-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="566b4-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="566b4-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="566b4-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="566b4-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="566b4-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="566b4-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="566b4-140">Schema Name</span></span>  <br/> |<span data-ttu-id="566b4-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="566b4-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="566b4-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="566b4-142">Validation File</span></span>  <br/> |<span data-ttu-id="566b4-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="566b4-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="566b4-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="566b4-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="566b4-145">False</span><span class="sxs-lookup"><span data-stu-id="566b4-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="566b4-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="566b4-146">See also</span></span>



- [<span data-ttu-id="566b4-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="566b4-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
