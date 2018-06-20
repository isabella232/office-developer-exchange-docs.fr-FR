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
description: L’élément représente l’identité d’un utilisateur unique.
ms.openlocfilehash: a8dcb22f5c74a9622f978f34e48146115351fe82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838947"
---
# <a name="user-soap"></a><span data-ttu-id="5a7b3-103">Utilisateur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a7b3-103">User (SOAP)</span></span>

<span data-ttu-id="5a7b3-104">**L’élément** représente l’identité d’un utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="5a7b3-104">The **User** element represents the identity of a single user.</span></span> 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 <span data-ttu-id="5a7b3-105">**User**</span><span class="sxs-lookup"><span data-stu-id="5a7b3-105">**User**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a7b3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5a7b3-106">Attributes and elements</span></span>

<span data-ttu-id="5a7b3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5a7b3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a7b3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5a7b3-108">Attributes</span></span>

<span data-ttu-id="5a7b3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5a7b3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a7b3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5a7b3-110">Child elements</span></span>

|<span data-ttu-id="5a7b3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5a7b3-111">**Element**</span></span>|<span data-ttu-id="5a7b3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="5a7b3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a7b3-113">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a7b3-113">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="5a7b3-114">Représente le nom unique hérité autre boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5a7b3-114">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="5a7b3-115">Boîte aux lettres (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a7b3-115">Mailbox (SOAP)</span></span>](mailbox-soap.md) <br/> |<span data-ttu-id="5a7b3-116">Contient l’adresse de messagerie de l’utilisateur à être découvert.</span><span class="sxs-lookup"><span data-stu-id="5a7b3-116">Contains the e-mail address of the user to be discovered.</span></span>  <br/> |
|[<span data-ttu-id="5a7b3-117">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a7b3-117">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="5a7b3-118">Contient les noms des paramètres de configuration demandé.</span><span class="sxs-lookup"><span data-stu-id="5a7b3-118">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5a7b3-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5a7b3-119">Parent elements</span></span>

|<span data-ttu-id="5a7b3-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5a7b3-120">**Element**</span></span>|<span data-ttu-id="5a7b3-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="5a7b3-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a7b3-122">Utilisateurs (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a7b3-122">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="5a7b3-123">Représente une collection d’éléments de **l’utilisateur** .</span><span class="sxs-lookup"><span data-stu-id="5a7b3-123">Represents a collection of **User** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5a7b3-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5a7b3-124">Text value</span></span>

<span data-ttu-id="5a7b3-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5a7b3-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a7b3-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5a7b3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a7b3-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5a7b3-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5a7b3-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5a7b3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5a7b3-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="5a7b3-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5a7b3-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5a7b3-130">Validation File</span></span>  <br/> |<span data-ttu-id="5a7b3-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5a7b3-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5a7b3-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5a7b3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a7b3-133">True</span><span class="sxs-lookup"><span data-stu-id="5a7b3-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a7b3-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5a7b3-134">See also</span></span>



[<span data-ttu-id="5a7b3-135">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a7b3-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="5a7b3-136">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a7b3-136">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="5a7b3-137">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a7b3-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

