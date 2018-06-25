---
title: Adresse (chaîne)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: a3cdfcbd-d0c5-46d6-8daa-52405fc63ff0
description: L’élément adresse représente l’adresse de messagerie de l’utilisateur de boîte aux lettres.
ms.openlocfilehash: 07c634d6166d88a8912bc66081a13671e600c801
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755183"
---
# <a name="address-string"></a><span data-ttu-id="cf621-103">Adresse (chaîne)</span><span class="sxs-lookup"><span data-stu-id="cf621-103">Address (string)</span></span>

<span data-ttu-id="cf621-104">L’élément **adresse** représente l’adresse de messagerie de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cf621-104">The **Address** element represents the e-mail address of the mailbox user.</span></span> 
  
```xml
<Address>...</Address>
```

 <span data-ttu-id="cf621-105">**string**</span><span class="sxs-lookup"><span data-stu-id="cf621-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf621-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cf621-106">Attributes and elements</span></span>

<span data-ttu-id="cf621-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cf621-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf621-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cf621-108">Attributes</span></span>

<span data-ttu-id="cf621-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cf621-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf621-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cf621-110">Child elements</span></span>

<span data-ttu-id="cf621-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cf621-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf621-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cf621-112">Parent elements</span></span>

|<span data-ttu-id="cf621-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cf621-113">**Element**</span></span>|<span data-ttu-id="cf621-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf621-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf621-115">Courrier électronique (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="cf621-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="cf621-116">Spécifie l’adresse de messagerie de l’objet MailboxData.</span><span class="sxs-lookup"><span data-stu-id="cf621-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="cf621-117">Cet élément est utilisé dans l' [opération GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="cf621-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span><br/><br/> <span data-ttu-id="cf621-118">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="cf621-118">The following is the XPath to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="cf621-119">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="cf621-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="cf621-120">Représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="cf621-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span><br/><br/>  <span data-ttu-id="cf621-121">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="cf621-121">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf621-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="cf621-122">Text value</span></span>

<span data-ttu-id="cf621-123">Une valeur de texte est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="cf621-123">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cf621-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="cf621-124">Remarks</span></span>

<span data-ttu-id="cf621-125">Cet élément peut se produire au maximum une seule fois dans l’élément de [courrier électronique (EmailAddressType)](email-emailaddresstype.md) et l’élément de [boîte aux lettres (disponibilité)](mailbox-availability.md) .</span><span class="sxs-lookup"><span data-stu-id="cf621-125">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element and the [Mailbox (Availability)](mailbox-availability.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="cf621-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="cf621-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="cf621-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cf621-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf621-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cf621-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf621-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cf621-129">Schema Name</span></span>  <br/> |<span data-ttu-id="cf621-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cf621-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf621-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cf621-131">Validation File</span></span>  <br/> |<span data-ttu-id="cf621-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cf621-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf621-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cf621-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf621-134">False</span><span class="sxs-lookup"><span data-stu-id="cf621-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf621-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cf621-135">See also</span></span>

- [<span data-ttu-id="cf621-136">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="cf621-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="cf621-137">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="cf621-137">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="cf621-138">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="cf621-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="cf621-139">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="cf621-139">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="cf621-140">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="cf621-140">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
- [<span data-ttu-id="cf621-141">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="cf621-141">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
- [<span data-ttu-id="cf621-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="cf621-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

