---
title: messageSnapshot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- messageSnapshot
api_type:
- schema
ms.assetid: f157e44c-b950-463f-b086-31d5da94b7ff
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: 8a58444580c803efb7312df95d75d697bc42e8e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461841"
---
# <a name="messagesnapshot"></a><span data-ttu-id="885b3-103">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="885b3-103">messageSnapshot</span></span>

<span data-ttu-id="885b3-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="885b3-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="885b3-105">L’élément **messageSnapshot** contient un attribut qui spécifie si la fonctionnalité de suivi du pipeline est activée pour le serveur Exchange sur lequel le rôle serveur d’accès au client ou de boîte aux lettres est installé.</span><span class="sxs-lookup"><span data-stu-id="885b3-105">The **messageSnapshot** element contains an attribute that specifies whether the pipeline tracing feature is enabled for the Exchange server that has the Client Access or the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="885b3-106">configuration</span><span class="sxs-lookup"><span data-stu-id="885b3-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="885b3-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="885b3-107">mexRuntime</span></span>](mexruntime.md) 
- [<span data-ttu-id="885b3-108">surveillance</span><span class="sxs-lookup"><span data-stu-id="885b3-108">monitoring</span></span>](monitoring.md) 
- [<span data-ttu-id="885b3-109">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="885b3-109">messageSnapshot</span></span>](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

<span data-ttu-id="885b3-110">**messageSnapshotType (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="885b3-110">**messageSnapshotType (Boolean)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="885b3-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="885b3-111">Attributes and elements</span></span>

<span data-ttu-id="885b3-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="885b3-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="885b3-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="885b3-113">Attributes</span></span>

|<span data-ttu-id="885b3-114">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="885b3-114">**Attribute**</span></span>|<span data-ttu-id="885b3-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="885b3-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="885b3-116">**enabled**</span><span class="sxs-lookup"><span data-stu-id="885b3-116">**enabled**</span></span> <br/> |<span data-ttu-id="885b3-117">Valeur booléenne qui indique si la fonctionnalité de suivi de pipeline est activée pour le serveur d’accès au client ou de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="885b3-117">A Boolean value that indicates whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span> <span data-ttu-id="885b3-118">La valeur est **true** si le suivi du pipeline est activé ; dans le cas contraire, la valeur est **false** ou l’élément n’est pas présent.</span><span class="sxs-lookup"><span data-stu-id="885b3-118">The value is **true** if pipeline tracing is enabled; otherwise, the value is **false** or the element is not present.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="885b3-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="885b3-119">Child elements</span></span>

<span data-ttu-id="885b3-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="885b3-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="885b3-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="885b3-121">Parent elements</span></span>

|<span data-ttu-id="885b3-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="885b3-122">**Element**</span></span>|<span data-ttu-id="885b3-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="885b3-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="885b3-124">surveillance</span><span class="sxs-lookup"><span data-stu-id="885b3-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="885b3-125">Contient des informations de configuration qui définissent comment et quand le service de transport analyse les agents installés.</span><span class="sxs-lookup"><span data-stu-id="885b3-125">Contains configuration information that defines how and when the transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="885b3-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="885b3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="885b3-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="885b3-127">Namespace</span></span>  <br/> |<span data-ttu-id="885b3-128">Ce fichier ne définit pas d’espace de noms.</span><span class="sxs-lookup"><span data-stu-id="885b3-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="885b3-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="885b3-129">Schema Name</span></span>  <br/> |<span data-ttu-id="885b3-130">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="885b3-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="885b3-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="885b3-131">Validation File</span></span>  <br/> |<span data-ttu-id="885b3-132">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="885b3-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="885b3-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="885b3-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="885b3-134">Faux.</span><span class="sxs-lookup"><span data-stu-id="885b3-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="885b3-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="885b3-135">See also</span></span>

- [<span data-ttu-id="885b3-136">Éléments du fichier de configuration des agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="885b3-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

