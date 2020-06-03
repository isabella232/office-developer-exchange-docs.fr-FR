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
description: L’élément RequestedConfiguration contient les configurations de service demandées.
ms.openlocfilehash: bbc503e6d6f7c56c785365924106bc2468965d0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457150"
---
# <a name="requestedconfiguration"></a><span data-ttu-id="2f622-103">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f622-103">RequestedConfiguration</span></span>

<span data-ttu-id="2f622-104">L’élément **RequestedConfiguration** contient les configurations de service demandées.</span><span class="sxs-lookup"><span data-stu-id="2f622-104">The **RequestedConfiguration** element contains the requested service configurations.</span></span> 
  
```XML
<RequestedConfiguration>
   <ConfigurationName/>
</RequestedConfiguration>
```

 <span data-ttu-id="2f622-105">**ArrayOfServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="2f622-105">**ArrayOfServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f622-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2f622-106">Attributes and elements</span></span>

<span data-ttu-id="2f622-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2f622-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f622-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2f622-108">Attributes</span></span>

<span data-ttu-id="2f622-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2f622-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f622-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2f622-110">Child elements</span></span>

|<span data-ttu-id="2f622-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2f622-111">**Element**</span></span>|<span data-ttu-id="2f622-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2f622-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f622-113">ConfigurationName</span><span class="sxs-lookup"><span data-stu-id="2f622-113">ConfigurationName</span></span>](configurationname.md) <br/> |<span data-ttu-id="2f622-114">Spécifie les configurations de service demandées par nom.</span><span class="sxs-lookup"><span data-stu-id="2f622-114">Specifies the requested service configurations by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2f622-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2f622-115">Parent elements</span></span>

|<span data-ttu-id="2f622-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2f622-116">**Element**</span></span>|<span data-ttu-id="2f622-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="2f622-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f622-118">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f622-118">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="2f622-119">Définit une requête GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f622-119">Defines a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2f622-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2f622-120">Text value</span></span>

<span data-ttu-id="2f622-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2f622-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2f622-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="2f622-122">Remarks</span></span>

<span data-ttu-id="2f622-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f622-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f622-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2f622-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f622-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2f622-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2f622-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2f622-126">Schema Name</span></span>  <br/> |<span data-ttu-id="2f622-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="2f622-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2f622-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2f622-128">Validation File</span></span>  <br/> |<span data-ttu-id="2f622-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2f622-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2f622-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2f622-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="2f622-131">False</span><span class="sxs-lookup"><span data-stu-id="2f622-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f622-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2f622-132">See also</span></span>



- [<span data-ttu-id="2f622-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2f622-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

