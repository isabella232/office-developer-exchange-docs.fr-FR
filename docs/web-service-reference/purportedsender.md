---
title: PurportedSender
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PurportedSender
api_type:
- schema
ms.assetid: eb7a54ec-2e48-4030-bbcf-50a31609691b
description: L’élément PurportedSender contient les informations de contact pour l’expéditeur allégué d’un message électronique.
ms.openlocfilehash: 5ecf352484a423e3955736620bf5a65c4e98099a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468333"
---
# <a name="purportedsender"></a><span data-ttu-id="e77da-103">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="e77da-103">PurportedSender</span></span>

<span data-ttu-id="e77da-104">L’élément **PurportedSender** contient les informations de contact pour l’expéditeur allégué d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="e77da-104">The **PurportedSender** element contains contact information for the alleged sender of an e-mail message.</span></span> 
  
```XML
<PurportedSender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</PurportedSender>
```

 <span data-ttu-id="e77da-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="e77da-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e77da-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e77da-106">Attributes and elements</span></span>

<span data-ttu-id="e77da-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e77da-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e77da-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e77da-108">Attributes</span></span>

<span data-ttu-id="e77da-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e77da-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e77da-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e77da-110">Child elements</span></span>

|<span data-ttu-id="e77da-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e77da-111">**Element**</span></span>|<span data-ttu-id="e77da-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e77da-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e77da-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e77da-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="e77da-114">Représente le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e77da-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="e77da-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e77da-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e77da-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="e77da-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="e77da-117">Définit l’adresse SMTP (Simple Mail Transfer Protocol) d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e77da-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="e77da-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e77da-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e77da-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="e77da-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="e77da-120">Représente le protocole de routage pour le destinataire.</span><span class="sxs-lookup"><span data-stu-id="e77da-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="e77da-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="e77da-121">The default value is SMTP.</span></span> <span data-ttu-id="e77da-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e77da-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e77da-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="e77da-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="e77da-124">Représente le type de boîte aux lettres représenté par l’adresse de messagerie..</span><span class="sxs-lookup"><span data-stu-id="e77da-124">Represents the type of mailbox that is represented by the e-mail address..</span></span> <span data-ttu-id="e77da-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e77da-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e77da-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="e77da-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e77da-127">Définit l’identificateur d’élément d’une liste de distribution privée ou de contact pour les destinataires à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e77da-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="e77da-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e77da-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e77da-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e77da-129">Parent elements</span></span>

|<span data-ttu-id="e77da-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e77da-130">**Element**</span></span>|<span data-ttu-id="e77da-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="e77da-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e77da-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="e77da-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="e77da-133">Spécifie les critères pour les types de messages à rechercher.</span><span class="sxs-lookup"><span data-stu-id="e77da-133">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="e77da-134">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="e77da-134">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="e77da-135">Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e77da-135">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="e77da-136">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="e77da-136">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="e77da-137">Contient un seul résultat de message pour un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="e77da-137">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e77da-138">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e77da-138">Text value</span></span>

<span data-ttu-id="e77da-139">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e77da-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e77da-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="e77da-140">Remarks</span></span>

<span data-ttu-id="e77da-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e77da-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e77da-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e77da-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e77da-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e77da-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e77da-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e77da-144">Schema Name</span></span>  <br/> |<span data-ttu-id="e77da-145">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e77da-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e77da-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e77da-146">Validation File</span></span>  <br/> |<span data-ttu-id="e77da-147">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e77da-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e77da-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e77da-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="e77da-149">False</span><span class="sxs-lookup"><span data-stu-id="e77da-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e77da-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e77da-150">See also</span></span>



[<span data-ttu-id="e77da-151">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="e77da-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="e77da-152">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e77da-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

