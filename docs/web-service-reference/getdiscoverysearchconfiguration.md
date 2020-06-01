---
title: GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e15dbfca-3b9d-463e-94ec-4f1b6115bee3
description: L’élément GetDiscoverySearchConfiguration spécifie une demande de récupération de la configuration de recherche de découverte électronique.
ms.openlocfilehash: 821c5e1429c160e326f6d99df3ff4fcc831b83d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461001"
---
# <a name="getdiscoverysearchconfiguration"></a><span data-ttu-id="79692-103">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="79692-103">GetDiscoverySearchConfiguration</span></span>

<span data-ttu-id="79692-104">L’élément **GetDiscoverySearchConfiguration** spécifie une demande de récupération de la configuration de recherche de découverte électronique.</span><span class="sxs-lookup"><span data-stu-id="79692-104">The **GetDiscoverySearchConfiguration** element specifies a request to retrieve the eDiscovery search configuration.</span></span> 
  
```XML
<GetDiscoverySearchConfiguration>
    <SearchId/>
    <ExpandGroupMembership/>
</GetDiscoverySearchConfiguration>
```

 <span data-ttu-id="79692-105">**GetDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="79692-105">**GetDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79692-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="79692-106">Attributes and elements</span></span>

<span data-ttu-id="79692-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="79692-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79692-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="79692-108">Attributes</span></span>

<span data-ttu-id="79692-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="79692-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79692-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="79692-110">Child elements</span></span>

|<span data-ttu-id="79692-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="79692-111">**Element**</span></span>|<span data-ttu-id="79692-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="79692-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79692-113">SearchId</span><span class="sxs-lookup"><span data-stu-id="79692-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="79692-114">Spécifie l’identificateur de la recherche.</span><span class="sxs-lookup"><span data-stu-id="79692-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="79692-115">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="79692-115">ExpandGroupMembership</span></span>](expandgroupmembership.md) <br/> |<span data-ttu-id="79692-116">Contient une valeur de type Boolean qui indique s’il faut développer l’appartenance au groupe renvoyé à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="79692-116">Contains a Boolean value that indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="79692-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="79692-117">Parent elements</span></span>

<span data-ttu-id="79692-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79692-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="79692-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="79692-119">Remarks</span></span>

<span data-ttu-id="79692-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="79692-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="79692-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="79692-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79692-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="79692-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79692-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="79692-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="79692-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="79692-124">Schema Name</span></span>  <br/> |<span data-ttu-id="79692-125">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="79692-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="79692-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="79692-126">Validation File</span></span>  <br/> |<span data-ttu-id="79692-127">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="79692-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="79692-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="79692-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="79692-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79692-129">See also</span></span>



- [<span data-ttu-id="79692-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="79692-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

