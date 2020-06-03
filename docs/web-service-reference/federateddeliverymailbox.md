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
description: L’élément FederatedDeliveryMailbox représente la boîte aux lettres à laquelle un message intersites a été envoyé.
ms.openlocfilehash: d493ed81e82237b7257e8c469f4552d931b73aa6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461946"
---
# <a name="federateddeliverymailbox"></a><span data-ttu-id="57e8d-103">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="57e8d-103">FederatedDeliveryMailbox</span></span>

<span data-ttu-id="57e8d-104">L’élément **FederatedDeliveryMailbox** représente la boîte aux lettres à laquelle un message intersites a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="57e8d-104">The **FederatedDeliveryMailbox** element represents the mailbox to which a cross-premise message was sent.</span></span> 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 <span data-ttu-id="57e8d-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="57e8d-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57e8d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="57e8d-106">Attributes and elements</span></span>

<span data-ttu-id="57e8d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="57e8d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57e8d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="57e8d-108">Attributes</span></span>

<span data-ttu-id="57e8d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="57e8d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57e8d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="57e8d-110">Child elements</span></span>

|<span data-ttu-id="57e8d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="57e8d-111">**Element**</span></span>|<span data-ttu-id="57e8d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="57e8d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57e8d-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="57e8d-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="57e8d-114">Définit le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="57e8d-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="57e8d-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="57e8d-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="57e8d-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="57e8d-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="57e8d-117">Définit l’adresse SMTP (Simple Mail Transfer Protocol) d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="57e8d-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="57e8d-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="57e8d-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="57e8d-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="57e8d-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="57e8d-120">Définit le routage utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="57e8d-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="57e8d-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="57e8d-121">The default is SMTP.</span></span> <span data-ttu-id="57e8d-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="57e8d-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="57e8d-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="57e8d-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="57e8d-124">Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="57e8d-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="57e8d-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="57e8d-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="57e8d-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="57e8d-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="57e8d-127">Définit l’identificateur d’élément d’une liste de distribution privée ou de contact pour les destinataires à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="57e8d-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="57e8d-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="57e8d-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57e8d-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="57e8d-129">Parent elements</span></span>

|<span data-ttu-id="57e8d-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="57e8d-130">**Element**</span></span>|<span data-ttu-id="57e8d-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="57e8d-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57e8d-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="57e8d-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="57e8d-133">Contient des critères pour les types de messages à rechercher.</span><span class="sxs-lookup"><span data-stu-id="57e8d-133">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57e8d-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="57e8d-134">Text value</span></span>

<span data-ttu-id="57e8d-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="57e8d-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57e8d-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="57e8d-136">Remarks</span></span>

<span data-ttu-id="57e8d-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="57e8d-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57e8d-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="57e8d-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57e8d-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="57e8d-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57e8d-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="57e8d-140">Schema Name</span></span>  <br/> |<span data-ttu-id="57e8d-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="57e8d-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="57e8d-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="57e8d-142">Validation File</span></span>  <br/> |<span data-ttu-id="57e8d-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="57e8d-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57e8d-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="57e8d-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="57e8d-145">False</span><span class="sxs-lookup"><span data-stu-id="57e8d-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57e8d-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="57e8d-146">See also</span></span>



- [<span data-ttu-id="57e8d-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="57e8d-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

