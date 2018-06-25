---
title: RoomList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoomList
api_type:
- schema
ms.assetid: cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2
description: L’élément RoomList représente une adresse de messagerie qui identifie une liste de salles de réunion.
ms.openlocfilehash: 7de2c67f8001387abf463186933f0b81ee45a58a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829262"
---
# <a name="roomlist"></a><span data-ttu-id="e01ac-103">RoomList</span><span class="sxs-lookup"><span data-stu-id="e01ac-103">RoomList</span></span>

<span data-ttu-id="e01ac-104">L’élément **RoomList** représente une adresse de messagerie qui identifie une liste de salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="e01ac-104">The **RoomList** element represents an e-mail address that identifies a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="e01ac-105">GetRooms</span><span class="sxs-lookup"><span data-stu-id="e01ac-105">GetRooms</span></span>](getrooms.md)
  
[<span data-ttu-id="e01ac-106">RoomList</span><span class="sxs-lookup"><span data-stu-id="e01ac-106">RoomList</span></span>](roomlist.md)
  
```XML
<RoomList>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RoomList>
```

 <span data-ttu-id="e01ac-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="e01ac-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e01ac-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e01ac-108">Attributes and elements</span></span>

<span data-ttu-id="e01ac-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e01ac-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e01ac-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="e01ac-110">Attributes</span></span>

<span data-ttu-id="e01ac-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e01ac-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e01ac-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e01ac-112">Child elements</span></span>

|<span data-ttu-id="e01ac-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e01ac-113">**Element**</span></span>|<span data-ttu-id="e01ac-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="e01ac-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e01ac-115">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e01ac-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="e01ac-116">Définit le nom complet de la liste de salles.</span><span class="sxs-lookup"><span data-stu-id="e01ac-116">Defines the display name of the room list.</span></span> <span data-ttu-id="e01ac-117">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e01ac-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e01ac-118">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="e01ac-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="e01ac-119">Définit l’adresse SMTP Simple Mail Transfer Protocol () d’une liste de salles.</span><span class="sxs-lookup"><span data-stu-id="e01ac-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a room list.</span></span> <span data-ttu-id="e01ac-120">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e01ac-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e01ac-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="e01ac-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="e01ac-122">Définit le routage est utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e01ac-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="e01ac-123">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="e01ac-123">The default is SMTP.</span></span> <span data-ttu-id="e01ac-124">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e01ac-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e01ac-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="e01ac-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="e01ac-126">Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e01ac-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="e01ac-127">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e01ac-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e01ac-128">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="e01ac-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e01ac-129">Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires à partir du dossier de Contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e01ac-129">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="e01ac-130">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e01ac-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e01ac-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e01ac-131">Parent elements</span></span>

|<span data-ttu-id="e01ac-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e01ac-132">**Element**</span></span>|<span data-ttu-id="e01ac-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="e01ac-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e01ac-134">GetRooms</span><span class="sxs-lookup"><span data-stu-id="e01ac-134">GetRooms</span></span>](getrooms.md) <br/> |<span data-ttu-id="e01ac-135">L’élément racine dans une requête pour obtenir une liste de salles au sein d’une liste de salles particulier.</span><span class="sxs-lookup"><span data-stu-id="e01ac-135">The root element in a request to get a list of rooms within a particular room list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e01ac-136">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e01ac-136">Text value</span></span>

<span data-ttu-id="e01ac-137">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e01ac-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e01ac-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="e01ac-138">Remarks</span></span>

<span data-ttu-id="e01ac-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e01ac-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e01ac-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e01ac-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e01ac-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e01ac-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e01ac-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e01ac-142">Schema Name</span></span>  <br/> |<span data-ttu-id="e01ac-143">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e01ac-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e01ac-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e01ac-144">Validation File</span></span>  <br/> |<span data-ttu-id="e01ac-145">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e01ac-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e01ac-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e01ac-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="e01ac-147">False</span><span class="sxs-lookup"><span data-stu-id="e01ac-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e01ac-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e01ac-148">See also</span></span>



[<span data-ttu-id="e01ac-149">Opération GetRooms</span><span class="sxs-lookup"><span data-stu-id="e01ac-149">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="e01ac-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e01ac-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

