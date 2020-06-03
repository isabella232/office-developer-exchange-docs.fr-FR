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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44446489"
---
# <a name="agentexecution"></a><span data-ttu-id="81e24-103">agentExecution</span><span class="sxs-lookup"><span data-stu-id="81e24-103">agentExecution</span></span>
  
<span data-ttu-id="81e24-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="81e24-104">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="81e24-105">L’élément **agentExecution** définit le temps, en millisecondes, pendant lequel le serveur d’accès au client ou de boîtes aux lettres doit attendre qu’un agent renvoie à partir d’un événement avant d’écrire dans le journal des événements.</span><span class="sxs-lookup"><span data-stu-id="81e24-105">The **agentExecution** element defines the time, in milliseconds, for the Client Access or Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span> 
  
- [<span data-ttu-id="81e24-106">configuration</span><span class="sxs-lookup"><span data-stu-id="81e24-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="81e24-107">surveillance</span><span class="sxs-lookup"><span data-stu-id="81e24-107">monitoring</span></span>](monitoring.md)
- [<span data-ttu-id="81e24-108">agentExecution</span><span class="sxs-lookup"><span data-stu-id="81e24-108">agentExecution</span></span>](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

<span data-ttu-id="81e24-109">**agentExecutionType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="81e24-109">**agentExecutionType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="81e24-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="81e24-110">Attributes and elements</span></span>

<span data-ttu-id="81e24-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="81e24-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81e24-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="81e24-112">Attributes</span></span>

|<span data-ttu-id="81e24-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="81e24-113">**Attribute**</span></span>|<span data-ttu-id="81e24-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="81e24-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="81e24-115">**timeLimitInMilliseconds**</span><span class="sxs-lookup"><span data-stu-id="81e24-115">**timeLimitInMilliseconds**</span></span> <br/> |<span data-ttu-id="81e24-116">Valeur entière positive qui spécifie le temps, en millisecondes, pendant lequel le serveur doit attendre qu’un agent renvoie à partir d’un événement avant d’écrire un avertissement dans le journal des événements.</span><span class="sxs-lookup"><span data-stu-id="81e24-116">A positive integer value that specifies the time, in milliseconds, for the server to wait for an agent to return from an event before it writes a warning to the event log.</span></span> <span data-ttu-id="81e24-117">Les performances peuvent diminuer si cette valeur est trop petite.</span><span class="sxs-lookup"><span data-stu-id="81e24-117">Performance can decrease if this value is too small.</span></span> <span data-ttu-id="81e24-118">La valeur suggérée pour cet attribut est 300 000, ce qui équivaut à 5 minutes.</span><span class="sxs-lookup"><span data-stu-id="81e24-118">The suggested value for this attribute is 300,000, which equates to 5 minutes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="81e24-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="81e24-119">Child elements</span></span>

<span data-ttu-id="81e24-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="81e24-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="81e24-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="81e24-121">Parent elements</span></span>

|<span data-ttu-id="81e24-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="81e24-122">**Element**</span></span>|<span data-ttu-id="81e24-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="81e24-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81e24-124">surveillance</span><span class="sxs-lookup"><span data-stu-id="81e24-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="81e24-125">Contient des informations de configuration qui définissent comment et quand le service de transport frontal ou le service de transport surveille les agents installés.</span><span class="sxs-lookup"><span data-stu-id="81e24-125">Contains configuration information that defines how and when the Front End Transport service or the Transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="81e24-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="81e24-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81e24-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="81e24-127">Namespace</span></span>  <br/> |<span data-ttu-id="81e24-128">Ce fichier ne définit pas d’espace de noms.</span><span class="sxs-lookup"><span data-stu-id="81e24-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="81e24-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="81e24-129">Schema Name</span></span>  <br/> |<span data-ttu-id="81e24-130">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="81e24-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="81e24-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="81e24-131">Validation File</span></span>  <br/> |<span data-ttu-id="81e24-132">Non disponible.</span><span class="sxs-lookup"><span data-stu-id="81e24-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="81e24-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="81e24-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="81e24-134">Faux.</span><span class="sxs-lookup"><span data-stu-id="81e24-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81e24-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="81e24-135">See also</span></span>

- [<span data-ttu-id="81e24-136">Éléments du fichier de configuration des agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="81e24-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

