---
title: Utilisateur (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6bc0031-bc1d-41bd-84e4-9074a5b77012
description: L’élément User représente l’identité d’un utilisateur unique.
ms.openlocfilehash: f151ffa8050a10cdbb4562471d815f8692596cc3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456345"
---
# <a name="user-soap"></a><span data-ttu-id="3eaa0-103">Utilisateur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3eaa0-103">User (SOAP)</span></span>

<span data-ttu-id="3eaa0-104">L’élément **User** représente l’identité d’un utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="3eaa0-104">The **User** element represents the identity of a single user.</span></span> 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 <span data-ttu-id="3eaa0-105">**User**</span><span class="sxs-lookup"><span data-stu-id="3eaa0-105">**User**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3eaa0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3eaa0-106">Attributes and elements</span></span>

<span data-ttu-id="3eaa0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3eaa0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3eaa0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3eaa0-108">Attributes</span></span>

<span data-ttu-id="3eaa0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3eaa0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3eaa0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3eaa0-110">Child elements</span></span>

|<span data-ttu-id="3eaa0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3eaa0-111">**Element**</span></span>|<span data-ttu-id="3eaa0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3eaa0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3eaa0-113">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3eaa0-113">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="3eaa0-114">Représente le nom unique hérité de la boîte aux lettres de substitution.</span><span class="sxs-lookup"><span data-stu-id="3eaa0-114">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="3eaa0-115">Boîte aux lettres (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3eaa0-115">Mailbox (SOAP)</span></span>](mailbox-soap.md) <br/> |<span data-ttu-id="3eaa0-116">Contient l’adresse de messagerie de l’utilisateur à découvrir.</span><span class="sxs-lookup"><span data-stu-id="3eaa0-116">Contains the e-mail address of the user to be discovered.</span></span>  <br/> |
|[<span data-ttu-id="3eaa0-117">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3eaa0-117">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="3eaa0-118">Contient les noms des paramètres de configuration demandés.</span><span class="sxs-lookup"><span data-stu-id="3eaa0-118">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3eaa0-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3eaa0-119">Parent elements</span></span>

|<span data-ttu-id="3eaa0-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3eaa0-120">**Element**</span></span>|<span data-ttu-id="3eaa0-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="3eaa0-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3eaa0-122">Utilisateurs (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3eaa0-122">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="3eaa0-123">Représente une collection d’éléments **utilisateur** .</span><span class="sxs-lookup"><span data-stu-id="3eaa0-123">Represents a collection of **User** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3eaa0-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3eaa0-124">Text value</span></span>

<span data-ttu-id="3eaa0-125">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3eaa0-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3eaa0-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3eaa0-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3eaa0-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3eaa0-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3eaa0-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3eaa0-128">Schema Name</span></span>  <br/> |<span data-ttu-id="3eaa0-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="3eaa0-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3eaa0-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3eaa0-130">Validation File</span></span>  <br/> |<span data-ttu-id="3eaa0-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3eaa0-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3eaa0-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3eaa0-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="3eaa0-133">True</span><span class="sxs-lookup"><span data-stu-id="3eaa0-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3eaa0-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3eaa0-134">See also</span></span>



[<span data-ttu-id="3eaa0-135">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3eaa0-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="3eaa0-136">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3eaa0-136">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="3eaa0-137">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3eaa0-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

