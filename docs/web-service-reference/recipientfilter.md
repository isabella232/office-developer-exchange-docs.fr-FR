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
description: L’élément RecipientFilter représente une adresse de destinataire à utiliser avec le rapport de suivi des messages spécifié.
ms.openlocfilehash: 945adf9155434e0690debfccc7caf70ba0cb94ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465806"
---
# <a name="recipientfilter"></a><span data-ttu-id="20de0-103">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="20de0-103">RecipientFilter</span></span>

<span data-ttu-id="20de0-104">L’élément **RecipientFilter** représente une adresse de destinataire à utiliser avec le rapport de suivi des messages spécifié.</span><span class="sxs-lookup"><span data-stu-id="20de0-104">The **RecipientFilter** element represents a recipient address to use with the specified message tracking report.</span></span> 
  
```XML
 <RecipientFilter>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientFilter>
```

 <span data-ttu-id="20de0-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="20de0-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20de0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="20de0-106">Attributes and elements</span></span>

<span data-ttu-id="20de0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="20de0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20de0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="20de0-108">Attributes</span></span>

<span data-ttu-id="20de0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="20de0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20de0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="20de0-110">Child elements</span></span>

|<span data-ttu-id="20de0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20de0-111">**Element**</span></span>|<span data-ttu-id="20de0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="20de0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20de0-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="20de0-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="20de0-114">Représente le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="20de0-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="20de0-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="20de0-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="20de0-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="20de0-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="20de0-117">Définit l’adresse SMTP (Simple Mail Transfer Protocol) principale d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="20de0-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="20de0-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="20de0-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="20de0-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="20de0-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="20de0-120">Représente le protocole de routage de ce destinataire.</span><span class="sxs-lookup"><span data-stu-id="20de0-120">Represents the routing protocol for this recipient.</span></span> <span data-ttu-id="20de0-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="20de0-121">The default value is SMTP.</span></span> <span data-ttu-id="20de0-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="20de0-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="20de0-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="20de0-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="20de0-124">Représente le type de boîte aux lettres représenté par l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="20de0-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="20de0-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="20de0-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="20de0-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="20de0-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="20de0-127">Définit l’identificateur d’élément d’une liste de distribution privée ou de contact pour les destinataires à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="20de0-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="20de0-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="20de0-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="20de0-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="20de0-129">Parent elements</span></span>

|<span data-ttu-id="20de0-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20de0-130">**Element**</span></span>|<span data-ttu-id="20de0-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="20de0-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20de0-132">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="20de0-132">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="20de0-133">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) afin de récupérer le rapport de suivi complet des messages pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="20de0-133">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20de0-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="20de0-134">Text value</span></span>

<span data-ttu-id="20de0-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="20de0-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="20de0-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="20de0-136">Remarks</span></span>

<span data-ttu-id="20de0-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="20de0-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20de0-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="20de0-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20de0-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="20de0-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="20de0-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="20de0-140">Schema Name</span></span>  <br/> |<span data-ttu-id="20de0-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="20de0-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="20de0-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="20de0-142">Validation File</span></span>  <br/> |<span data-ttu-id="20de0-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="20de0-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="20de0-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="20de0-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="20de0-145">False</span><span class="sxs-lookup"><span data-stu-id="20de0-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20de0-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="20de0-146">See also</span></span>



[<span data-ttu-id="20de0-147">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="20de0-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="20de0-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="20de0-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

