---
title: DiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 085384f9-dca4-4534-82e2-dd782471d0da
description: L’élément DiscoverySearchConfiguration spécifie la configuration de la recherche de découverte électronique.
ms.openlocfilehash: 8819d951f35ccc215bdf0128d2a16b60bbf20f2a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529055"
---
# <a name="discoverysearchconfiguration"></a><span data-ttu-id="00a59-103">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="00a59-103">DiscoverySearchConfiguration</span></span>

<span data-ttu-id="00a59-104">L’élément **DiscoverySearchConfiguration** spécifie la configuration de la recherche de découverte électronique.</span><span class="sxs-lookup"><span data-stu-id="00a59-104">The **DiscoverySearchConfiguration** element specifies the configuration for eDiscovery search.</span></span> 
  
```XML
<DiscoverySearchConfiguration>
    <SearchId></SearchId>
    <SearchQuery></SearchQuery>
    <SearchableMailboxes></SearchableMailboxes>
</DiscoverySearchConfiguration>
```

 <span data-ttu-id="00a59-105">**DiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="00a59-105">**DiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00a59-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="00a59-106">Attributes and elements</span></span>

<span data-ttu-id="00a59-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="00a59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00a59-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="00a59-108">Attributes</span></span>

<span data-ttu-id="00a59-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="00a59-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00a59-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="00a59-110">Child elements</span></span>

|<span data-ttu-id="00a59-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00a59-111">**Element**</span></span>|<span data-ttu-id="00a59-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="00a59-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00a59-113">SearchId</span><span class="sxs-lookup"><span data-stu-id="00a59-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="00a59-114">Spécifie l’identificateur de la recherche.</span><span class="sxs-lookup"><span data-stu-id="00a59-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="00a59-115">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="00a59-115">SearchQuery</span></span>](searchquery.md) <br/> |<span data-ttu-id="00a59-116">Spécifie le nom d’une requête de recherche de découverte électronique.</span><span class="sxs-lookup"><span data-stu-id="00a59-116">Specifies the name of an eDiscovery search query.</span></span>  <br/> |
|[<span data-ttu-id="00a59-117">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="00a59-117">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="00a59-118">Contient une liste des boîtes aux lettres renvoyées par une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="00a59-118">Contains a list of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00a59-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="00a59-119">Parent elements</span></span>

|<span data-ttu-id="00a59-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00a59-120">**Element**</span></span>|<span data-ttu-id="00a59-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="00a59-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00a59-122">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="00a59-122">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md) <br/> |<span data-ttu-id="00a59-123">Spécifie un tableau d’éléments **DiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="00a59-123">Specifies an array of **DiscoverySearchConfiguration** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="00a59-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="00a59-124">Remarks</span></span>

<span data-ttu-id="00a59-125">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="00a59-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="00a59-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="00a59-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00a59-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="00a59-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00a59-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="00a59-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="00a59-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="00a59-129">Schema Name</span></span>  <br/> |<span data-ttu-id="00a59-130">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="00a59-130">Message schema</span></span>  <br/> |
|<span data-ttu-id="00a59-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="00a59-131">Validation File</span></span>  <br/> |<span data-ttu-id="00a59-132">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="00a59-132">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="00a59-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="00a59-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="00a59-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00a59-134">See also</span></span>

- [<span data-ttu-id="00a59-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="00a59-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

