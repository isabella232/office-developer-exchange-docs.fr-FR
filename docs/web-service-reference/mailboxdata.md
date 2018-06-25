---
title: MailboxData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxData
api_type:
- schema
ms.assetid: e9e3f50c-5a7b-49c7-a9ea-117959c08352
description: L’élément MailboxData représente un utilisateur de boîte aux lettres et les options pour le type de données à renvoyer sur l’utilisateur de boîte aux lettres.
ms.openlocfilehash: df60294e7d83b1459e5cca7d75c2b6b4bb9d931d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828281"
---
# <a name="mailboxdata"></a><span data-ttu-id="320e1-103">MailboxData</span><span class="sxs-lookup"><span data-stu-id="320e1-103">MailboxData</span></span>

<span data-ttu-id="320e1-104">L’élément **MailboxData** représente un utilisateur de boîte aux lettres et les options pour le type de données à renvoyer sur l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="320e1-104">The **MailboxData** element represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span> 
  
- [<span data-ttu-id="320e1-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="320e1-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="320e1-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="320e1-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="320e1-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="320e1-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

<span data-ttu-id="320e1-108">**MailboxData**</span><span class="sxs-lookup"><span data-stu-id="320e1-108">**MailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="320e1-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="320e1-109">Attributes and elements</span></span>

<span data-ttu-id="320e1-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="320e1-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="320e1-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="320e1-111">Attributes</span></span>

<span data-ttu-id="320e1-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="320e1-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="320e1-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="320e1-113">Child elements</span></span>

|<span data-ttu-id="320e1-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="320e1-114">**Element**</span></span>|<span data-ttu-id="320e1-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="320e1-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="320e1-116">Courrier électronique (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="320e1-116">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="320e1-117">Représente l’utilisateur de boîte aux lettres pour une requête GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="320e1-117">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> |
|[<span data-ttu-id="320e1-118">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="320e1-118">AttendeeType</span></span>](attendeetype.md) <br/> |<span data-ttu-id="320e1-119">Représente le type de participant identifié dans l’élément de [courrier électronique (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="320e1-119">Represents the type of attendee identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="320e1-120">Il est utilisé dans les requêtes de suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="320e1-120">This is used in requests for meeting suggestions.</span></span>  <br/> |
|[<span data-ttu-id="320e1-121">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="320e1-121">ExcludeConflicts</span></span>](excludeconflicts.md) <br/> |<span data-ttu-id="320e1-122">Spécifie s’il faut renvoyer suggérées heures de temps de calendrier en conflit entre les participants.</span><span class="sxs-lookup"><span data-stu-id="320e1-122">Specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="320e1-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="320e1-123">Parent elements</span></span>

|<span data-ttu-id="320e1-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="320e1-124">**Element**</span></span>|<span data-ttu-id="320e1-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="320e1-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="320e1-126">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="320e1-126">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="320e1-127">Contient une liste des boîtes aux lettres pour interroger des informations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="320e1-127">Contains a list of mailboxes to query for availability information.</span></span>  <br/> <span data-ttu-id="320e1-128">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="320e1-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="320e1-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="320e1-129">Remarks</span></span>

<span data-ttu-id="320e1-130">Une application cliente peut en définir une à de nombreux éléments **MailboxData** .</span><span class="sxs-lookup"><span data-stu-id="320e1-130">A client application can define one to many **MailboxData** elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="320e1-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="320e1-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="320e1-132">Exemple</span><span class="sxs-lookup"><span data-stu-id="320e1-132">Example</span></span>

```xml
<MailboxDataArray>
  <MailboxData xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
    <Email>
      <Name></Name>
      <Address>someone@ExServer.example.com</Address>
      <RoutingType>SMTP</RoutingType>
    </Email>
    <AttendeeType>Organizer</AttendeeType>
    <ExcludeConflicts>false</ExcludeConflicts>
  </MailboxData>
</MailboxDataArray>
```

## <a name="element-information"></a><span data-ttu-id="320e1-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="320e1-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="320e1-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="320e1-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="320e1-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="320e1-135">Schema Name</span></span>  <br/> |<span data-ttu-id="320e1-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="320e1-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="320e1-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="320e1-137">Validation File</span></span>  <br/> |<span data-ttu-id="320e1-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="320e1-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="320e1-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="320e1-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="320e1-140">False</span><span class="sxs-lookup"><span data-stu-id="320e1-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="320e1-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="320e1-141">See also</span></span>

- [<span data-ttu-id="320e1-142">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="320e1-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="320e1-143">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="320e1-143">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="320e1-144">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="320e1-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

