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
description: L’élément Recipient représente le destinataire pour lequel l’événement s’est produit.
ms.openlocfilehash: eb7e85acf3c2b898b3f0bff4b63168d344e1daa8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465855"
---
# <a name="recipient"></a><span data-ttu-id="40061-103">Destinataire</span><span class="sxs-lookup"><span data-stu-id="40061-103">Recipient</span></span>

<span data-ttu-id="40061-104">L’élément **Recipient** représente le destinataire pour lequel l’événement s’est produit.</span><span class="sxs-lookup"><span data-stu-id="40061-104">The **Recipient** element represents the recipient for whom the event occurred.</span></span> 
  
```XML
<Recipient>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Recipient>
```

 <span data-ttu-id="40061-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="40061-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40061-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="40061-106">Attributes and elements</span></span>

<span data-ttu-id="40061-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="40061-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40061-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="40061-108">Attributes</span></span>

<span data-ttu-id="40061-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="40061-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40061-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="40061-110">Child elements</span></span>

|<span data-ttu-id="40061-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="40061-111">**Element**</span></span>|<span data-ttu-id="40061-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="40061-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40061-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="40061-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="40061-114">Représente le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="40061-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="40061-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="40061-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="40061-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="40061-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="40061-117">Définit l’adresse SMTP (Simple Mail Transfer Protocol) principale d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="40061-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="40061-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="40061-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="40061-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="40061-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="40061-120">Définit le routage utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="40061-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="40061-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="40061-121">The default value is SMTP.</span></span> <span data-ttu-id="40061-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="40061-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="40061-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="40061-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="40061-124">Représente le type de boîte aux lettres représenté par l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="40061-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="40061-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="40061-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="40061-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="40061-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="40061-127">Définit l’identificateur d’élément d’une liste de distribution privée ou de contact pour les destinataires à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="40061-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="40061-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="40061-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="40061-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="40061-129">Parent elements</span></span>

|<span data-ttu-id="40061-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="40061-130">**Element**</span></span>|<span data-ttu-id="40061-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="40061-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40061-132">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="40061-132">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="40061-133">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="40061-133">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="40061-134">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="40061-134">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="40061-135">Spécifie les critères pour les types de messages à rechercher.</span><span class="sxs-lookup"><span data-stu-id="40061-135">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="40061-136">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="40061-136">Text value</span></span>

<span data-ttu-id="40061-137">Aucun.</span><span class="sxs-lookup"><span data-stu-id="40061-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="40061-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="40061-138">Remarks</span></span>

<span data-ttu-id="40061-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="40061-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40061-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="40061-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40061-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="40061-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="40061-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="40061-142">Schema Name</span></span>  <br/> |<span data-ttu-id="40061-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="40061-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="40061-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="40061-144">Validation File</span></span>  <br/> |<span data-ttu-id="40061-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="40061-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="40061-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="40061-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="40061-147">False</span><span class="sxs-lookup"><span data-stu-id="40061-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40061-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="40061-148">See also</span></span>



- [<span data-ttu-id="40061-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="40061-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

