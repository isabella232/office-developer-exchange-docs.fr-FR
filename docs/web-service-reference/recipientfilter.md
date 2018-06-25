---
title: RecipientFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientFilter
api_type:
- schema
ms.assetid: 956c287a-a38a-49a7-a877-6d2088dfbc06
description: L’élément RecipientFilter représente une adresse de destinataire à utiliser avec le rapport de suivi de message spécifié.
ms.openlocfilehash: c31ed469132b110a690416b112d5e4e96e44c501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828972"
---
# <a name="recipientfilter"></a><span data-ttu-id="45185-103">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="45185-103">RecipientFilter</span></span>

<span data-ttu-id="45185-104">L’élément **RecipientFilter** représente une adresse de destinataire à utiliser avec le rapport de suivi de message spécifié.</span><span class="sxs-lookup"><span data-stu-id="45185-104">The **RecipientFilter** element represents a recipient address to use with the specified message tracking report.</span></span> 
  
```XML
 <RecipientFilter>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientFilter>
```

 <span data-ttu-id="45185-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="45185-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45185-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="45185-106">Attributes and elements</span></span>

<span data-ttu-id="45185-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="45185-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45185-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="45185-108">Attributes</span></span>

<span data-ttu-id="45185-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="45185-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="45185-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="45185-110">Child elements</span></span>

|<span data-ttu-id="45185-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="45185-111">**Element**</span></span>|<span data-ttu-id="45185-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="45185-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45185-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="45185-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="45185-114">Représente le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45185-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="45185-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="45185-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="45185-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="45185-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="45185-117">Définit l’adresse SMTP Simple Mail Transfer Protocol () principal d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45185-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="45185-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="45185-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="45185-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="45185-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="45185-120">Représente le protocole de routage pour ce destinataire.</span><span class="sxs-lookup"><span data-stu-id="45185-120">Represents the routing protocol for this recipient.</span></span> <span data-ttu-id="45185-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="45185-121">The default value is SMTP.</span></span> <span data-ttu-id="45185-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="45185-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="45185-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="45185-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="45185-124">Représente le type de boîte aux lettres qui est représenté par l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="45185-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="45185-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="45185-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="45185-126">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="45185-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="45185-127">Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires à partir du dossier de Contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="45185-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="45185-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="45185-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="45185-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="45185-129">Parent elements</span></span>

|<span data-ttu-id="45185-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="45185-130">**Element**</span></span>|<span data-ttu-id="45185-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="45185-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45185-132">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="45185-132">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="45185-133">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) récupérer le message complet suivi du rapport pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="45185-133">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="45185-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="45185-134">Text value</span></span>

<span data-ttu-id="45185-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="45185-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="45185-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="45185-136">Remarks</span></span>

<span data-ttu-id="45185-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="45185-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45185-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="45185-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45185-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="45185-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="45185-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="45185-140">Schema Name</span></span>  <br/> |<span data-ttu-id="45185-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="45185-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="45185-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="45185-142">Validation File</span></span>  <br/> |<span data-ttu-id="45185-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="45185-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="45185-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="45185-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="45185-145">False</span><span class="sxs-lookup"><span data-stu-id="45185-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45185-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="45185-146">See also</span></span>



[<span data-ttu-id="45185-147">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="45185-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="45185-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="45185-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

