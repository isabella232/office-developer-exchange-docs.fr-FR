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
ms.openlocfilehash: 6af4c8198f2ad73f8b39f9718e11b88aa8075c39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461379"
---
# <a name="discoverysearchconfigurations"></a><span data-ttu-id="c7c1e-103">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="c7c1e-103">DiscoverySearchConfigurations</span></span>

<span data-ttu-id="c7c1e-104">L’élément **DiscoverySearchConfigurations** spécifie un tableau d’éléments **DiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="c7c1e-104">The **DiscoverySearchConfigurations** element specifies an array of **DiscoverySearchConfiguration** elements.</span></span> 
  
```XML
<DiscoverySearchConfigurations>
    <DiscoverySearchConfiguration></DiscoverySearchConfiguration>
</DiscoverySearchConfigurations>
```

 <span data-ttu-id="c7c1e-105">**ArrayOfDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="c7c1e-105">**ArrayOfDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7c1e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c7c1e-106">Attributes and elements</span></span>

<span data-ttu-id="c7c1e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c7c1e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7c1e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c7c1e-108">Attributes</span></span>

<span data-ttu-id="c7c1e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c7c1e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7c1e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c7c1e-110">Child elements</span></span>

|<span data-ttu-id="c7c1e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c7c1e-111">**Element**</span></span>|<span data-ttu-id="c7c1e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c7c1e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7c1e-113">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7c1e-113">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md) <br/> |<span data-ttu-id="c7c1e-114">Spécifie la configuration de la recherche de découverte électronique.</span><span class="sxs-lookup"><span data-stu-id="c7c1e-114">Specifies the configuration for eDiscovery search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7c1e-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c7c1e-115">Parent elements</span></span>

|<span data-ttu-id="c7c1e-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c7c1e-116">**Element**</span></span>|<span data-ttu-id="c7c1e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c7c1e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7c1e-118">GetDiscoverySearchConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c7c1e-118">GetDiscoverySearchConfigurationResponseMessage</span></span>](getdiscoverysearchconfigurationresponsemessage.md) <br/> |<span data-ttu-id="c7c1e-119">Spécifie le message de réponse pour une demande **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="c7c1e-119">Specifies the response message for a **GetDiscoverySearchConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c7c1e-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="c7c1e-120">Remarks</span></span>

<span data-ttu-id="c7c1e-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c7c1e-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c7c1e-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7c1e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7c1e-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c7c1e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7c1e-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c7c1e-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c7c1e-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c7c1e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c7c1e-126">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="c7c1e-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="c7c1e-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c7c1e-127">Validation File</span></span>  <br/> |<span data-ttu-id="c7c1e-128">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c7c1e-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c7c1e-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c7c1e-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c7c1e-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c7c1e-130">See also</span></span>

- [<span data-ttu-id="c7c1e-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c7c1e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

