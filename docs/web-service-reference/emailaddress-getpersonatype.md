---
title: EmailAddress (GetPersonaType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 052055b5-4630-40ed-9b24-9e7f4bf7ba1d
description: L’élément EmailAddress (GetPersonaType) spécifie l’adresse de messagerie électronique associée au personnage.
ms.openlocfilehash: b58f61202cd94ff282b21138b47b40887b38752a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463453"
---
# <a name="emailaddress-getpersonatype"></a><span data-ttu-id="34e7a-103">EmailAddress (GetPersonaType)</span><span class="sxs-lookup"><span data-stu-id="34e7a-103">EmailAddress (GetPersonaType)</span></span>

<span data-ttu-id="34e7a-104">L’élément **EmailAddress (GetPersonaType)** spécifie l’adresse de messagerie électronique associée au personnage.</span><span class="sxs-lookup"><span data-stu-id="34e7a-104">The **EmailAddress (GetPersonaType)** element specifies the email address associated with the persona.</span></span> 
  
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

 <span data-ttu-id="34e7a-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="34e7a-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34e7a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="34e7a-106">Attributes and elements</span></span>

<span data-ttu-id="34e7a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="34e7a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34e7a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="34e7a-108">Attributes</span></span>

<span data-ttu-id="34e7a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="34e7a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34e7a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="34e7a-110">Child elements</span></span>

<span data-ttu-id="34e7a-111">[Nom (chaîne)](name-string.md)  |  [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)  |  [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)  |  [MailboxType](mailboxtype.md)  |  [ItemId](itemid.md)  |  [OriginalDisplayName](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="34e7a-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34e7a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="34e7a-112">Parent elements</span></span>

[<span data-ttu-id="34e7a-113">GetPersona</span><span class="sxs-lookup"><span data-stu-id="34e7a-113">GetPersona</span></span>](getpersona.md)
  
## <a name="remarks"></a><span data-ttu-id="34e7a-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="34e7a-114">Remarks</span></span>

<span data-ttu-id="34e7a-115">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="34e7a-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="34e7a-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="34e7a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34e7a-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="34e7a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34e7a-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="34e7a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="34e7a-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="34e7a-119">Schema Name</span></span>  <br/> |<span data-ttu-id="34e7a-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="34e7a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="34e7a-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="34e7a-121">Validation File</span></span>  <br/> |<span data-ttu-id="34e7a-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="34e7a-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="34e7a-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="34e7a-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="34e7a-124">True</span><span class="sxs-lookup"><span data-stu-id="34e7a-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34e7a-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="34e7a-125">See also</span></span>

- [<span data-ttu-id="34e7a-126">GetPersona</span><span class="sxs-lookup"><span data-stu-id="34e7a-126">GetPersona</span></span>](getpersona.md)
- [<span data-ttu-id="34e7a-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="34e7a-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

