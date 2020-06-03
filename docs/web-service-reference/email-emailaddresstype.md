---
title: E-mail (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Email
api_type:
- schema
ms.assetid: dfffa1d5-2c3c-4f56-af63-5853df462e58
description: L’élément email représente l’utilisateur de boîte aux lettres d’une requête GetUserAvailability.
ms.openlocfilehash: 2ed8de9c011a385ec6c4ebd2f8d1d47304343a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459229"
---
# <a name="email-emailaddresstype"></a><span data-ttu-id="e08f8-103">E-mail (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e08f8-103">Email (EmailAddressType)</span></span>

<span data-ttu-id="e08f8-104">L’élément **email** représente l’utilisateur de boîte aux lettres d’une requête GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="e08f8-104">The **Email** element represents the mailbox user for a GetUserAvailability query.</span></span> 
  
- [<span data-ttu-id="e08f8-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e08f8-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)  
- [<span data-ttu-id="e08f8-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="e08f8-106">MailboxDataArray</span></span>](mailboxdataarray.md) 
- [<span data-ttu-id="e08f8-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="e08f8-107">MailboxData</span></span>](mailboxdata.md) 
- [<span data-ttu-id="e08f8-108">E-mail (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e08f8-108">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 <span data-ttu-id="e08f8-109">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="e08f8-109">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e08f8-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e08f8-110">Attributes and elements</span></span>

<span data-ttu-id="e08f8-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e08f8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e08f8-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="e08f8-112">Attributes</span></span>

<span data-ttu-id="e08f8-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e08f8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e08f8-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e08f8-114">Child elements</span></span>

|<span data-ttu-id="e08f8-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e08f8-115">**Element**</span></span>|<span data-ttu-id="e08f8-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="e08f8-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e08f8-117">Nom (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="e08f8-117">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="e08f8-118">Représente le nom complet de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e08f8-118">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="e08f8-119">Address (chaîne)</span><span class="sxs-lookup"><span data-stu-id="e08f8-119">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="e08f8-120">Représente l’adresse de messagerie de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e08f8-120">Represents the e-mail address of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="e08f8-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="e08f8-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="e08f8-122">Représente le protocole de routage du message.</span><span class="sxs-lookup"><span data-stu-id="e08f8-122">Represents the routing protocol for the message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e08f8-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e08f8-123">Parent elements</span></span>

|<span data-ttu-id="e08f8-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e08f8-124">**Element**</span></span>|<span data-ttu-id="e08f8-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="e08f8-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e08f8-126">MailboxData</span><span class="sxs-lookup"><span data-stu-id="e08f8-126">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="e08f8-127">Représente un utilisateur et des options de boîte aux lettres individuelle pour le type de données à renvoyer à propos de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e08f8-127">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="e08f8-128">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="e08f8-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e08f8-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="e08f8-129">Remarks</span></span>

<span data-ttu-id="e08f8-130">Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur exécutant MicrosoftExchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e08f8-130">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e08f8-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e08f8-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e08f8-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e08f8-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e08f8-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e08f8-133">Schema Name</span></span>  <br/> |<span data-ttu-id="e08f8-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e08f8-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="e08f8-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e08f8-135">Validation File</span></span>  <br/> |<span data-ttu-id="e08f8-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e08f8-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e08f8-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e08f8-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="e08f8-138">False</span><span class="sxs-lookup"><span data-stu-id="e08f8-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e08f8-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e08f8-139">See also</span></span>

- [<span data-ttu-id="e08f8-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e08f8-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="e08f8-141">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e08f8-141">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="e08f8-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e08f8-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

