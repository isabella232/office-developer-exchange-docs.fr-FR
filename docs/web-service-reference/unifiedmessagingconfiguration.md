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
description: L’élément UnifiedMessagingConfiguration contient les informations de configuration de service pour le service de messagerie unifiée.
ms.openlocfilehash: 3f9f4ed65721929c552615c07e2239f48ef837f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528691"
---
# <a name="unifiedmessagingconfiguration"></a><span data-ttu-id="26a7d-103">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="26a7d-103">UnifiedMessagingConfiguration</span></span>

<span data-ttu-id="26a7d-104">L’élément **UnifiedMessagingConfiguration** contient les informations de configuration de service pour le service de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="26a7d-104">The **UnifiedMessagingConfiguration** element contains service configuration information for the Unified Messaging service.</span></span> 
  
```XML
<UnifiedMessagingConfiguration>
   <UmEnabled/>
   <PlayOnPhoneDialString/>
   <PlayOnPhoneEnabled/>
</UnifiedMessagingConfiguration>
```

 <span data-ttu-id="26a7d-105">**UnifiedMessageServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="26a7d-105">**UnifiedMessageServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26a7d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="26a7d-106">Attributes and elements</span></span>

<span data-ttu-id="26a7d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="26a7d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26a7d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="26a7d-108">Attributes</span></span>

<span data-ttu-id="26a7d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="26a7d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26a7d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="26a7d-110">Child elements</span></span>

|<span data-ttu-id="26a7d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="26a7d-111">**Element**</span></span>|<span data-ttu-id="26a7d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="26a7d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26a7d-113">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="26a7d-113">UmEnabled</span></span>](umenabled.md) <br/> |<span data-ttu-id="26a7d-114">Indique si la messagerie unifiée est activée pour un compte.</span><span class="sxs-lookup"><span data-stu-id="26a7d-114">Indicates whether Unified Messaging is enabled for an account.</span></span> <span data-ttu-id="26a7d-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="26a7d-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="26a7d-116">PlayOnPhoneDialString (services Web Exchange)</span><span class="sxs-lookup"><span data-stu-id="26a7d-116">PlayOnPhoneDialString (Exchange Web Services)</span></span>](playonphonedialstring-exchange-web-services.md) <br/> |<span data-ttu-id="26a7d-117">Identifie la chaîne de numérotation d’émission sur téléphone.</span><span class="sxs-lookup"><span data-stu-id="26a7d-117">Identifies the Play-on-Phone dial string.</span></span> <span data-ttu-id="26a7d-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="26a7d-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="26a7d-119">PlayOnPhoneEnabled</span><span class="sxs-lookup"><span data-stu-id="26a7d-119">PlayOnPhoneEnabled</span></span>](playonphoneenabled.md) <br/> |<span data-ttu-id="26a7d-120">Indique si la fonctionnalité d’émission sur téléphone est activée.</span><span class="sxs-lookup"><span data-stu-id="26a7d-120">Indicates whether the Play-on-Phone feature is enabled.</span></span> <span data-ttu-id="26a7d-121">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="26a7d-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="26a7d-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="26a7d-122">Parent elements</span></span>

|<span data-ttu-id="26a7d-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="26a7d-123">**Element**</span></span>|<span data-ttu-id="26a7d-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="26a7d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26a7d-125">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="26a7d-125">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="26a7d-126">Contient les paramètres de configuration du service.</span><span class="sxs-lookup"><span data-stu-id="26a7d-126">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="26a7d-127">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="26a7d-127">Text value</span></span>

<span data-ttu-id="26a7d-128">Aucun.</span><span class="sxs-lookup"><span data-stu-id="26a7d-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="26a7d-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="26a7d-129">Remarks</span></span>

<span data-ttu-id="26a7d-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="26a7d-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26a7d-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="26a7d-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26a7d-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="26a7d-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26a7d-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="26a7d-133">Schema Name</span></span>  <br/> |<span data-ttu-id="26a7d-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="26a7d-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="26a7d-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="26a7d-135">Validation File</span></span>  <br/> |<span data-ttu-id="26a7d-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="26a7d-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26a7d-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="26a7d-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="26a7d-138">False</span><span class="sxs-lookup"><span data-stu-id="26a7d-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26a7d-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="26a7d-139">See also</span></span>



- [<span data-ttu-id="26a7d-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="26a7d-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

