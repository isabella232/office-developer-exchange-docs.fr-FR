---
title: Nom (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: c719c55f-d625-4e64-846f-50ac91881443
description: L’élément Name représente le nom complet de l’utilisateur de boîte aux lettres.
ms.openlocfilehash: 2c6b29f1b069f9cc72ac84e7aebfff99437e630a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466954"
---
# <a name="name-emailaddress"></a><span data-ttu-id="828ca-103">Nom (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="828ca-103">Name (EmailAddress)</span></span>

<span data-ttu-id="828ca-104">L’élément **Name** représente le nom complet de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="828ca-104">The **Name** element represents the display name of the mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="828ca-105">**String**</span><span class="sxs-lookup"><span data-stu-id="828ca-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="828ca-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="828ca-106">Attributes and elements</span></span>

<span data-ttu-id="828ca-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="828ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="828ca-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="828ca-108">Attributes</span></span>

<span data-ttu-id="828ca-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="828ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="828ca-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="828ca-110">Child elements</span></span>

<span data-ttu-id="828ca-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="828ca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="828ca-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="828ca-112">Parent elements</span></span>

|<span data-ttu-id="828ca-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="828ca-113">**Element**</span></span>|<span data-ttu-id="828ca-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="828ca-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="828ca-115">E-mail (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="828ca-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="828ca-116">Représente l’utilisateur de boîte aux lettres pour une requête GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="828ca-116">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> <br/><span data-ttu-id="828ca-117">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="828ca-117">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="828ca-118">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="828ca-118">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="828ca-119">Représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="828ca-119">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="828ca-120">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="828ca-120">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="828ca-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="828ca-121">Text value</span></span>

<span data-ttu-id="828ca-122">Une valeur de texte est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="828ca-122">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="828ca-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="828ca-123">Remarks</span></span>

<span data-ttu-id="828ca-124">Cet élément peut apparaître au plus une fois dans l’élément [email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="828ca-124">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="828ca-125">Cet élément n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="828ca-125">This element is not required.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="828ca-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="828ca-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="828ca-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="828ca-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="828ca-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="828ca-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="828ca-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="828ca-129">Schema Name</span></span>  <br/> |<span data-ttu-id="828ca-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="828ca-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="828ca-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="828ca-131">Validation File</span></span>  <br/> |<span data-ttu-id="828ca-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="828ca-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="828ca-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="828ca-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="828ca-134">False</span><span class="sxs-lookup"><span data-stu-id="828ca-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="828ca-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="828ca-135">See also</span></span>

- [<span data-ttu-id="828ca-136">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="828ca-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="828ca-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="828ca-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="828ca-138">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="828ca-138">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

