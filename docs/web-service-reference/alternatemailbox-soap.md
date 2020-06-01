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
description: L’élément AlternateMailbox représente une boîte aux lettres de substitution.
ms.openlocfilehash: 9019f85a373cc186cc9dadddceee3dc9d11b3854
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466156"
---
# <a name="alternatemailbox-soap"></a><span data-ttu-id="bb501-103">AlternateMailbox (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb501-103">AlternateMailbox (SOAP)</span></span>

<span data-ttu-id="bb501-104">L’élément **AlternateMailbox** représente une boîte aux lettres de substitution.</span><span class="sxs-lookup"><span data-stu-id="bb501-104">The **AlternateMailbox** element represents an alternate mailbox.</span></span> 
  
```XML
<AlternateMailbox>
   <Type/>
   <DisplayName/>
   <LegacyDN/>
   <Server/>
   <SmtpAddress/>
</AlternateMailbox>
```

 <span data-ttu-id="bb501-105">**AlternateMailbox**</span><span class="sxs-lookup"><span data-stu-id="bb501-105">**AlternateMailbox**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb501-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bb501-106">Attributes and elements</span></span>

<span data-ttu-id="bb501-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bb501-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb501-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bb501-108">Attributes</span></span>

<span data-ttu-id="bb501-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bb501-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb501-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bb501-110">Child elements</span></span>

|<span data-ttu-id="bb501-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bb501-111">**Element**</span></span>|<span data-ttu-id="bb501-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="bb501-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb501-113">Type (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb501-113">Type (SOAP)</span></span>](type-soap.md) <br/> |<span data-ttu-id="bb501-114">Représente le type de boîte aux lettres de substitution.</span><span class="sxs-lookup"><span data-stu-id="bb501-114">Represents the alternate mailbox type.</span></span>  <br/> |
|[<span data-ttu-id="bb501-115">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb501-115">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="bb501-116">Représente le nom d’affichage de la boîte aux lettres de remplacement.</span><span class="sxs-lookup"><span data-stu-id="bb501-116">Represents the alternate mailbox display name.</span></span>  <br/> |
|[<span data-ttu-id="bb501-117">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb501-117">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="bb501-118">Représente le nom unique hérité de la boîte aux lettres de substitution.</span><span class="sxs-lookup"><span data-stu-id="bb501-118">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="bb501-119">Serveur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb501-119">Server (SOAP)</span></span>](server-soap.md) <br/> |<span data-ttu-id="bb501-120">Représente le serveur de boîtes aux lettres de substitution.</span><span class="sxs-lookup"><span data-stu-id="bb501-120">Represents the alternate mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="bb501-121">SmtpAddress (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb501-121">SmtpAddress (SOAP)</span></span>](smtpaddress-soap.md) <br/> |<span data-ttu-id="bb501-122">Représente l’adresse SMTP de la boîte aux lettres de substitution.</span><span class="sxs-lookup"><span data-stu-id="bb501-122">Represents the alternate mailbox SMTP address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bb501-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bb501-123">Parent elements</span></span>

|<span data-ttu-id="bb501-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bb501-124">**Element**</span></span>|<span data-ttu-id="bb501-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="bb501-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb501-126">AlternateMailboxes (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb501-126">AlternateMailboxes (SOAP)</span></span>](alternatemailboxes-soap.md) <br/> |<span data-ttu-id="bb501-127">Représente une collection de boîtes aux lettres de substitution.</span><span class="sxs-lookup"><span data-stu-id="bb501-127">Represents a collection of alternate mailboxes.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bb501-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bb501-128">Text value</span></span>

<span data-ttu-id="bb501-129">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bb501-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb501-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bb501-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb501-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bb501-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="bb501-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bb501-132">Schema Name</span></span>  <br/> |<span data-ttu-id="bb501-133">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="bb501-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="bb501-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bb501-134">Validation File</span></span>  <br/> |<span data-ttu-id="bb501-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bb501-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bb501-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bb501-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="bb501-137">True</span><span class="sxs-lookup"><span data-stu-id="bb501-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb501-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bb501-138">See also</span></span>

- [<span data-ttu-id="bb501-139">AlternateMailboxCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb501-139">AlternateMailboxCollectionSetting (SOAP)</span></span>](alternatemailboxcollectionsetting-soap.md)

