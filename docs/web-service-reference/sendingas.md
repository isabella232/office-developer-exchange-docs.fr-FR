---
title: Envoyeras
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
description: L’élément SendAs représente une adresse de messagerie électronique qu’un utilisateur tente d’envoyer en tant que.
ms.openlocfilehash: cd11bd60cbbe3434fcc1b0b9a1cfe0de9f0b1e21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462135"
---
# <a name="sendingas"></a><span data-ttu-id="9d089-103">Envoyeras</span><span class="sxs-lookup"><span data-stu-id="9d089-103">SendingAs</span></span>

<span data-ttu-id="9d089-104">L’élément **SendAs** représente une adresse de messagerie électronique qu’un utilisateur tente d’envoyer en tant que.</span><span class="sxs-lookup"><span data-stu-id="9d089-104">The **SendingAs** element represents an e-mail address that a user is trying to send as.</span></span> 
  
```XML
<SendingAs>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</SendingAs>
```

 <span data-ttu-id="9d089-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="9d089-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d089-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9d089-106">Attributes and elements</span></span>

<span data-ttu-id="9d089-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9d089-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d089-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9d089-108">Attributes</span></span>

<span data-ttu-id="9d089-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9d089-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d089-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9d089-110">Child elements</span></span>

|<span data-ttu-id="9d089-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9d089-111">**Element**</span></span>|<span data-ttu-id="9d089-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9d089-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d089-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="9d089-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="9d089-114">Représente le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9d089-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="9d089-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="9d089-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9d089-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="9d089-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="9d089-117">Définit l’adresse SMTP (Simple Mail Transfer Protocol) principale d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9d089-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="9d089-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="9d089-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9d089-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="9d089-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="9d089-120">Définit le type d’adresse de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9d089-120">Defines the address type for the mailbox.</span></span> <span data-ttu-id="9d089-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="9d089-121">The default is SMTP.</span></span> <span data-ttu-id="9d089-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="9d089-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9d089-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="9d089-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="9d089-124">Représente le type de boîte aux lettres représenté par un utilisateur de messagerie.</span><span class="sxs-lookup"><span data-stu-id="9d089-124">Represents the type of mailbox that is represented by an e-mail user.</span></span> <span data-ttu-id="9d089-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="9d089-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9d089-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="9d089-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9d089-127">Définit l’identificateur d’élément d’une liste de distribution privée ou de contact pour les destinataires à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9d089-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="9d089-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="9d089-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d089-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9d089-129">Parent elements</span></span>

|<span data-ttu-id="9d089-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9d089-130">**Element**</span></span>|<span data-ttu-id="9d089-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="9d089-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d089-132">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="9d089-132">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="9d089-133">Contient les destinataires et les types de conseils de messagerie à récupérer.</span><span class="sxs-lookup"><span data-stu-id="9d089-133">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9d089-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9d089-134">Text value</span></span>

<span data-ttu-id="9d089-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9d089-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d089-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="9d089-136">Remarks</span></span>

<span data-ttu-id="9d089-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d089-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d089-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9d089-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d089-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9d089-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d089-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9d089-140">Schema Name</span></span>  <br/> |<span data-ttu-id="9d089-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9d089-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9d089-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9d089-142">Validation File</span></span>  <br/> |<span data-ttu-id="9d089-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9d089-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d089-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9d089-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d089-145">False</span><span class="sxs-lookup"><span data-stu-id="9d089-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d089-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9d089-146">See also</span></span>



- [<span data-ttu-id="9d089-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9d089-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

