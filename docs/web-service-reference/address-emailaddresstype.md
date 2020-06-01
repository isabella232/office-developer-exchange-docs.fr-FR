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
description: L’élément Address représente une adresse de messagerie entièrement résolue.
ms.openlocfilehash: 591bc675165ec80f69407bd8ee19d16c9ddff15a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464902"
---
# <a name="address-emailaddresstype"></a><span data-ttu-id="e7783-103">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e7783-103">Address (EmailAddressType)</span></span>

<span data-ttu-id="e7783-104">L’élément **Address** représente une adresse de messagerie entièrement résolue.</span><span class="sxs-lookup"><span data-stu-id="e7783-104">The **Address** element represents a fully resolved e-mail address.</span></span> 
  
```XML
<Address>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Address >
```

 <span data-ttu-id="e7783-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="e7783-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7783-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e7783-106">Attributes and elements</span></span>

<span data-ttu-id="e7783-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e7783-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7783-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e7783-108">Attributes</span></span>

<span data-ttu-id="e7783-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e7783-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7783-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e7783-110">Child elements</span></span>

|<span data-ttu-id="e7783-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e7783-111">**Element**</span></span>|<span data-ttu-id="e7783-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e7783-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7783-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e7783-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="e7783-114">Définit le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e7783-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="e7783-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e7783-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e7783-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="e7783-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="e7783-117">Définit l’adresse SMTP (Simple Mail Transfer Protocol) d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e7783-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="e7783-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e7783-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e7783-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="e7783-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="e7783-120">Définit le routage utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e7783-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="e7783-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="e7783-121">The default is SMTP.</span></span> <span data-ttu-id="e7783-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e7783-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e7783-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="e7783-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="e7783-124">Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e7783-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="e7783-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e7783-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e7783-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="e7783-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e7783-127">Définit l’identificateur d’élément d’une liste de distribution privée ou de contact pour les destinataires à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e7783-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="e7783-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e7783-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e7783-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e7783-129">Parent elements</span></span>

|<span data-ttu-id="e7783-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e7783-130">**Element**</span></span>|<span data-ttu-id="e7783-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="e7783-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7783-132">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="e7783-132">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="e7783-133">Contient une collection d’adresses de messagerie qui représentent les destinataires d’origine d’un message suivi.</span><span class="sxs-lookup"><span data-stu-id="e7783-133">Contains a collection of e-mail addresses that represent the original recipients of a tracked message.</span></span>  <br/> |
|[<span data-ttu-id="e7783-134">RoomLists</span><span class="sxs-lookup"><span data-stu-id="e7783-134">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="e7783-135">Contient une liste de salles de réunion dans une organisation.</span><span class="sxs-lookup"><span data-stu-id="e7783-135">Contains a list of meeting rooms in an organization.</span></span>  <br/> |
|[<span data-ttu-id="e7783-136">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="e7783-136">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="e7783-137">Contient une liste des adresses de messagerie auxquelles les messages entrants doivent avoir été envoyés pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="e7783-137">Contains a list of e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7783-138">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e7783-138">Text value</span></span>

<span data-ttu-id="e7783-139">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e7783-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e7783-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="e7783-140">Remarks</span></span>

<span data-ttu-id="e7783-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7783-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7783-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e7783-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7783-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e7783-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7783-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e7783-144">Schema Name</span></span>  <br/> |<span data-ttu-id="e7783-145">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e7783-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="e7783-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e7783-146">Validation File</span></span>  <br/> |<span data-ttu-id="e7783-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e7783-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7783-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e7783-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="e7783-149">False</span><span class="sxs-lookup"><span data-stu-id="e7783-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7783-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e7783-150">See also</span></span>

- [<span data-ttu-id="e7783-151">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="e7783-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md) 
- [<span data-ttu-id="e7783-152">Opération GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="e7783-152">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="e7783-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e7783-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

