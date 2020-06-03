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
description: L’élément MailboxData représente un utilisateur de boîte aux lettres et des options individuelles pour le type de données à renvoyer à propos de l’utilisateur de boîte aux lettres.
ms.openlocfilehash: bfcb8c01d40af81097c7d9868006fe9b7b5519d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467248"
---
# <a name="mailboxdata"></a><span data-ttu-id="e189a-103">MailboxData</span><span class="sxs-lookup"><span data-stu-id="e189a-103">MailboxData</span></span>

<span data-ttu-id="e189a-104">L’élément **MailboxData** représente un utilisateur de boîte aux lettres et des options individuelles pour le type de données à renvoyer à propos de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e189a-104">The **MailboxData** element represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span> 
  
- [<span data-ttu-id="e189a-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e189a-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="e189a-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="e189a-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="e189a-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="e189a-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

<span data-ttu-id="e189a-108">**MailboxData**</span><span class="sxs-lookup"><span data-stu-id="e189a-108">**MailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e189a-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e189a-109">Attributes and elements</span></span>

<span data-ttu-id="e189a-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e189a-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e189a-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="e189a-111">Attributes</span></span>

<span data-ttu-id="e189a-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e189a-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e189a-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e189a-113">Child elements</span></span>

|<span data-ttu-id="e189a-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e189a-114">**Element**</span></span>|<span data-ttu-id="e189a-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="e189a-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e189a-116">E-mail (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e189a-116">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="e189a-117">Représente l’utilisateur de boîte aux lettres pour une requête GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="e189a-117">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> |
|[<span data-ttu-id="e189a-118">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="e189a-118">AttendeeType</span></span>](attendeetype.md) <br/> |<span data-ttu-id="e189a-119">Représente le type de participant identifié dans l’élément [email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="e189a-119">Represents the type of attendee identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="e189a-120">Elle est utilisée dans les demandes de suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="e189a-120">This is used in requests for meeting suggestions.</span></span>  <br/> |
|[<span data-ttu-id="e189a-121">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="e189a-121">ExcludeConflicts</span></span>](excludeconflicts.md) <br/> |<span data-ttu-id="e189a-122">Spécifie s’il faut renvoyer les heures suggérées pour les heures de calendrier qui sont en conflit entre les participants.</span><span class="sxs-lookup"><span data-stu-id="e189a-122">Specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e189a-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e189a-123">Parent elements</span></span>

|<span data-ttu-id="e189a-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e189a-124">**Element**</span></span>|<span data-ttu-id="e189a-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="e189a-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e189a-126">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="e189a-126">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="e189a-127">Contient la liste des boîtes aux lettres à interroger pour obtenir des informations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="e189a-127">Contains a list of mailboxes to query for availability information.</span></span>  <br/> <span data-ttu-id="e189a-128">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="e189a-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e189a-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="e189a-129">Remarks</span></span>

<span data-ttu-id="e189a-130">Une application cliente peut définir un à plusieurs éléments **MailboxData** .</span><span class="sxs-lookup"><span data-stu-id="e189a-130">A client application can define one to many **MailboxData** elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e189a-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e189a-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="e189a-132">Exemple</span><span class="sxs-lookup"><span data-stu-id="e189a-132">Example</span></span>

```xml
<MailboxDataArray>
  <MailboxData xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="e189a-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e189a-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e189a-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e189a-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e189a-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e189a-135">Schema Name</span></span>  <br/> |<span data-ttu-id="e189a-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e189a-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="e189a-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e189a-137">Validation File</span></span>  <br/> |<span data-ttu-id="e189a-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e189a-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e189a-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e189a-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="e189a-140">False</span><span class="sxs-lookup"><span data-stu-id="e189a-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e189a-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e189a-141">See also</span></span>

- [<span data-ttu-id="e189a-142">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e189a-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="e189a-143">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e189a-143">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="e189a-144">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e189a-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

