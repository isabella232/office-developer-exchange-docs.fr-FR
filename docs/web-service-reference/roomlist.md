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
ms.openlocfilehash: 0444475cb9fffbb89ba2861096baee0c7e645995
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460518"
---
# <a name="roomlist"></a><span data-ttu-id="1001b-103">RoomList</span><span class="sxs-lookup"><span data-stu-id="1001b-103">RoomList</span></span>

<span data-ttu-id="1001b-104">L’élément **RoomList** représente une adresse de messagerie qui identifie une liste de salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="1001b-104">The **RoomList** element represents an e-mail address that identifies a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="1001b-105">GetRooms</span><span class="sxs-lookup"><span data-stu-id="1001b-105">GetRooms</span></span>](getrooms.md)
  
[<span data-ttu-id="1001b-106">RoomList</span><span class="sxs-lookup"><span data-stu-id="1001b-106">RoomList</span></span>](roomlist.md)
  
```XML
<RoomList>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RoomList>
```

 <span data-ttu-id="1001b-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="1001b-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1001b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1001b-108">Attributes and elements</span></span>

<span data-ttu-id="1001b-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1001b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1001b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="1001b-110">Attributes</span></span>

<span data-ttu-id="1001b-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1001b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1001b-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1001b-112">Child elements</span></span>

|<span data-ttu-id="1001b-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1001b-113">**Element**</span></span>|<span data-ttu-id="1001b-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1001b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1001b-115">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1001b-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="1001b-116">Définit le nom d’affichage de la liste de salles.</span><span class="sxs-lookup"><span data-stu-id="1001b-116">Defines the display name of the room list.</span></span> <span data-ttu-id="1001b-117">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="1001b-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1001b-118">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="1001b-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="1001b-119">Définit l’adresse SMTP (Simple Mail Transfer Protocol) d’une liste de salles.</span><span class="sxs-lookup"><span data-stu-id="1001b-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a room list.</span></span> <span data-ttu-id="1001b-120">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="1001b-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1001b-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="1001b-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="1001b-122">Définit le routage utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1001b-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="1001b-123">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="1001b-123">The default is SMTP.</span></span> <span data-ttu-id="1001b-124">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="1001b-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1001b-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="1001b-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="1001b-126">Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1001b-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="1001b-127">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="1001b-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1001b-128">ItemId</span><span class="sxs-lookup"><span data-stu-id="1001b-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="1001b-129">Définit l’identificateur d’élément d’une liste de distribution privée ou de contact pour les destinataires à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1001b-129">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="1001b-130">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="1001b-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1001b-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1001b-131">Parent elements</span></span>

|<span data-ttu-id="1001b-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1001b-132">**Element**</span></span>|<span data-ttu-id="1001b-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="1001b-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1001b-134">GetRooms</span><span class="sxs-lookup"><span data-stu-id="1001b-134">GetRooms</span></span>](getrooms.md) <br/> |<span data-ttu-id="1001b-135">Élément racine dans une demande pour obtenir une liste de salles dans une liste de salles particulière.</span><span class="sxs-lookup"><span data-stu-id="1001b-135">The root element in a request to get a list of rooms within a particular room list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1001b-136">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1001b-136">Text value</span></span>

<span data-ttu-id="1001b-137">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1001b-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1001b-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="1001b-138">Remarks</span></span>

<span data-ttu-id="1001b-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1001b-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1001b-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1001b-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1001b-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1001b-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1001b-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1001b-142">Schema Name</span></span>  <br/> |<span data-ttu-id="1001b-143">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1001b-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1001b-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1001b-144">Validation File</span></span>  <br/> |<span data-ttu-id="1001b-145">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1001b-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1001b-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1001b-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="1001b-147">False</span><span class="sxs-lookup"><span data-stu-id="1001b-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1001b-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1001b-148">See also</span></span>



[<span data-ttu-id="1001b-149">Opération GetRooms</span><span class="sxs-lookup"><span data-stu-id="1001b-149">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="1001b-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1001b-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

