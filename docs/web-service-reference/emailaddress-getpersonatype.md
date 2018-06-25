---
title: EmailAddress (GetPersonaType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 052055b5-4630-40ed-9b24-9e7f4bf7ba1d
description: L’élément EmailAddress (GetPersonaType) spécifie l’adresse de messagerie associée personnage.
ms.openlocfilehash: a28a4a61a9719875fe99e1c950bcd3ec3af9ab13
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756101"
---
# <a name="emailaddress-getpersonatype"></a><span data-ttu-id="735ac-103">EmailAddress (GetPersonaType)</span><span class="sxs-lookup"><span data-stu-id="735ac-103">EmailAddress (GetPersonaType)</span></span>

<span data-ttu-id="735ac-104">L’élément **EmailAddress (GetPersonaType)** Spécifie l’adresse de messagerie associée personnage.</span><span class="sxs-lookup"><span data-stu-id="735ac-104">The **EmailAddress (GetPersonaType)** element specifies the email address associated with the persona.</span></span> 
  
```XML
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
    <OriginalDisplayName></OriginalDisplayName>
</EmailAddress>>
```

 <span data-ttu-id="735ac-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="735ac-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="735ac-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="735ac-106">Attributes and elements</span></span>

<span data-ttu-id="735ac-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="735ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="735ac-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="735ac-108">Attributes</span></span>

<span data-ttu-id="735ac-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="735ac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="735ac-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="735ac-110">Child elements</span></span>

<span data-ttu-id="735ac-111">[Name (chaîne)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="735ac-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="735ac-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="735ac-112">Parent elements</span></span>

[<span data-ttu-id="735ac-113">GetPersona</span><span class="sxs-lookup"><span data-stu-id="735ac-113">GetPersona</span></span>](getpersona.md)
  
## <a name="remarks"></a><span data-ttu-id="735ac-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="735ac-114">Remarks</span></span>

<span data-ttu-id="735ac-115">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="735ac-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="735ac-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ac-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="735ac-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="735ac-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="735ac-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="735ac-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="735ac-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="735ac-119">Schema Name</span></span>  <br/> |<span data-ttu-id="735ac-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="735ac-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="735ac-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="735ac-121">Validation File</span></span>  <br/> |<span data-ttu-id="735ac-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="735ac-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="735ac-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="735ac-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="735ac-124">True</span><span class="sxs-lookup"><span data-stu-id="735ac-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="735ac-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="735ac-125">See also</span></span>

- [<span data-ttu-id="735ac-126">GetPersona</span><span class="sxs-lookup"><span data-stu-id="735ac-126">GetPersona</span></span>](getpersona.md)
- [<span data-ttu-id="735ac-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="735ac-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

