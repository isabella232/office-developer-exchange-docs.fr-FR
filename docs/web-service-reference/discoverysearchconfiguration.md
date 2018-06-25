---
title: DiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 085384f9-dca4-4534-82e2-dd782471d0da
description: L’élément DiscoverySearchConfiguration spécifie la configuration de recherche de découverte électronique.
ms.openlocfilehash: 11bf90d8fe73bb0b308deb7ae51f1443488f87e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755971"
---
# <a name="discoverysearchconfiguration"></a><span data-ttu-id="65cda-103">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="65cda-103">DiscoverySearchConfiguration</span></span>

<span data-ttu-id="65cda-104">L’élément **DiscoverySearchConfiguration** spécifie la configuration de recherche de découverte électronique.</span><span class="sxs-lookup"><span data-stu-id="65cda-104">The **DiscoverySearchConfiguration** element specifies the configuration for eDiscovery search.</span></span> 
  
```XML
<DiscoverySearchConfiguration>
    <SearchId></SearchId>
    <SearchQuery></SearchQuery>
    <SearchableMailboxes></SearchableMailboxes>
</DiscoverySearchConfiguration>
```

 <span data-ttu-id="65cda-105">**DiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="65cda-105">**DiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65cda-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="65cda-106">Attributes and elements</span></span>

<span data-ttu-id="65cda-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="65cda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65cda-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="65cda-108">Attributes</span></span>

<span data-ttu-id="65cda-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="65cda-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65cda-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="65cda-110">Child elements</span></span>

|<span data-ttu-id="65cda-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65cda-111">**Element**</span></span>|<span data-ttu-id="65cda-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="65cda-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65cda-113">Valeur SearchId</span><span class="sxs-lookup"><span data-stu-id="65cda-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="65cda-114">Spécifie l’identificateur de la recherche.</span><span class="sxs-lookup"><span data-stu-id="65cda-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="65cda-115">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="65cda-115">SearchQuery</span></span>](searchquery.md) <br/> |<span data-ttu-id="65cda-116">Spécifie le nom d’une requête de recherche de découverte électronique.</span><span class="sxs-lookup"><span data-stu-id="65cda-116">Specifies the name of an eDiscovery search query.</span></span>  <br/> |
|[<span data-ttu-id="65cda-117">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="65cda-117">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="65cda-118">Contient une liste des boîtes aux lettres renvoyé à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="65cda-118">Contains a list of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65cda-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="65cda-119">Parent elements</span></span>

|<span data-ttu-id="65cda-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65cda-120">**Element**</span></span>|<span data-ttu-id="65cda-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="65cda-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65cda-122">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="65cda-122">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md) <br/> |<span data-ttu-id="65cda-123">Spécifie un tableau d’éléments **DiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="65cda-123">Specifies an array of **DiscoverySearchConfiguration** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="65cda-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="65cda-124">Remarks</span></span>

<span data-ttu-id="65cda-125">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="65cda-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="65cda-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="65cda-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65cda-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="65cda-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65cda-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="65cda-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="65cda-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="65cda-129">Schema Name</span></span>  <br/> |<span data-ttu-id="65cda-130">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="65cda-130">Message schema</span></span>  <br/> |
|<span data-ttu-id="65cda-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="65cda-131">Validation File</span></span>  <br/> |<span data-ttu-id="65cda-132">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="65cda-132">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="65cda-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="65cda-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="65cda-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65cda-134">See also</span></span>

- [<span data-ttu-id="65cda-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="65cda-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

