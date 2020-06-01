---
title: ID (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Id
api_type:
- schema
ms.assetid: 3e1e37b5-5469-4447-ad1f-c2c6d4e0482f
description: L’élément ID identifie une salle de réunion au sein de l’organisation Exchange Server.
ms.openlocfilehash: aa09e7764746ac6bc283de2d13248d769aba75b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460777"
---
# <a name="id-emailaddresstype"></a><span data-ttu-id="ffd7c-103">ID (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ffd7c-103">Id (EmailAddressType)</span></span>

<span data-ttu-id="ffd7c-104">L’élément **ID** identifie une salle de réunion au sein de l’organisation Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-104">The **Id** element identifies a meeting room within the Exchange server organization.</span></span> 
  
[<span data-ttu-id="ffd7c-105">Salle</span><span class="sxs-lookup"><span data-stu-id="ffd7c-105">Room</span></span>](room.md)
  
[<span data-ttu-id="ffd7c-106">ID (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ffd7c-106">Id (EmailAddressType)</span></span>](id-emailaddresstype.md)
  
```xml
<Id>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Id>
```

 <span data-ttu-id="ffd7c-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="ffd7c-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffd7c-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ffd7c-108">Attributes and elements</span></span>

<span data-ttu-id="ffd7c-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffd7c-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="ffd7c-110">Attributes</span></span>

<span data-ttu-id="ffd7c-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffd7c-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ffd7c-112">Child elements</span></span>

|<span data-ttu-id="ffd7c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ffd7c-113">**Element**</span></span>|<span data-ttu-id="ffd7c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ffd7c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffd7c-115">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ffd7c-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="ffd7c-116">Définit le nom de la salle de réunion.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-116">Defines the name of the meeting room.</span></span> <span data-ttu-id="ffd7c-117">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ffd7c-118">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="ffd7c-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="ffd7c-119">Définit l’adresse SMTP (Simple Mail Transfer Protocol) d’une salle de réunion.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a meeting room.</span></span> <span data-ttu-id="ffd7c-120">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ffd7c-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ffd7c-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="ffd7c-122">Définit le routage utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="ffd7c-123">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-123">The default is SMTP.</span></span> <span data-ttu-id="ffd7c-124">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ffd7c-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="ffd7c-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="ffd7c-126">Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="ffd7c-127">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ffd7c-128">ItemId</span><span class="sxs-lookup"><span data-stu-id="ffd7c-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ffd7c-129">Définit l’identificateur d’élément d’une liste de distribution privée ou de contact pour les destinataires à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-129">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="ffd7c-130">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ffd7c-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ffd7c-131">Parent elements</span></span>

|<span data-ttu-id="ffd7c-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ffd7c-132">**Element**</span></span>|<span data-ttu-id="ffd7c-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="ffd7c-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffd7c-134">Salle</span><span class="sxs-lookup"><span data-stu-id="ffd7c-134">Room</span></span>](room.md) <br/> |<span data-ttu-id="ffd7c-135">Définit une salle de réunion dans l’organisation Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-135">Defines a meeting room in the Exchange server organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ffd7c-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="ffd7c-136">Remarks</span></span>

<span data-ttu-id="ffd7c-137">Le schéma qui décrit cet élément se trouve dans le répertoire EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ffd7c-137">The schema that describes this element is located in the EWS directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffd7c-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ffd7c-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffd7c-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ffd7c-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ffd7c-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ffd7c-140">Schema Name</span></span>  <br/> |<span data-ttu-id="ffd7c-141">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ffd7c-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="ffd7c-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ffd7c-142">Validation File</span></span>  <br/> |<span data-ttu-id="ffd7c-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ffd7c-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ffd7c-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ffd7c-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="ffd7c-145">False</span><span class="sxs-lookup"><span data-stu-id="ffd7c-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffd7c-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ffd7c-146">See also</span></span>



[<span data-ttu-id="ffd7c-147">Opération GetRooms</span><span class="sxs-lookup"><span data-stu-id="ffd7c-147">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="ffd7c-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ffd7c-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

