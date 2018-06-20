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
description: L’élément RecipientAddress représente la boîte aux lettres du destinataire.
ms.openlocfilehash: 10928ac206227cfc21bd83ab5bfa9a55aad354e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828974"
---
# <a name="recipientaddress"></a><span data-ttu-id="8b72d-103">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="8b72d-103">RecipientAddress</span></span>

<span data-ttu-id="8b72d-104">L’élément **RecipientAddress** représente la boîte aux lettres du destinataire.</span><span class="sxs-lookup"><span data-stu-id="8b72d-104">The **RecipientAddress** element represents the mailbox of the recipient.</span></span> 
  
```xml
<RecipientAddress>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientAddress>
```

 <span data-ttu-id="8b72d-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="8b72d-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b72d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8b72d-106">Attributes and elements</span></span>

<span data-ttu-id="8b72d-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8b72d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b72d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8b72d-108">Attributes</span></span>

<span data-ttu-id="8b72d-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8b72d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b72d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8b72d-110">Child elements</span></span>

|<span data-ttu-id="8b72d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8b72d-111">**Element**</span></span>|<span data-ttu-id="8b72d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8b72d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b72d-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8b72d-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="8b72d-114">Représente le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8b72d-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="8b72d-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="8b72d-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8b72d-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="8b72d-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="8b72d-117">Définit l’adresse SMTP Simple Mail Transfer Protocol () d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8b72d-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="8b72d-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="8b72d-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8b72d-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="8b72d-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="8b72d-120">Représente le protocole de routage pour le destinataire.</span><span class="sxs-lookup"><span data-stu-id="8b72d-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="8b72d-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="8b72d-121">The default is SMTP.</span></span> <span data-ttu-id="8b72d-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="8b72d-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8b72d-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="8b72d-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="8b72d-124">Représente le type de boîte aux lettres qui est représenté par l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="8b72d-124">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="8b72d-125">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="8b72d-125">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="8b72d-126">Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8b72d-126">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="8b72d-127">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="8b72d-127">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8b72d-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8b72d-128">Parent elements</span></span>

|<span data-ttu-id="8b72d-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8b72d-129">**Element**</span></span>|<span data-ttu-id="8b72d-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="8b72d-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b72d-131">Les infos-courrier</span><span class="sxs-lookup"><span data-stu-id="8b72d-131">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="8b72d-132">Représente les valeurs pour les différents types d’astuces de la messagerie.</span><span class="sxs-lookup"><span data-stu-id="8b72d-132">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8b72d-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="8b72d-133">Remarks</span></span>

<span data-ttu-id="8b72d-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b72d-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b72d-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8b72d-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b72d-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8b72d-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b72d-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8b72d-137">Schema Name</span></span>  <br/> |<span data-ttu-id="8b72d-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8b72d-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b72d-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8b72d-139">Validation File</span></span>  <br/> |<span data-ttu-id="8b72d-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8b72d-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b72d-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8b72d-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b72d-142">False</span><span class="sxs-lookup"><span data-stu-id="8b72d-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b72d-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8b72d-143">See also</span></span>



- [<span data-ttu-id="8b72d-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8b72d-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

