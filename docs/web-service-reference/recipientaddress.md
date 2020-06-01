---
title: RecipientAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientAddress
api_type:
- schema
ms.assetid: 9ae6351a-2c60-4715-a489-5681a13641f9
description: L’élément Destinatairel’adresse représente la boîte aux lettres du destinataire.
ms.openlocfilehash: f4b6edd034dd91471e6496f6b0cca65bd3ffb69a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465848"
---
# <a name="recipientaddress"></a><span data-ttu-id="aa938-103">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="aa938-103">RecipientAddress</span></span>

<span data-ttu-id="aa938-104">L’élément **destinatairel’adresse** représente la boîte aux lettres du destinataire.</span><span class="sxs-lookup"><span data-stu-id="aa938-104">The **RecipientAddress** element represents the mailbox of the recipient.</span></span> 
  
```xml
<RecipientAddress>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientAddress>
```

 <span data-ttu-id="aa938-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="aa938-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa938-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aa938-106">Attributes and elements</span></span>

<span data-ttu-id="aa938-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aa938-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa938-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="aa938-108">Attributes</span></span>

<span data-ttu-id="aa938-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="aa938-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa938-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aa938-110">Child elements</span></span>

|<span data-ttu-id="aa938-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aa938-111">**Element**</span></span>|<span data-ttu-id="aa938-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="aa938-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa938-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="aa938-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="aa938-114">Représente le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="aa938-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="aa938-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="aa938-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="aa938-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="aa938-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="aa938-117">Définit l’adresse SMTP (Simple Mail Transfer Protocol) d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="aa938-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="aa938-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="aa938-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="aa938-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="aa938-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="aa938-120">Représente le protocole de routage pour le destinataire.</span><span class="sxs-lookup"><span data-stu-id="aa938-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="aa938-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="aa938-121">The default is SMTP.</span></span> <span data-ttu-id="aa938-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="aa938-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="aa938-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="aa938-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="aa938-124">Représente le type de boîte aux lettres représenté par l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="aa938-124">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="aa938-125">ItemId</span><span class="sxs-lookup"><span data-stu-id="aa938-125">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="aa938-126">Définit l’identificateur d’élément d’une liste de distribution privée ou de contact pour les destinataires à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="aa938-126">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="aa938-127">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="aa938-127">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa938-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aa938-128">Parent elements</span></span>

|<span data-ttu-id="aa938-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aa938-129">**Element**</span></span>|<span data-ttu-id="aa938-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="aa938-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa938-131">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="aa938-131">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="aa938-132">Représente les valeurs de différents types de conseils de courrier.</span><span class="sxs-lookup"><span data-stu-id="aa938-132">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aa938-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="aa938-133">Remarks</span></span>

<span data-ttu-id="aa938-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa938-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa938-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aa938-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa938-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aa938-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aa938-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aa938-137">Schema Name</span></span>  <br/> |<span data-ttu-id="aa938-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="aa938-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="aa938-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="aa938-139">Validation File</span></span>  <br/> |<span data-ttu-id="aa938-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aa938-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aa938-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aa938-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa938-142">False</span><span class="sxs-lookup"><span data-stu-id="aa938-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa938-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aa938-143">See also</span></span>



- [<span data-ttu-id="aa938-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="aa938-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

