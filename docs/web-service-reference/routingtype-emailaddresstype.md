---
title: RoutingType (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 683216be-9972-4f48-a148-c34bfe7f53e5
description: L’élément RoutingType définit le type d’adresse pour la boîte aux lettres.
ms.openlocfilehash: a02c3b5711a657311428d67cccabd9c8c231db67
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829256"
---
# <a name="routingtype-emailaddresstype"></a><span data-ttu-id="11678-103">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="11678-103">RoutingType (EmailAddressType)</span></span>

<span data-ttu-id="11678-104">L’élément **RoutingType** définit le type d’adresse pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="11678-104">The **RoutingType** element defines the address type for the mailbox.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="11678-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="11678-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11678-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="11678-106">Attributes and elements</span></span>

<span data-ttu-id="11678-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="11678-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11678-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="11678-108">Attributes</span></span>

<span data-ttu-id="11678-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="11678-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11678-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="11678-110">Child elements</span></span>

<span data-ttu-id="11678-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="11678-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="11678-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="11678-112">Parent elements</span></span>

|<span data-ttu-id="11678-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="11678-113">**Element**</span></span>|<span data-ttu-id="11678-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="11678-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11678-115">ActingAs</span><span class="sxs-lookup"><span data-stu-id="11678-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="11678-116">Identifie les personnes envoie par l’appelant.</span><span class="sxs-lookup"><span data-stu-id="11678-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="11678-117">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="11678-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="11678-118">Identifie une adresse de messagerie entièrement résolu.</span><span class="sxs-lookup"><span data-stu-id="11678-118">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="11678-119">RoomList</span><span class="sxs-lookup"><span data-stu-id="11678-119">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="11678-120">Identifie une liste de salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="11678-120">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="11678-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="11678-121">Text value</span></span>

<span data-ttu-id="11678-122">La valeur de texte représente un type de routage.</span><span class="sxs-lookup"><span data-stu-id="11678-122">The text value represents a routing type.</span></span> <span data-ttu-id="11678-123">SMTP est la valeur de type texte pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="11678-123">SMTP is the typical text value for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="11678-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="11678-124">Remarks</span></span>

<span data-ttu-id="11678-125">Cet élément est facultatif dans l’élément de [boîte aux lettres](mailbox.md) .</span><span class="sxs-lookup"><span data-stu-id="11678-125">This element is optional in the [Mailbox](mailbox.md) element.</span></span> <span data-ttu-id="11678-126">Un autre élément [RoutingType (EmailAddress)](routingtype-emailaddress.md) est utilisé pour les opérations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="11678-126">Another [RoutingType (EmailAddress)](routingtype-emailaddress.md) element is used for Availability operations.</span></span> 
  
<span data-ttu-id="11678-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="11678-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11678-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="11678-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11678-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="11678-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="11678-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="11678-130">Schema Name</span></span>  <br/> |<span data-ttu-id="11678-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="11678-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="11678-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="11678-132">Validation File</span></span>  <br/> |<span data-ttu-id="11678-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="11678-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="11678-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="11678-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="11678-135">False</span><span class="sxs-lookup"><span data-stu-id="11678-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11678-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="11678-136">See also</span></span>



- [<span data-ttu-id="11678-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="11678-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

