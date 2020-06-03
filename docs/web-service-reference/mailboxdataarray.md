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
description: L’élément MailboxDataArray contient la liste des boîtes aux lettres dans lesquelles Rechercher les informations de disponibilité.
ms.openlocfilehash: 894bf97a0d633d7eef0434331ccf1580fcba386e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468193"
---
# <a name="mailboxdataarray"></a><span data-ttu-id="4df31-103">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="4df31-103">MailboxDataArray</span></span>

<span data-ttu-id="4df31-104">L’élément **MailboxDataArray** contient la liste des boîtes aux lettres dans lesquelles Rechercher les informations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="4df31-104">The **MailboxDataArray** element contains a list of mailboxes to query for availability information.</span></span> 
  
- [<span data-ttu-id="4df31-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="4df31-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="4df31-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="4df31-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="4df31-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="4df31-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxDataArray>
   <MailboxData>...</MailboxData>
</MailboxDataArray>
```

<span data-ttu-id="4df31-108">**ArrayOfMailboxData**</span><span class="sxs-lookup"><span data-stu-id="4df31-108">**ArrayOfMailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4df31-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4df31-109">Attributes and elements</span></span>

<span data-ttu-id="4df31-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4df31-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4df31-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="4df31-111">Attributes</span></span>

<span data-ttu-id="4df31-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4df31-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4df31-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4df31-113">Child elements</span></span>

|<span data-ttu-id="4df31-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4df31-114">**Element**</span></span>|<span data-ttu-id="4df31-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="4df31-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4df31-116">MailboxData</span><span class="sxs-lookup"><span data-stu-id="4df31-116">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="4df31-117">Représente un utilisateur et des options de boîte aux lettres individuelle pour le type de données à renvoyer à propos de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4df31-117">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4df31-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4df31-118">Parent elements</span></span>

|<span data-ttu-id="4df31-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4df31-119">**Element**</span></span>|<span data-ttu-id="4df31-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="4df31-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4df31-121">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="4df31-121">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="4df31-122">Contient les arguments utilisés pour obtenir les informations de disponibilité de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="4df31-122">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="4df31-123">Il s’agit d’un élément racine.</span><span class="sxs-lookup"><span data-stu-id="4df31-123">This is a root element.</span></span>  <br/> <span data-ttu-id="4df31-124">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="4df31-124">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4df31-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="4df31-125">Remarks</span></span>

<span data-ttu-id="4df31-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft® Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4df31-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4df31-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4df31-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4df31-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4df31-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4df31-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4df31-129">Schema Name</span></span>  <br/> |<span data-ttu-id="4df31-130">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4df31-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4df31-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4df31-131">Validation File</span></span>  <br/> |<span data-ttu-id="4df31-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4df31-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4df31-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4df31-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="4df31-134">False</span><span class="sxs-lookup"><span data-stu-id="4df31-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4df31-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4df31-135">See also</span></span>

- [<span data-ttu-id="4df31-136">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4df31-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="4df31-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="4df31-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="4df31-138">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="4df31-138">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

