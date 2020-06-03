---
title: Address (chaîne)
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
description: L’élément Address représente l’adresse de messagerie de l’utilisateur de boîte aux lettres.
ms.openlocfilehash: 839107050f22df5c00cb4dea9c531563df52933d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463642"
---
# <a name="address-string"></a><span data-ttu-id="18994-103">Address (chaîne)</span><span class="sxs-lookup"><span data-stu-id="18994-103">Address (string)</span></span>

<span data-ttu-id="18994-104">L’élément **Address** représente l’adresse de messagerie de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="18994-104">The **Address** element represents the e-mail address of the mailbox user.</span></span> 
  
```xml
<Address>...</Address>
```

 <span data-ttu-id="18994-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="18994-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18994-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="18994-106">Attributes and elements</span></span>

<span data-ttu-id="18994-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="18994-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18994-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="18994-108">Attributes</span></span>

<span data-ttu-id="18994-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="18994-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18994-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="18994-110">Child elements</span></span>

<span data-ttu-id="18994-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="18994-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18994-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="18994-112">Parent elements</span></span>

|<span data-ttu-id="18994-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="18994-113">**Element**</span></span>|<span data-ttu-id="18994-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="18994-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18994-115">E-mail (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="18994-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="18994-116">Spécifie l’adresse de messagerie de l’objet MailboxData.</span><span class="sxs-lookup"><span data-stu-id="18994-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="18994-117">Cet élément est utilisé dans l' [opération GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="18994-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span><br/><br/> <span data-ttu-id="18994-118">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="18994-118">The following is the XPath to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="18994-119">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="18994-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="18994-120">Représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="18994-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span><br/><br/>  <span data-ttu-id="18994-121">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="18994-121">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18994-122">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="18994-122">Text value</span></span>

<span data-ttu-id="18994-123">Une valeur de texte est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="18994-123">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="18994-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="18994-124">Remarks</span></span>

<span data-ttu-id="18994-125">Cet élément peut apparaître au plus une fois dans l’élément [email (EmailAddressType)](email-emailaddresstype.md) et l’élément [Mailbox (Availability)](mailbox-availability.md) .</span><span class="sxs-lookup"><span data-stu-id="18994-125">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element and the [Mailbox (Availability)](mailbox-availability.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="18994-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="18994-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="18994-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="18994-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18994-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="18994-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18994-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="18994-129">Schema Name</span></span>  <br/> |<span data-ttu-id="18994-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="18994-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="18994-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="18994-131">Validation File</span></span>  <br/> |<span data-ttu-id="18994-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="18994-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18994-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="18994-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="18994-134">False</span><span class="sxs-lookup"><span data-stu-id="18994-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18994-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="18994-135">See also</span></span>

- [<span data-ttu-id="18994-136">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="18994-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="18994-137">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="18994-137">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="18994-138">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="18994-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="18994-139">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="18994-139">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="18994-140">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="18994-140">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
- [<span data-ttu-id="18994-141">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="18994-141">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
- [<span data-ttu-id="18994-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="18994-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

