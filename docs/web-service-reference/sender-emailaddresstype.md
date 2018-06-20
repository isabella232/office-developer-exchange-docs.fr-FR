---
title: Expéditeur (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Sender
api_type:
- schema
ms.assetid: 717eb6d0-d167-4b20-92e2-5d08b96186c4
description: L’élément de l’expéditeur représente l’adresse de messagerie de l’expéditeur du message.
ms.openlocfilehash: bac62412caf1044c13015f1d9d7ef63552747c1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829320"
---
# <a name="sender-emailaddresstype"></a><span data-ttu-id="773d8-103">Expéditeur (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="773d8-103">Sender (EmailAddressType)</span></span>

<span data-ttu-id="773d8-104">L’élément de **l’expéditeur** représente l’adresse de messagerie de l’expéditeur du message.</span><span class="sxs-lookup"><span data-stu-id="773d8-104">The **Sender** element represents the e-mail address for the sender of the message.</span></span> 
  
```XML
<Sender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Sender>
```

 <span data-ttu-id="773d8-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="773d8-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="773d8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="773d8-106">Attributes and elements</span></span>

<span data-ttu-id="773d8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="773d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="773d8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="773d8-108">Attributes</span></span>

<span data-ttu-id="773d8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="773d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="773d8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="773d8-110">Child elements</span></span>

|<span data-ttu-id="773d8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="773d8-111">**Element**</span></span>|<span data-ttu-id="773d8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="773d8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="773d8-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="773d8-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="773d8-114">Représente le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="773d8-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="773d8-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="773d8-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="773d8-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="773d8-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="773d8-117">Définit l’adresse SMTP Simple Mail Transfer Protocol () principal d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="773d8-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="773d8-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="773d8-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="773d8-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="773d8-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="773d8-120">Représente le protocole de routage pour le destinataire.</span><span class="sxs-lookup"><span data-stu-id="773d8-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="773d8-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="773d8-121">The default value is SMTP.</span></span> <span data-ttu-id="773d8-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="773d8-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="773d8-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="773d8-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="773d8-124">Représente le type de boîte aux lettres qui est représenté par l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="773d8-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="773d8-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="773d8-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="773d8-126">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="773d8-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="773d8-127">Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires à partir du dossier de Contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="773d8-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="773d8-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="773d8-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="773d8-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="773d8-129">Parent elements</span></span>

|<span data-ttu-id="773d8-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="773d8-130">**Element**</span></span>|<span data-ttu-id="773d8-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="773d8-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="773d8-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="773d8-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="773d8-133">Spécifie les critères pour les types de messages.</span><span class="sxs-lookup"><span data-stu-id="773d8-133">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="773d8-134">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="773d8-134">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="773d8-135">Contient un résultat de message unique d’un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="773d8-135">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
|[<span data-ttu-id="773d8-136">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="773d8-136">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="773d8-137">Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="773d8-137">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="773d8-138">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="773d8-138">Text value</span></span>

<span data-ttu-id="773d8-139">Aucun.</span><span class="sxs-lookup"><span data-stu-id="773d8-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="773d8-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="773d8-140">Remarks</span></span>

<span data-ttu-id="773d8-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="773d8-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="773d8-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="773d8-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="773d8-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="773d8-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="773d8-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="773d8-144">Schema Name</span></span>  <br/> |<span data-ttu-id="773d8-145">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="773d8-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="773d8-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="773d8-146">Validation File</span></span>  <br/> |<span data-ttu-id="773d8-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="773d8-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="773d8-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="773d8-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="773d8-149">False</span><span class="sxs-lookup"><span data-stu-id="773d8-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="773d8-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="773d8-150">See also</span></span>



[<span data-ttu-id="773d8-151">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="773d8-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="773d8-152">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="773d8-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
