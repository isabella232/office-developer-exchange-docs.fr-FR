---
title: Nom de configuration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConfigurationName
api_type:
- schema
ms.assetid: 3b524a2f-9c6b-4550-9f3d-f78d176b0f7b
description: L’élément de nom de configuration spécifie les configurations de service requis par un nom.
ms.openlocfilehash: a03a0bc0ab7ecbc1c2aec31f864503ee0f560908
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755535"
---
# <a name="configurationname"></a><span data-ttu-id="f7c5f-103">Nom de configuration</span><span class="sxs-lookup"><span data-stu-id="f7c5f-103">ConfigurationName</span></span>

<span data-ttu-id="f7c5f-104">L’élément de **nom de configuration** spécifie les configurations de service requis par un nom.</span><span class="sxs-lookup"><span data-stu-id="f7c5f-104">The **ConfigurationName** element specifies the requested service configurations by name.</span></span> 
  
```xml
<ConfigurationName>MailTips or UnifiedMessagingConfiguration or ProtectionRules</ConfigurationName>
```

 <span data-ttu-id="f7c5f-105">**ServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="f7c5f-105">**ServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7c5f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f7c5f-106">Attributes and elements</span></span>

<span data-ttu-id="f7c5f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f7c5f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7c5f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f7c5f-108">Attributes</span></span>

<span data-ttu-id="f7c5f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f7c5f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7c5f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f7c5f-110">Child elements</span></span>

<span data-ttu-id="f7c5f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f7c5f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f7c5f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f7c5f-112">Parent elements</span></span>

|<span data-ttu-id="f7c5f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7c5f-113">**Element**</span></span>|<span data-ttu-id="f7c5f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7c5f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7c5f-115">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7c5f-115">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="f7c5f-116">Contient les configurations de service demandé.</span><span class="sxs-lookup"><span data-stu-id="f7c5f-116">Contains the requested service configurations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f7c5f-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f7c5f-117">Text value</span></span>

<span data-ttu-id="f7c5f-118">Le tableau suivant répertorie les valeurs possibles pour l’élément de **nom de configuration** .</span><span class="sxs-lookup"><span data-stu-id="f7c5f-118">The following table lists the possible values for the **ConfigurationName** element.</span></span> 
  
<span data-ttu-id="f7c5f-119">**Valeurs des éléments de nom de configuration**</span><span class="sxs-lookup"><span data-stu-id="f7c5f-119">**ConfigurationName element values**</span></span>

|<span data-ttu-id="f7c5f-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f7c5f-120">**Value**</span></span>|<span data-ttu-id="f7c5f-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7c5f-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f7c5f-122">Les infos-courrier</span><span class="sxs-lookup"><span data-stu-id="f7c5f-122">MailTips</span></span>  <br/> |<span data-ttu-id="f7c5f-123">Identifie la configuration du service Infos-courrier.</span><span class="sxs-lookup"><span data-stu-id="f7c5f-123">Identifies the MailTips service configuration.</span></span>  <br/> |
|<span data-ttu-id="f7c5f-124">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7c5f-124">UnifiedMessagingConfiguration</span></span>  <br/> |<span data-ttu-id="f7c5f-125">Identifie la configuration du service de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="f7c5f-125">Identifies the Unified Messaging service configuration.</span></span>  <br/> |
|<span data-ttu-id="f7c5f-126">ProtectionRules</span><span class="sxs-lookup"><span data-stu-id="f7c5f-126">ProtectionRules</span></span>  <br/> |<span data-ttu-id="f7c5f-127">Identifie la configuration des règles de Protection du service.</span><span class="sxs-lookup"><span data-stu-id="f7c5f-127">Identifies the Protection Rules service configuration.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f7c5f-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="f7c5f-128">Remarks</span></span>

<span data-ttu-id="f7c5f-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7c5f-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7c5f-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f7c5f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7c5f-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f7c5f-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f7c5f-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f7c5f-132">Schema Name</span></span>  <br/> |<span data-ttu-id="f7c5f-133">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f7c5f-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f7c5f-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f7c5f-134">Validation File</span></span>  <br/> |<span data-ttu-id="f7c5f-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f7c5f-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f7c5f-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f7c5f-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7c5f-137">False</span><span class="sxs-lookup"><span data-stu-id="f7c5f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7c5f-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f7c5f-138">See also</span></span>



- [<span data-ttu-id="f7c5f-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f7c5f-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

