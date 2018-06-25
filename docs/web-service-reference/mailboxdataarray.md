---
title: MailboxDataArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxDataArray
api_type:
- schema
ms.assetid: a14af788-beee-452c-b5d0-37bcb4ef02ff
description: L’élément MailboxDataArray contient une liste des boîtes aux lettres pour interroger des informations de disponibilité.
ms.openlocfilehash: b76e71ee9127dc2221e0065a27d3c781f8b5786a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828283"
---
# <a name="mailboxdataarray"></a><span data-ttu-id="04443-103">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="04443-103">MailboxDataArray</span></span>

<span data-ttu-id="04443-104">L’élément **MailboxDataArray** contient une liste des boîtes aux lettres pour interroger des informations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="04443-104">The **MailboxDataArray** element contains a list of mailboxes to query for availability information.</span></span> 
  
- [<span data-ttu-id="04443-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="04443-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="04443-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="04443-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="04443-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="04443-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxDataArray>
   <MailboxData>...</MailboxData>
</MailboxDataArray>
```

<span data-ttu-id="04443-108">**ArrayOfMailboxData**</span><span class="sxs-lookup"><span data-stu-id="04443-108">**ArrayOfMailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="04443-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="04443-109">Attributes and elements</span></span>

<span data-ttu-id="04443-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="04443-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04443-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="04443-111">Attributes</span></span>

<span data-ttu-id="04443-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="04443-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04443-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="04443-113">Child elements</span></span>

|<span data-ttu-id="04443-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04443-114">**Element**</span></span>|<span data-ttu-id="04443-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="04443-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04443-116">MailboxData</span><span class="sxs-lookup"><span data-stu-id="04443-116">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="04443-117">Représente un utilisateur de boîte aux lettres et les options pour le type de données à renvoyer sur l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="04443-117">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04443-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="04443-118">Parent elements</span></span>

|<span data-ttu-id="04443-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04443-119">**Element**</span></span>|<span data-ttu-id="04443-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="04443-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04443-121">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="04443-121">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="04443-122">Contient les arguments utilisés pour obtenir des informations de disponibilité d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="04443-122">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="04443-123">Il s’agit d’un élément racine.</span><span class="sxs-lookup"><span data-stu-id="04443-123">This is a root element.</span></span>  <br/> <span data-ttu-id="04443-124">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="04443-124">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="04443-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="04443-125">Remarks</span></span>

<span data-ttu-id="04443-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft® Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="04443-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04443-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="04443-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04443-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="04443-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="04443-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="04443-129">Schema Name</span></span>  <br/> |<span data-ttu-id="04443-130">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="04443-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="04443-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="04443-131">Validation File</span></span>  <br/> |<span data-ttu-id="04443-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="04443-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="04443-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="04443-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="04443-134">False</span><span class="sxs-lookup"><span data-stu-id="04443-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04443-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="04443-135">See also</span></span>

- [<span data-ttu-id="04443-136">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="04443-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="04443-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="04443-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="04443-138">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="04443-138">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

