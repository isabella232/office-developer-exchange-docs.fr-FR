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
ms.openlocfilehash: d4229f2857a5c99cc9bb7ff9b9b103de099a0055
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465085"
---
# <a name="routingtype-emailaddresstype"></a><span data-ttu-id="22f09-103">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="22f09-103">RoutingType (EmailAddressType)</span></span>

<span data-ttu-id="22f09-104">L’élément **RoutingType** définit le type d’adresse pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="22f09-104">The **RoutingType** element defines the address type for the mailbox.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="22f09-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="22f09-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22f09-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="22f09-106">Attributes and elements</span></span>

<span data-ttu-id="22f09-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="22f09-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22f09-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="22f09-108">Attributes</span></span>

<span data-ttu-id="22f09-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="22f09-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22f09-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="22f09-110">Child elements</span></span>

<span data-ttu-id="22f09-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="22f09-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="22f09-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="22f09-112">Parent elements</span></span>

|<span data-ttu-id="22f09-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22f09-113">**Element**</span></span>|<span data-ttu-id="22f09-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="22f09-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22f09-115">Actionas</span><span class="sxs-lookup"><span data-stu-id="22f09-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="22f09-116">Identifie les personnes qui envoient l’appelant.</span><span class="sxs-lookup"><span data-stu-id="22f09-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="22f09-117">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="22f09-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="22f09-118">Identifie une adresse de messagerie entièrement résolue.</span><span class="sxs-lookup"><span data-stu-id="22f09-118">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="22f09-119">RoomList</span><span class="sxs-lookup"><span data-stu-id="22f09-119">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="22f09-120">Identifie une liste de salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="22f09-120">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="22f09-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="22f09-121">Text value</span></span>

<span data-ttu-id="22f09-122">La valeur texte représente un type de routage.</span><span class="sxs-lookup"><span data-stu-id="22f09-122">The text value represents a routing type.</span></span> <span data-ttu-id="22f09-123">SMTP est la valeur de texte standard de cet élément.</span><span class="sxs-lookup"><span data-stu-id="22f09-123">SMTP is the typical text value for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="22f09-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="22f09-124">Remarks</span></span>

<span data-ttu-id="22f09-125">Cet élément est facultatif dans l’élément [Mailbox](mailbox.md) .</span><span class="sxs-lookup"><span data-stu-id="22f09-125">This element is optional in the [Mailbox](mailbox.md) element.</span></span> <span data-ttu-id="22f09-126">Un autre élément [RoutingType (EmailAddress)](routingtype-emailaddress.md) est utilisé pour les opérations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="22f09-126">Another [RoutingType (EmailAddress)](routingtype-emailaddress.md) element is used for Availability operations.</span></span> 
  
<span data-ttu-id="22f09-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="22f09-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22f09-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="22f09-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22f09-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="22f09-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22f09-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="22f09-130">Schema Name</span></span>  <br/> |<span data-ttu-id="22f09-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="22f09-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="22f09-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="22f09-132">Validation File</span></span>  <br/> |<span data-ttu-id="22f09-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="22f09-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="22f09-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="22f09-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="22f09-135">False</span><span class="sxs-lookup"><span data-stu-id="22f09-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22f09-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="22f09-136">See also</span></span>



- [<span data-ttu-id="22f09-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="22f09-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

