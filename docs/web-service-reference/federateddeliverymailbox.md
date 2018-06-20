---
title: FederatedDeliveryMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FederatedDeliveryMailbox
api_type:
- schema
ms.assetid: cd56bcc0-d24a-4e8b-87bd-999bf69234b7
description: L’élément FederatedDeliveryMailbox représente la boîte aux lettres à laquelle un message cross-site a été envoyé.
ms.openlocfilehash: 4a9250455f8de3ede25f2b5ba9433690137ca1d3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756351"
---
# <a name="federateddeliverymailbox"></a><span data-ttu-id="ad514-103">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="ad514-103">FederatedDeliveryMailbox</span></span>

<span data-ttu-id="ad514-104">L’élément **FederatedDeliveryMailbox** représente la boîte aux lettres à laquelle un message cross-site a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="ad514-104">The **FederatedDeliveryMailbox** element represents the mailbox to which a cross-premise message was sent.</span></span> 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 <span data-ttu-id="ad514-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="ad514-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad514-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad514-106">Attributes and elements</span></span>

<span data-ttu-id="ad514-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad514-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad514-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad514-108">Attributes</span></span>

<span data-ttu-id="ad514-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad514-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad514-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad514-110">Child elements</span></span>

|<span data-ttu-id="ad514-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad514-111">**Element**</span></span>|<span data-ttu-id="ad514-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad514-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad514-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ad514-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="ad514-114">Définit le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad514-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="ad514-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ad514-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad514-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="ad514-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="ad514-117">Définit l’adresse SMTP Simple Mail Transfer Protocol () d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad514-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="ad514-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ad514-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad514-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ad514-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="ad514-120">Définit le routage est utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad514-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="ad514-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="ad514-121">The default is SMTP.</span></span> <span data-ttu-id="ad514-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ad514-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad514-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="ad514-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="ad514-124">Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad514-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="ad514-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ad514-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad514-126">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="ad514-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ad514-127">Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires à partir du dossier de Contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ad514-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="ad514-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ad514-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad514-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad514-129">Parent elements</span></span>

|<span data-ttu-id="ad514-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad514-130">**Element**</span></span>|<span data-ttu-id="ad514-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad514-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad514-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="ad514-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="ad514-133">Contient des critères pour les types de messages.</span><span class="sxs-lookup"><span data-stu-id="ad514-133">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad514-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ad514-134">Text value</span></span>

<span data-ttu-id="ad514-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad514-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ad514-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="ad514-136">Remarks</span></span>

<span data-ttu-id="ad514-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad514-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad514-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad514-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad514-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad514-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ad514-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad514-140">Schema Name</span></span>  <br/> |<span data-ttu-id="ad514-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ad514-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ad514-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ad514-142">Validation File</span></span>  <br/> |<span data-ttu-id="ad514-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ad514-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ad514-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad514-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad514-145">False</span><span class="sxs-lookup"><span data-stu-id="ad514-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad514-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad514-146">See also</span></span>



- [<span data-ttu-id="ad514-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ad514-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

