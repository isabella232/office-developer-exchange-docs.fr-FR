---
title: Destinataire
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipient
api_type:
- schema
ms.assetid: 52adbb30-3bfd-48aa-9ea8-9f7d3b4bee44
description: L’élément destinataire représente le destinataire pour lequel l’événement s’est produite.
ms.openlocfilehash: e8e8f9d6031d27c7441017c85eb26a143258b183
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828971"
---
# <a name="recipient"></a><span data-ttu-id="7bb5c-103">Destinataire</span><span class="sxs-lookup"><span data-stu-id="7bb5c-103">Recipient</span></span>

<span data-ttu-id="7bb5c-104">L’élément **destinataire** représente le destinataire pour lequel l’événement s’est produite.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-104">The **Recipient** element represents the recipient for whom the event occurred.</span></span> 
  
```XML
<Recipient>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Recipient>
```

 <span data-ttu-id="7bb5c-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="7bb5c-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7bb5c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7bb5c-106">Attributes and elements</span></span>

<span data-ttu-id="7bb5c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7bb5c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7bb5c-108">Attributes</span></span>

<span data-ttu-id="7bb5c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7bb5c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7bb5c-110">Child elements</span></span>

|<span data-ttu-id="7bb5c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7bb5c-111">**Element**</span></span>|<span data-ttu-id="7bb5c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7bb5c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7bb5c-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7bb5c-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="7bb5c-114">Représente le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="7bb5c-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7bb5c-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="7bb5c-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="7bb5c-117">Définit l’adresse SMTP Simple Mail Transfer Protocol () principal d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="7bb5c-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7bb5c-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="7bb5c-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="7bb5c-120">Définit le routage est utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="7bb5c-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-121">The default value is SMTP.</span></span> <span data-ttu-id="7bb5c-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7bb5c-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="7bb5c-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="7bb5c-124">Représente le type de boîte aux lettres qui est représenté par l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="7bb5c-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7bb5c-126">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="7bb5c-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7bb5c-127">Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires à partir du dossier de Contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="7bb5c-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7bb5c-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7bb5c-129">Parent elements</span></span>

|<span data-ttu-id="7bb5c-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7bb5c-130">**Element**</span></span>|<span data-ttu-id="7bb5c-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="7bb5c-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7bb5c-132">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="7bb5c-132">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="7bb5c-133">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-133">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="7bb5c-134">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7bb5c-134">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="7bb5c-135">Spécifie les critères pour les types de messages.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-135">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7bb5c-136">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7bb5c-136">Text value</span></span>

<span data-ttu-id="7bb5c-137">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7bb5c-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="7bb5c-138">Remarks</span></span>

<span data-ttu-id="7bb5c-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bb5c-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7bb5c-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7bb5c-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7bb5c-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7bb5c-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7bb5c-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7bb5c-142">Schema Name</span></span>  <br/> |<span data-ttu-id="7bb5c-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7bb5c-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="7bb5c-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7bb5c-144">Validation File</span></span>  <br/> |<span data-ttu-id="7bb5c-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7bb5c-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7bb5c-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7bb5c-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="7bb5c-147">False</span><span class="sxs-lookup"><span data-stu-id="7bb5c-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7bb5c-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7bb5c-148">See also</span></span>



- [<span data-ttu-id="7bb5c-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7bb5c-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
