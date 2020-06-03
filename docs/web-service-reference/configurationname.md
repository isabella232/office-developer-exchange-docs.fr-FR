---
title: ConfigurationName
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
description: L’élément ConfigurationName spécifie les configurations de service demandées par nom.
ms.openlocfilehash: 5e1216253a633af643dbd276827842dbe2db5d5f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463922"
---
# <a name="configurationname"></a><span data-ttu-id="0d574-103">ConfigurationName</span><span class="sxs-lookup"><span data-stu-id="0d574-103">ConfigurationName</span></span>

<span data-ttu-id="0d574-104">L’élément **ConfigurationName** spécifie les configurations de service demandées par nom.</span><span class="sxs-lookup"><span data-stu-id="0d574-104">The **ConfigurationName** element specifies the requested service configurations by name.</span></span> 
  
```xml
<ConfigurationName>MailTips or UnifiedMessagingConfiguration or ProtectionRules</ConfigurationName>
```

 <span data-ttu-id="0d574-105">**ServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="0d574-105">**ServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d574-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0d574-106">Attributes and elements</span></span>

<span data-ttu-id="0d574-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0d574-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d574-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0d574-108">Attributes</span></span>

<span data-ttu-id="0d574-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0d574-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d574-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0d574-110">Child elements</span></span>

<span data-ttu-id="0d574-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0d574-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0d574-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0d574-112">Parent elements</span></span>

|<span data-ttu-id="0d574-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0d574-113">**Element**</span></span>|<span data-ttu-id="0d574-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0d574-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d574-115">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d574-115">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="0d574-116">Contient les configurations de service demandées.</span><span class="sxs-lookup"><span data-stu-id="0d574-116">Contains the requested service configurations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0d574-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0d574-117">Text value</span></span>

<span data-ttu-id="0d574-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **ConfigurationName** .</span><span class="sxs-lookup"><span data-stu-id="0d574-118">The following table lists the possible values for the **ConfigurationName** element.</span></span> 
  
<span data-ttu-id="0d574-119">**Valeurs de l’élément ConfigurationName**</span><span class="sxs-lookup"><span data-stu-id="0d574-119">**ConfigurationName element values**</span></span>

|<span data-ttu-id="0d574-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="0d574-120">**Value**</span></span>|<span data-ttu-id="0d574-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="0d574-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d574-122">MailTips</span><span class="sxs-lookup"><span data-stu-id="0d574-122">MailTips</span></span>  <br/> |<span data-ttu-id="0d574-123">Identifie la configuration du service infos-courrier.</span><span class="sxs-lookup"><span data-stu-id="0d574-123">Identifies the MailTips service configuration.</span></span>  <br/> |
|<span data-ttu-id="0d574-124">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d574-124">UnifiedMessagingConfiguration</span></span>  <br/> |<span data-ttu-id="0d574-125">Identifie la configuration du service de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="0d574-125">Identifies the Unified Messaging service configuration.</span></span>  <br/> |
|<span data-ttu-id="0d574-126">ProtectionRules</span><span class="sxs-lookup"><span data-stu-id="0d574-126">ProtectionRules</span></span>  <br/> |<span data-ttu-id="0d574-127">Identifie la configuration du service des règles de protection.</span><span class="sxs-lookup"><span data-stu-id="0d574-127">Identifies the Protection Rules service configuration.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0d574-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="0d574-128">Remarks</span></span>

<span data-ttu-id="0d574-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d574-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d574-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0d574-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d574-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0d574-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0d574-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0d574-132">Schema Name</span></span>  <br/> |<span data-ttu-id="0d574-133">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0d574-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0d574-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0d574-134">Validation File</span></span>  <br/> |<span data-ttu-id="0d574-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0d574-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0d574-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0d574-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="0d574-137">False</span><span class="sxs-lookup"><span data-stu-id="0d574-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d574-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0d574-138">See also</span></span>



- [<span data-ttu-id="0d574-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0d574-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

