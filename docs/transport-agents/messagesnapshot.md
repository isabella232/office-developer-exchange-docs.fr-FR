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
ms.openlocfilehash: 4b814def8eef8fb452d2e754c5f6787d644055f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755140"
---
# <a name="messagesnapshot"></a><span data-ttu-id="8ce51-103">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="8ce51-103">messageSnapshot</span></span>

<span data-ttu-id="8ce51-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="8ce51-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="8ce51-105">L’élément **messageSnapshot** contient un attribut qui spécifie si la fonctionnalité de suivi du pipeline est activée pour le serveur Exchange qui a l’accès au Client ou le rôle serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8ce51-105">The **messageSnapshot** element contains an attribute that specifies whether the pipeline tracing feature is enabled for the Exchange server that has the Client Access or the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="8ce51-106">configuration</span><span class="sxs-lookup"><span data-stu-id="8ce51-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="8ce51-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="8ce51-107">mexRuntime</span></span>](mexruntime.md) 
- [<span data-ttu-id="8ce51-108">surveillance</span><span class="sxs-lookup"><span data-stu-id="8ce51-108">monitoring</span></span>](monitoring.md) 
- [<span data-ttu-id="8ce51-109">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="8ce51-109">messageSnapshot</span></span>](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

<span data-ttu-id="8ce51-110">**messageSnapshotType (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="8ce51-110">**messageSnapshotType (Boolean)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8ce51-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8ce51-111">Attributes and elements</span></span>

<span data-ttu-id="8ce51-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8ce51-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ce51-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="8ce51-113">Attributes</span></span>

|<span data-ttu-id="8ce51-114">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="8ce51-114">**Attribute**</span></span>|<span data-ttu-id="8ce51-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="8ce51-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8ce51-116">**activé**</span><span class="sxs-lookup"><span data-stu-id="8ce51-116">**enabled**</span></span> <br/> |<span data-ttu-id="8ce51-117">Une valeur de type Boolean qui indique si la fonctionnalité de suivi du pipeline est activée pour l’accès au Client ou le serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8ce51-117">A Boolean value that indicates whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span> <span data-ttu-id="8ce51-118">La valeur est **true** si le suivi du pipeline est activé ; dans le cas contraire, la valeur est **false** ou l’élément n’est pas présent.</span><span class="sxs-lookup"><span data-stu-id="8ce51-118">The value is **true** if pipeline tracing is enabled; otherwise, the value is **false** or the element is not present.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8ce51-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8ce51-119">Child elements</span></span>

<span data-ttu-id="8ce51-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8ce51-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ce51-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8ce51-121">Parent elements</span></span>

|<span data-ttu-id="8ce51-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8ce51-122">**Element**</span></span>|<span data-ttu-id="8ce51-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="8ce51-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ce51-124">surveillance</span><span class="sxs-lookup"><span data-stu-id="8ce51-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="8ce51-125">Contient des informations de configuration qui définit comment et quand le service de transport analyse les agents qui sont installés.</span><span class="sxs-lookup"><span data-stu-id="8ce51-125">Contains configuration information that defines how and when the transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="8ce51-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8ce51-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ce51-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8ce51-127">Namespace</span></span>  <br/> |<span data-ttu-id="8ce51-128">Ce fichier ne définit pas un espace de noms.</span><span class="sxs-lookup"><span data-stu-id="8ce51-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="8ce51-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8ce51-129">Schema Name</span></span>  <br/> |<span data-ttu-id="8ce51-130">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="8ce51-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="8ce51-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8ce51-131">Validation File</span></span>  <br/> |<span data-ttu-id="8ce51-132">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="8ce51-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="8ce51-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8ce51-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="8ce51-134">Faux</span><span class="sxs-lookup"><span data-stu-id="8ce51-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ce51-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8ce51-135">See also</span></span>

- [<span data-ttu-id="8ce51-136">Éléments du fichier de configuration agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8ce51-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

