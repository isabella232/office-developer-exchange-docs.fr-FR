---
title: RequestedConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestedConfiguration
api_type:
- schema
ms.assetid: 24921387-f676-49e6-8d7a-ef3115024866
description: L’élément RequestedConfiguration contient les configurations de service demandé.
ms.openlocfilehash: 1edc6394360250c9a9810fe614c975cb48eba3f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829130"
---
# <a name="requestedconfiguration"></a><span data-ttu-id="067fa-103">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="067fa-103">RequestedConfiguration</span></span>

<span data-ttu-id="067fa-104">L’élément **RequestedConfiguration** contient les configurations de service demandé.</span><span class="sxs-lookup"><span data-stu-id="067fa-104">The **RequestedConfiguration** element contains the requested service configurations.</span></span> 
  
```XML
<RequestedConfiguration>
   <ConfigurationName/>
</RequestedConfiguration>
```

 <span data-ttu-id="067fa-105">**ArrayOfServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="067fa-105">**ArrayOfServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="067fa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="067fa-106">Attributes and elements</span></span>

<span data-ttu-id="067fa-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="067fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="067fa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="067fa-108">Attributes</span></span>

<span data-ttu-id="067fa-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="067fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="067fa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="067fa-110">Child elements</span></span>

|<span data-ttu-id="067fa-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="067fa-111">**Element**</span></span>|<span data-ttu-id="067fa-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="067fa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="067fa-113">Nom de configuration</span><span class="sxs-lookup"><span data-stu-id="067fa-113">ConfigurationName</span></span>](configurationname.md) <br/> |<span data-ttu-id="067fa-114">Spécifie les configurations de service demandé par son nom.</span><span class="sxs-lookup"><span data-stu-id="067fa-114">Specifies the requested service configurations by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="067fa-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="067fa-115">Parent elements</span></span>

|<span data-ttu-id="067fa-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="067fa-116">**Element**</span></span>|<span data-ttu-id="067fa-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="067fa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="067fa-118">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="067fa-118">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="067fa-119">Définit une demande GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="067fa-119">Defines a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="067fa-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="067fa-120">Text value</span></span>

<span data-ttu-id="067fa-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="067fa-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="067fa-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="067fa-122">Remarks</span></span>

<span data-ttu-id="067fa-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="067fa-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="067fa-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="067fa-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="067fa-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="067fa-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="067fa-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="067fa-126">Schema Name</span></span>  <br/> |<span data-ttu-id="067fa-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="067fa-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="067fa-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="067fa-128">Validation File</span></span>  <br/> |<span data-ttu-id="067fa-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="067fa-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="067fa-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="067fa-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="067fa-131">False</span><span class="sxs-lookup"><span data-stu-id="067fa-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="067fa-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="067fa-132">See also</span></span>



- [<span data-ttu-id="067fa-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="067fa-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

