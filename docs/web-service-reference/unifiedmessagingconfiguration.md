---
title: UnifiedMessagingConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnifiedMessagingConfiguration
api_type:
- schema
ms.assetid: cbdb4268-077e-44ed-8ec2-9d759c84cc6d
description: L’élément UnifiedMessagingConfiguration contient des informations de configuration de service pour le service de messagerie unifiée.
ms.openlocfilehash: 3ad8f66ecdf21062c00c2a6ac6f65fac875da38c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838805"
---
# <a name="unifiedmessagingconfiguration"></a><span data-ttu-id="2a4d3-103">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a4d3-103">UnifiedMessagingConfiguration</span></span>

<span data-ttu-id="2a4d3-104">L’élément **UnifiedMessagingConfiguration** contient des informations de configuration de service pour le service de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-104">The **UnifiedMessagingConfiguration** element contains service configuration information for the Unified Messaging service.</span></span> 
  
```XML
<UnifiedMessagingConfiguration>
   <UmEnabled/>
   <PlayOnPhoneDialString/>
   <PlayOnPhoneEnabled/>
</UnifiedMessagingConfiguration>
```

 <span data-ttu-id="2a4d3-105">**UnifiedMessageServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="2a4d3-105">**UnifiedMessageServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a4d3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2a4d3-106">Attributes and elements</span></span>

<span data-ttu-id="2a4d3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a4d3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2a4d3-108">Attributes</span></span>

<span data-ttu-id="2a4d3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a4d3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2a4d3-110">Child elements</span></span>

|<span data-ttu-id="2a4d3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2a4d3-111">**Element**</span></span>|<span data-ttu-id="2a4d3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2a4d3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a4d3-113">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="2a4d3-113">UmEnabled</span></span>](umenabled.md) <br/> |<span data-ttu-id="2a4d3-114">Indique si la messagerie unifiée est activée pour un compte.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-114">Indicates whether Unified Messaging is enabled for an account.</span></span> <span data-ttu-id="2a4d3-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="2a4d3-116">PlayOnPhoneDialString (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="2a4d3-116">PlayOnPhoneDialString (Exchange Web Services)</span></span>](playonphonedialstring-exchange-web-services.md) <br/> |<span data-ttu-id="2a4d3-117">Identifie la chaîne de numérotation lire sur le téléphone.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-117">Identifies the Play-on-Phone dial string.</span></span> <span data-ttu-id="2a4d3-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="2a4d3-119">PlayOnPhoneEnabled</span><span class="sxs-lookup"><span data-stu-id="2a4d3-119">PlayOnPhoneEnabled</span></span>](playonphoneenabled.md) <br/> |<span data-ttu-id="2a4d3-120">Indique si la fonctionnalité de lecture sur le téléphone est activée.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-120">Indicates whether the Play-on-Phone feature is enabled.</span></span> <span data-ttu-id="2a4d3-121">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2a4d3-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2a4d3-122">Parent elements</span></span>

|<span data-ttu-id="2a4d3-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2a4d3-123">**Element**</span></span>|<span data-ttu-id="2a4d3-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="2a4d3-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a4d3-125">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="2a4d3-125">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="2a4d3-126">Contient les paramètres de configuration de service.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-126">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2a4d3-127">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2a4d3-127">Text value</span></span>

<span data-ttu-id="2a4d3-128">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2a4d3-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="2a4d3-129">Remarks</span></span>

<span data-ttu-id="2a4d3-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2a4d3-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a4d3-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2a4d3-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a4d3-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2a4d3-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2a4d3-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2a4d3-133">Schema Name</span></span>  <br/> |<span data-ttu-id="2a4d3-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="2a4d3-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2a4d3-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2a4d3-135">Validation File</span></span>  <br/> |<span data-ttu-id="2a4d3-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2a4d3-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2a4d3-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2a4d3-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="2a4d3-138">False</span><span class="sxs-lookup"><span data-stu-id="2a4d3-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2a4d3-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2a4d3-139">See also</span></span>



- [<span data-ttu-id="2a4d3-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2a4d3-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

