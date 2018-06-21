---
title: AlternateMailbox (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d913a70d-5a85-4b6e-becc-2fb9334b6088
description: L’élément AlternateMailbox représente une autre boîte aux lettres.
ms.openlocfilehash: 8eb53e4846ad55916e2c5876606c00c0f2e371ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19755251"
---
# <a name="alternatemailbox-soap"></a><span data-ttu-id="5ccde-103">AlternateMailbox (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ccde-103">AlternateMailbox (SOAP)</span></span>

<span data-ttu-id="5ccde-104">L’élément **AlternateMailbox** représente une autre boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5ccde-104">The **AlternateMailbox** element represents an alternate mailbox.</span></span> 
  
```XML
<AlternateMailbox>
   <Type/>
   <DisplayName/>
   <LegacyDN/>
   <Server/>
   <SmtpAddress/>
</AlternateMailbox>
```

 <span data-ttu-id="5ccde-105">**AlternateMailbox**</span><span class="sxs-lookup"><span data-stu-id="5ccde-105">**AlternateMailbox**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ccde-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5ccde-106">Attributes and elements</span></span>

<span data-ttu-id="5ccde-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5ccde-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ccde-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5ccde-108">Attributes</span></span>

<span data-ttu-id="5ccde-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5ccde-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ccde-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5ccde-110">Child elements</span></span>

|<span data-ttu-id="5ccde-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5ccde-111">**Element**</span></span>|<span data-ttu-id="5ccde-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ccde-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ccde-113">Type (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ccde-113">Type (SOAP)</span></span>](type-soap.md) <br/> |<span data-ttu-id="5ccde-114">Représente le type de boîte aux lettres de substitution.</span><span class="sxs-lookup"><span data-stu-id="5ccde-114">Represents the alternate mailbox type.</span></span>  <br/> |
|[<span data-ttu-id="5ccde-115">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ccde-115">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="5ccde-116">Représente le nom complet de boîte aux lettres de substitution.</span><span class="sxs-lookup"><span data-stu-id="5ccde-116">Represents the alternate mailbox display name.</span></span>  <br/> |
|[<span data-ttu-id="5ccde-117">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ccde-117">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="5ccde-118">Représente le nom unique hérité autre boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5ccde-118">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="5ccde-119">Serveur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ccde-119">Server (SOAP)</span></span>](server-soap.md) <br/> |<span data-ttu-id="5ccde-120">Représente le serveur de boîtes aux lettres de substitution.</span><span class="sxs-lookup"><span data-stu-id="5ccde-120">Represents the alternate mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="5ccde-121">SmtpAddress (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ccde-121">SmtpAddress (SOAP)</span></span>](smtpaddress-soap.md) <br/> |<span data-ttu-id="5ccde-122">Représente la boîte aux lettres autre adresse SMTP.</span><span class="sxs-lookup"><span data-stu-id="5ccde-122">Represents the alternate mailbox SMTP address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5ccde-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5ccde-123">Parent elements</span></span>

|<span data-ttu-id="5ccde-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5ccde-124">**Element**</span></span>|<span data-ttu-id="5ccde-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ccde-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ccde-126">AlternateMailboxes (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ccde-126">AlternateMailboxes (SOAP)</span></span>](alternatemailboxes-soap.md) <br/> |<span data-ttu-id="5ccde-127">Représente une collection d’autres boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5ccde-127">Represents a collection of alternate mailboxes.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5ccde-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5ccde-128">Text value</span></span>

<span data-ttu-id="5ccde-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5ccde-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ccde-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5ccde-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ccde-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5ccde-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5ccde-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5ccde-132">Schema Name</span></span>  <br/> |<span data-ttu-id="5ccde-133">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="5ccde-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5ccde-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5ccde-134">Validation File</span></span>  <br/> |<span data-ttu-id="5ccde-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5ccde-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5ccde-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5ccde-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ccde-137">True</span><span class="sxs-lookup"><span data-stu-id="5ccde-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ccde-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5ccde-138">See also</span></span>

- [<span data-ttu-id="5ccde-139">AlternateMailboxCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ccde-139">AlternateMailboxCollectionSetting (SOAP)</span></span>](alternatemailboxcollectionsetting-soap.md)

