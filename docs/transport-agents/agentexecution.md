---
title: agentExecution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: 457257e59fb37659daf2f91b0fa5dfced5c48c03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44446489"
---
# <a name="agentexecution"></a><span data-ttu-id="62133-103">agentExecution</span><span class="sxs-lookup"><span data-stu-id="62133-103">agentExecution</span></span>
  
<span data-ttu-id="62133-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="62133-104">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="62133-105">L’élément **agentExecution** définit le temps, en millisecondes, pendant lequel le serveur d’accès au client ou de boîtes aux lettres doit attendre qu’un agent renvoie à partir d’un événement avant d’écrire dans le journal des événements.</span><span class="sxs-lookup"><span data-stu-id="62133-105">The **agentExecution** element defines the time, in milliseconds, for the Client Access or Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span> 
  
- [<span data-ttu-id="62133-106">configuration</span><span class="sxs-lookup"><span data-stu-id="62133-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="62133-107">surveillance</span><span class="sxs-lookup"><span data-stu-id="62133-107">monitoring</span></span>](monitoring.md)
- [<span data-ttu-id="62133-108">agentExecution</span><span class="sxs-lookup"><span data-stu-id="62133-108">agentExecution</span></span>](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

<span data-ttu-id="62133-109">**agentExecutionType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="62133-109">**agentExecutionType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="62133-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="62133-110">Attributes and elements</span></span>

<span data-ttu-id="62133-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="62133-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="62133-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="62133-112">Attributes</span></span>

|<span data-ttu-id="62133-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="62133-113">**Attribute**</span></span>|<span data-ttu-id="62133-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="62133-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="62133-115">**timeLimitInMilliseconds**</span><span class="sxs-lookup"><span data-stu-id="62133-115">**timeLimitInMilliseconds**</span></span> <br/> |<span data-ttu-id="62133-116">Valeur entière positive qui spécifie le temps, en millisecondes, pendant lequel le serveur doit attendre qu’un agent renvoie à partir d’un événement avant d’écrire un avertissement dans le journal des événements.</span><span class="sxs-lookup"><span data-stu-id="62133-116">A positive integer value that specifies the time, in milliseconds, for the server to wait for an agent to return from an event before it writes a warning to the event log.</span></span> <span data-ttu-id="62133-117">Les performances peuvent diminuer si cette valeur est trop petite.</span><span class="sxs-lookup"><span data-stu-id="62133-117">Performance can decrease if this value is too small.</span></span> <span data-ttu-id="62133-118">La valeur suggérée pour cet attribut est 300 000, ce qui équivaut à 5 minutes.</span><span class="sxs-lookup"><span data-stu-id="62133-118">The suggested value for this attribute is 300,000, which equates to 5 minutes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="62133-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="62133-119">Child elements</span></span>

<span data-ttu-id="62133-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="62133-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="62133-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="62133-121">Parent elements</span></span>

|<span data-ttu-id="62133-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="62133-122">**Element**</span></span>|<span data-ttu-id="62133-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="62133-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62133-124">surveillance</span><span class="sxs-lookup"><span data-stu-id="62133-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="62133-125">Contient des informations de configuration qui définissent comment et quand le service de transport frontal ou le service de transport surveille les agents installés.</span><span class="sxs-lookup"><span data-stu-id="62133-125">Contains configuration information that defines how and when the Front End Transport service or the Transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="62133-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="62133-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="62133-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="62133-127">Namespace</span></span>  <br/> |<span data-ttu-id="62133-128">Ce fichier ne définit pas d’espace de noms.</span><span class="sxs-lookup"><span data-stu-id="62133-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="62133-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="62133-129">Schema Name</span></span>  <br/> |<span data-ttu-id="62133-130">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="62133-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="62133-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="62133-131">Validation File</span></span>  <br/> |<span data-ttu-id="62133-132">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="62133-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="62133-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="62133-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="62133-134">Faux.</span><span class="sxs-lookup"><span data-stu-id="62133-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="62133-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="62133-135">See also</span></span>

- [<span data-ttu-id="62133-136">Éléments du fichier de configuration des agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="62133-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

