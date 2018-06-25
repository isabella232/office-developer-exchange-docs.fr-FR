---
title: GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e15dbfca-3b9d-463e-94ec-4f1b6115bee3
description: L’élément GetDiscoverySearchConfiguration spécifie une requête pour récupérer la configuration de recherche eDiscovery.
ms.openlocfilehash: 41a3cabb2822c4ee6a31aa7ff3074d62987edc92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756576"
---
# <a name="getdiscoverysearchconfiguration"></a><span data-ttu-id="34234-103">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="34234-103">GetDiscoverySearchConfiguration</span></span>

<span data-ttu-id="34234-104">L’élément **GetDiscoverySearchConfiguration** spécifie une requête pour récupérer la configuration de recherche eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="34234-104">The **GetDiscoverySearchConfiguration** element specifies a request to retrieve the eDiscovery search configuration.</span></span> 
  
```XML
<GetDiscoverySearchConfiguration>
    <SearchId/>
    <ExpandGroupMembership/>
</GetDiscoverySearchConfiguration>
```

 <span data-ttu-id="34234-105">**GetDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="34234-105">**GetDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34234-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="34234-106">Attributes and elements</span></span>

<span data-ttu-id="34234-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="34234-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34234-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="34234-108">Attributes</span></span>

<span data-ttu-id="34234-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="34234-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34234-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="34234-110">Child elements</span></span>

|<span data-ttu-id="34234-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="34234-111">**Element**</span></span>|<span data-ttu-id="34234-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="34234-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34234-113">Valeur SearchId</span><span class="sxs-lookup"><span data-stu-id="34234-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="34234-114">Spécifie l’identificateur de la recherche.</span><span class="sxs-lookup"><span data-stu-id="34234-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="34234-115">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="34234-115">ExpandGroupMembership</span></span>](expandgroupmembership.md) <br/> |<span data-ttu-id="34234-116">Contient une valeur de type Boolean qui indique s’il faut développer l’appartenance au groupe renvoyé à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="34234-116">Contains a Boolean value that indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="34234-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="34234-117">Parent elements</span></span>

<span data-ttu-id="34234-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="34234-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="34234-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="34234-119">Remarks</span></span>

<span data-ttu-id="34234-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="34234-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="34234-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="34234-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34234-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="34234-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34234-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="34234-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="34234-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="34234-124">Schema Name</span></span>  <br/> |<span data-ttu-id="34234-125">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="34234-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="34234-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="34234-126">Validation File</span></span>  <br/> |<span data-ttu-id="34234-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="34234-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="34234-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="34234-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="34234-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="34234-129">See also</span></span>



- [<span data-ttu-id="34234-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="34234-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

