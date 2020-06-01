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
ms.openlocfilehash: 2193e72c38c687669f6e052b4d2526029aa89d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459033"
---
# <a name="routingtype-emailaddress"></a><span data-ttu-id="7cafc-103">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="7cafc-103">RoutingType (EmailAddress)</span></span>

<span data-ttu-id="7cafc-104">L’élément **RoutingType** représente le protocole de routage pour le destinataire.</span><span class="sxs-lookup"><span data-stu-id="7cafc-104">The **RoutingType** element represents the routing protocol for the recipient.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="7cafc-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="7cafc-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7cafc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7cafc-106">Attributes and elements</span></span>

<span data-ttu-id="7cafc-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7cafc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cafc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7cafc-108">Attributes</span></span>

<span data-ttu-id="7cafc-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7cafc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7cafc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7cafc-110">Child elements</span></span>

<span data-ttu-id="7cafc-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7cafc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7cafc-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7cafc-112">Parent elements</span></span>

|<span data-ttu-id="7cafc-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7cafc-113">**Element**</span></span>|<span data-ttu-id="7cafc-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7cafc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cafc-115">E-mail (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7cafc-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="7cafc-116">Spécifie l’adresse de messagerie de l’objet MailboxData.</span><span class="sxs-lookup"><span data-stu-id="7cafc-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="7cafc-117">Cet élément est utilisé dans l' [opération GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7cafc-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/><br/> <span data-ttu-id="7cafc-118">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="7cafc-118">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="7cafc-119">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="7cafc-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="7cafc-120">Représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="7cafc-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="7cafc-121">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="7cafc-121">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7cafc-122">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="7cafc-122">Text value</span></span>

<span data-ttu-id="7cafc-123">Une valeur de texte est facultative.</span><span class="sxs-lookup"><span data-stu-id="7cafc-123">A text value is optional.</span></span> <span data-ttu-id="7cafc-124">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="7cafc-124">The following are the possible values:</span></span>

* <span data-ttu-id="7cafc-125">SMTP</span><span class="sxs-lookup"><span data-stu-id="7cafc-125">SMTP</span></span>
* <span data-ttu-id="7cafc-126">EX</span><span class="sxs-lookup"><span data-stu-id="7cafc-126">EX</span></span>

<span data-ttu-id="7cafc-127">Si aucune valeur n’est fournie, la valeur par défaut SMTP est utilisée.</span><span class="sxs-lookup"><span data-stu-id="7cafc-127">If no value is provided, the default value of SMTP is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7cafc-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="7cafc-128">Remarks</span></span>

<span data-ttu-id="7cafc-129">Cet élément peut apparaître au plus une fois dans l’élément [email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="7cafc-129">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="7cafc-130">Cet élément n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="7cafc-130">This element is not required.</span></span> <span data-ttu-id="7cafc-131">Cet élément existe pour l’inclusion des futurs protocoles.</span><span class="sxs-lookup"><span data-stu-id="7cafc-131">This element exists for the inclusion of future protocols.</span></span> <span data-ttu-id="7cafc-132">Un autre élément **RoutingType** est utilisé pour accéder aux éléments de la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7cafc-132">Another **RoutingType** element is used for accessing items in a user's mailbox.</span></span> 
  
<span data-ttu-id="7cafc-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7cafc-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7cafc-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7cafc-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cafc-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7cafc-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7cafc-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7cafc-136">Schema Name</span></span>  <br/> |<span data-ttu-id="7cafc-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7cafc-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="7cafc-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7cafc-138">Validation File</span></span>  <br/> |<span data-ttu-id="7cafc-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7cafc-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7cafc-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7cafc-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="7cafc-141">False</span><span class="sxs-lookup"><span data-stu-id="7cafc-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cafc-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7cafc-142">See also</span></span>

- [<span data-ttu-id="7cafc-143">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="7cafc-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="7cafc-144">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="7cafc-144">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="7cafc-145">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="7cafc-145">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

