---
title: RoutingType (EmailAddress)
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
ms.assetid: 74d83198-0d9d-4c78-a2bc-9a671859ff37
description: L’élément RoutingType représente le protocole de routage pour le destinataire.
ms.openlocfilehash: a0a6cf312bcb1d4b4818a82bc8d8d3e3f33ad6f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829255"
---
# <a name="routingtype-emailaddress"></a><span data-ttu-id="91f33-103">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="91f33-103">RoutingType (EmailAddress)</span></span>

<span data-ttu-id="91f33-104">L’élément **RoutingType** représente le protocole de routage pour le destinataire.</span><span class="sxs-lookup"><span data-stu-id="91f33-104">The **RoutingType** element represents the routing protocol for the recipient.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="91f33-105">**string**</span><span class="sxs-lookup"><span data-stu-id="91f33-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91f33-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="91f33-106">Attributes and elements</span></span>

<span data-ttu-id="91f33-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="91f33-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91f33-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="91f33-108">Attributes</span></span>

<span data-ttu-id="91f33-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="91f33-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91f33-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="91f33-110">Child elements</span></span>

<span data-ttu-id="91f33-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="91f33-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91f33-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="91f33-112">Parent elements</span></span>

|<span data-ttu-id="91f33-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="91f33-113">**Element**</span></span>|<span data-ttu-id="91f33-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="91f33-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91f33-115">Courrier électronique (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="91f33-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="91f33-116">Spécifie l’adresse de messagerie de l’objet MailboxData.</span><span class="sxs-lookup"><span data-stu-id="91f33-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="91f33-117">Cet élément est utilisé dans l' [opération GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="91f33-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/><br/> <span data-ttu-id="91f33-118">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="91f33-118">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="91f33-119">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="91f33-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="91f33-120">Représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="91f33-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="91f33-121">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="91f33-121">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91f33-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="91f33-122">Text value</span></span>

<span data-ttu-id="91f33-123">Une valeur de texte est facultative.</span><span class="sxs-lookup"><span data-stu-id="91f33-123">A text value is optional.</span></span> <span data-ttu-id="91f33-124">La seule valeur valide est SMTP.</span><span class="sxs-lookup"><span data-stu-id="91f33-124">The only valid value is SMTP.</span></span> <span data-ttu-id="91f33-125">Si aucune valeur n’est fournie, la valeur par défaut du service SMTP est utilisée.</span><span class="sxs-lookup"><span data-stu-id="91f33-125">If no value is provided, the default value of SMTP is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="91f33-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="91f33-126">Remarks</span></span>

<span data-ttu-id="91f33-127">Cet élément peut se produire au maximum une seule fois dans l’élément de [courrier électronique (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="91f33-127">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="91f33-128">Cet élément n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="91f33-128">This element is not required.</span></span> <span data-ttu-id="91f33-129">Cet élément existe pour l’inclusion de protocoles à venir.</span><span class="sxs-lookup"><span data-stu-id="91f33-129">This element exists for the inclusion of future protocols.</span></span> <span data-ttu-id="91f33-130">Un autre élément **RoutingType** est utilisé pour accéder aux éléments de boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="91f33-130">Another **RoutingType** element is used for accessing items in a user's mailbox.</span></span> 
  
<span data-ttu-id="91f33-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="91f33-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91f33-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="91f33-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91f33-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="91f33-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91f33-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="91f33-134">Schema Name</span></span>  <br/> |<span data-ttu-id="91f33-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="91f33-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="91f33-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="91f33-136">Validation File</span></span>  <br/> |<span data-ttu-id="91f33-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91f33-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91f33-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="91f33-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="91f33-139">False</span><span class="sxs-lookup"><span data-stu-id="91f33-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91f33-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="91f33-140">See also</span></span>

- [<span data-ttu-id="91f33-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="91f33-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="91f33-142">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="91f33-142">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="91f33-143">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="91f33-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

