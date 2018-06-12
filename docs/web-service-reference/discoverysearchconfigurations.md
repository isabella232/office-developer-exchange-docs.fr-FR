---
title: DiscoverySearchConfigurations
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f04b14c9-384c-4016-b113-52a49e15e73b
description: L’élément DiscoverySearchConfigurations spécifie un tableau d’éléments DiscoverySearchConfiguration.
ms.openlocfilehash: a95bb35b88114e8e72e22de424679993fd4eef2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755980"
---
# <a name="discoverysearchconfigurations"></a><span data-ttu-id="00af4-103">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="00af4-103">DiscoverySearchConfigurations</span></span>

<span data-ttu-id="00af4-104">L’élément **DiscoverySearchConfigurations** spécifie un tableau d’éléments **DiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="00af4-104">The **DiscoverySearchConfigurations** element specifies an array of **DiscoverySearchConfiguration** elements.</span></span> 
  
```XML
<DiscoverySearchConfigurations>
    <DiscoverySearchConfiguration></DiscoverySearchConfiguration>
</DiscoverySearchConfigurations>
```

 <span data-ttu-id="00af4-105">**ArrayOfDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="00af4-105">**ArrayOfDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00af4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="00af4-106">Attributes and elements</span></span>

<span data-ttu-id="00af4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="00af4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00af4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="00af4-108">Attributes</span></span>

<span data-ttu-id="00af4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="00af4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00af4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="00af4-110">Child elements</span></span>

|<span data-ttu-id="00af4-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00af4-111">**Element**</span></span>|<span data-ttu-id="00af4-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="00af4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00af4-113">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="00af4-113">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md) <br/> |<span data-ttu-id="00af4-114">Spécifie la configuration de recherche de découverte électronique.</span><span class="sxs-lookup"><span data-stu-id="00af4-114">Specifies the configuration for eDiscovery search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00af4-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="00af4-115">Parent elements</span></span>

|<span data-ttu-id="00af4-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00af4-116">**Element**</span></span>|<span data-ttu-id="00af4-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="00af4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00af4-118">GetDiscoverySearchConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="00af4-118">GetDiscoverySearchConfigurationResponseMessage</span></span>](getdiscoverysearchconfigurationresponsemessage.md) <br/> |<span data-ttu-id="00af4-119">Spécifie le message de réponse pour une demande **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="00af4-119">Specifies the response message for a **GetDiscoverySearchConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="00af4-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="00af4-120">Remarks</span></span>

<span data-ttu-id="00af4-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="00af4-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="00af4-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="00af4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00af4-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="00af4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00af4-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="00af4-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="00af4-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="00af4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="00af4-126">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="00af4-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="00af4-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="00af4-127">Validation File</span></span>  <br/> |<span data-ttu-id="00af4-128">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="00af4-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="00af4-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="00af4-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="00af4-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00af4-130">See also</span></span>

- [<span data-ttu-id="00af4-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="00af4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

