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
ms.openlocfilehash: 5848d52a68c8c3f747614015e49becb34bc4cfd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755109"
---
# <a name="agentexecution"></a><span data-ttu-id="34ff5-103">agentExecution</span><span class="sxs-lookup"><span data-stu-id="34ff5-103">agentExecution</span></span>
  
<span data-ttu-id="34ff5-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="34ff5-104">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="34ff5-105">L’élément **agentExecution** définit la durée, en millisecondes, pour le serveur d’accès au Client ou de la boîte aux lettres doit attendre un agent renvoyer à partir d’un événement avant de les écrire dans le journal des événements.</span><span class="sxs-lookup"><span data-stu-id="34ff5-105">The **agentExecution** element defines the time, in milliseconds, for the Client Access or Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span> 
  
- [<span data-ttu-id="34ff5-106">configuration</span><span class="sxs-lookup"><span data-stu-id="34ff5-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="34ff5-107">surveillance</span><span class="sxs-lookup"><span data-stu-id="34ff5-107">monitoring</span></span>](monitoring.md)
- [<span data-ttu-id="34ff5-108">agentExecution</span><span class="sxs-lookup"><span data-stu-id="34ff5-108">agentExecution</span></span>](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

<span data-ttu-id="34ff5-109">**agentExecutionType (type complexe)**</span><span class="sxs-lookup"><span data-stu-id="34ff5-109">**agentExecutionType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="34ff5-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="34ff5-110">Attributes and elements</span></span>

<span data-ttu-id="34ff5-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="34ff5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34ff5-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="34ff5-112">Attributes</span></span>

|<span data-ttu-id="34ff5-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="34ff5-113">**Attribute**</span></span>|<span data-ttu-id="34ff5-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="34ff5-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="34ff5-115">**timeLimitInMilliseconds**</span><span class="sxs-lookup"><span data-stu-id="34ff5-115">**timeLimitInMilliseconds**</span></span> <br/> |<span data-ttu-id="34ff5-116">Une valeur entière positive qui spécifie la durée, en millisecondes, pour le serveur doit attendre pour un agent renvoyer à partir d’un événement avant qu’il écrit un message d’avertissement dans le journal des événements.</span><span class="sxs-lookup"><span data-stu-id="34ff5-116">A positive integer value that specifies the time, in milliseconds, for the server to wait for an agent to return from an event before it writes a warning to the event log.</span></span> <span data-ttu-id="34ff5-117">Performances peuvent diminuer si cette valeur est trop petite.</span><span class="sxs-lookup"><span data-stu-id="34ff5-117">Performance can decrease if this value is too small.</span></span> <span data-ttu-id="34ff5-118">La valeur suggérée pour cet attribut est 300 000, ce qui équivaut à 5 minutes.</span><span class="sxs-lookup"><span data-stu-id="34ff5-118">The suggested value for this attribute is 300,000, which equates to 5 minutes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="34ff5-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="34ff5-119">Child elements</span></span>

<span data-ttu-id="34ff5-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="34ff5-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34ff5-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="34ff5-121">Parent elements</span></span>

|<span data-ttu-id="34ff5-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="34ff5-122">**Element**</span></span>|<span data-ttu-id="34ff5-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="34ff5-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34ff5-124">surveillance</span><span class="sxs-lookup"><span data-stu-id="34ff5-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="34ff5-125">Contient des informations de configuration qui définit comment et quand le service de Transport frontal ou le service de Transport analyse les agents qui sont installés.</span><span class="sxs-lookup"><span data-stu-id="34ff5-125">Contains configuration information that defines how and when the Front End Transport service or the Transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="34ff5-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="34ff5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34ff5-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="34ff5-127">Namespace</span></span>  <br/> |<span data-ttu-id="34ff5-128">Ce fichier ne définit pas un espace de noms.</span><span class="sxs-lookup"><span data-stu-id="34ff5-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="34ff5-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="34ff5-129">Schema Name</span></span>  <br/> |<span data-ttu-id="34ff5-130">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="34ff5-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="34ff5-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="34ff5-131">Validation File</span></span>  <br/> |<span data-ttu-id="34ff5-132">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="34ff5-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="34ff5-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="34ff5-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="34ff5-134">Faux</span><span class="sxs-lookup"><span data-stu-id="34ff5-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34ff5-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="34ff5-135">See also</span></span>

- [<span data-ttu-id="34ff5-136">Éléments du fichier de configuration agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="34ff5-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

