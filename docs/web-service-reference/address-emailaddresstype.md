---
title: Adresse (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: 518641c8-7f6f-496c-86f9-341e7c1bb44c
description: L’élément adresse représente une adresse de messagerie entièrement résolu.
ms.openlocfilehash: 2a2d409edcc3a04bf82c6da0080183becfc9b25b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755249"
---
# <a name="address-emailaddresstype"></a><span data-ttu-id="8faf9-103">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8faf9-103">Address (EmailAddressType)</span></span>

<span data-ttu-id="8faf9-104">L’élément **adresse** représente une adresse de messagerie entièrement résolu.</span><span class="sxs-lookup"><span data-stu-id="8faf9-104">The **Address** element represents a fully resolved e-mail address.</span></span> 
  
```XML
<Address>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Address >
```

 <span data-ttu-id="8faf9-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="8faf9-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8faf9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8faf9-106">Attributes and elements</span></span>

<span data-ttu-id="8faf9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8faf9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8faf9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8faf9-108">Attributes</span></span>

<span data-ttu-id="8faf9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8faf9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8faf9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8faf9-110">Child elements</span></span>

|<span data-ttu-id="8faf9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8faf9-111">**Element**</span></span>|<span data-ttu-id="8faf9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8faf9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8faf9-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8faf9-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="8faf9-114">Définit le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8faf9-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="8faf9-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="8faf9-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8faf9-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="8faf9-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="8faf9-117">Définit l’adresse SMTP Simple Mail Transfer Protocol () d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8faf9-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="8faf9-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="8faf9-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8faf9-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="8faf9-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="8faf9-120">Définit le routage est utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8faf9-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="8faf9-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="8faf9-121">The default is SMTP.</span></span> <span data-ttu-id="8faf9-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="8faf9-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8faf9-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="8faf9-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="8faf9-124">Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8faf9-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="8faf9-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="8faf9-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8faf9-126">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="8faf9-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="8faf9-127">Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires à partir du dossier de Contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8faf9-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="8faf9-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="8faf9-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8faf9-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8faf9-129">Parent elements</span></span>

|<span data-ttu-id="8faf9-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8faf9-130">**Element**</span></span>|<span data-ttu-id="8faf9-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="8faf9-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8faf9-132">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="8faf9-132">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="8faf9-133">Contient une collection d’adresses de messagerie qui représentent les destinataires d’origine d’un message de suivi.</span><span class="sxs-lookup"><span data-stu-id="8faf9-133">Contains a collection of e-mail addresses that represent the original recipients of a tracked message.</span></span>  <br/> |
|[<span data-ttu-id="8faf9-134">RoomLists</span><span class="sxs-lookup"><span data-stu-id="8faf9-134">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="8faf9-135">Contient une liste de salles dans une organisation de réunions.</span><span class="sxs-lookup"><span data-stu-id="8faf9-135">Contains a list of meeting rooms in an organization.</span></span>  <br/> |
|[<span data-ttu-id="8faf9-136">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="8faf9-136">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="8faf9-137">Contient une liste d’adresses de messagerie dont les messages entrants ont été envoyées aux afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8faf9-137">Contains a list of e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8faf9-138">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8faf9-138">Text value</span></span>

<span data-ttu-id="8faf9-139">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8faf9-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8faf9-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="8faf9-140">Remarks</span></span>

<span data-ttu-id="8faf9-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8faf9-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8faf9-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8faf9-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8faf9-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8faf9-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8faf9-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8faf9-144">Schema Name</span></span>  <br/> |<span data-ttu-id="8faf9-145">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8faf9-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="8faf9-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8faf9-146">Validation File</span></span>  <br/> |<span data-ttu-id="8faf9-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8faf9-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8faf9-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8faf9-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="8faf9-149">False</span><span class="sxs-lookup"><span data-stu-id="8faf9-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8faf9-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8faf9-150">See also</span></span>

- [<span data-ttu-id="8faf9-151">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="8faf9-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md) 
- [<span data-ttu-id="8faf9-152">Opération GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="8faf9-152">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="8faf9-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8faf9-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

