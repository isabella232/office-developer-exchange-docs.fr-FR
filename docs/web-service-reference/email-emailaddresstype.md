---
title: Courrier électronique (EmailAddressType)
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
description: L’élément de courrier électronique représente l’utilisateur de boîte aux lettres pour une requête GetUserAvailability.
ms.openlocfilehash: 0e7848d7c4f5001ed86b06d11af1d7623b4bf1f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756095"
---
# <a name="email-emailaddresstype"></a><span data-ttu-id="71064-103">Courrier électronique (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="71064-103">Email (EmailAddressType)</span></span>

<span data-ttu-id="71064-104">L’élément de **courrier électronique** représente l’utilisateur de boîte aux lettres pour une requête GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="71064-104">The **Email** element represents the mailbox user for a GetUserAvailability query.</span></span> 
  
- [<span data-ttu-id="71064-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="71064-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)  
- [<span data-ttu-id="71064-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="71064-106">MailboxDataArray</span></span>](mailboxdataarray.md) 
- [<span data-ttu-id="71064-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="71064-107">MailboxData</span></span>](mailboxdata.md) 
- [<span data-ttu-id="71064-108">Courrier électronique (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="71064-108">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 <span data-ttu-id="71064-109">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="71064-109">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71064-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="71064-110">Attributes and elements</span></span>

<span data-ttu-id="71064-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="71064-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71064-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="71064-112">Attributes</span></span>

<span data-ttu-id="71064-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="71064-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71064-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="71064-114">Child elements</span></span>

|<span data-ttu-id="71064-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="71064-115">**Element**</span></span>|<span data-ttu-id="71064-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="71064-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71064-117">Nom (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="71064-117">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="71064-118">Représente le nom complet de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="71064-118">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="71064-119">Adresse (chaîne)</span><span class="sxs-lookup"><span data-stu-id="71064-119">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="71064-120">Représente l’adresse de messagerie de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="71064-120">Represents the e-mail address of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="71064-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="71064-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="71064-122">Représente le protocole de routage pour le message.</span><span class="sxs-lookup"><span data-stu-id="71064-122">Represents the routing protocol for the message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71064-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="71064-123">Parent elements</span></span>

|<span data-ttu-id="71064-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="71064-124">**Element**</span></span>|<span data-ttu-id="71064-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="71064-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71064-126">MailboxData</span><span class="sxs-lookup"><span data-stu-id="71064-126">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="71064-127">Représente un utilisateur de boîte aux lettres et les options pour le type de données à renvoyer sur l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="71064-127">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="71064-128">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="71064-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="71064-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="71064-129">Remarks</span></span>

<span data-ttu-id="71064-130">Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="71064-130">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71064-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="71064-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71064-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="71064-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71064-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="71064-133">Schema Name</span></span>  <br/> |<span data-ttu-id="71064-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="71064-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="71064-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="71064-135">Validation File</span></span>  <br/> |<span data-ttu-id="71064-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="71064-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71064-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="71064-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="71064-138">False</span><span class="sxs-lookup"><span data-stu-id="71064-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71064-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="71064-139">See also</span></span>

- [<span data-ttu-id="71064-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="71064-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="71064-141">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="71064-141">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="71064-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="71064-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

