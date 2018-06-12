---
title: InPlaceHoldConfigurationOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 921ecc73-b7e2-40a7-8458-68f18dd5a13b
description: L’élément InPlaceHoldConfigurationOnly Spécifie si pour inclure le blocage sur place configuration.
ms.openlocfilehash: 3ad020a10e43d8f54e3d603906c856e01b1956eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827934"
---
# <a name="inplaceholdconfigurationonly"></a><span data-ttu-id="46e9b-103">InPlaceHoldConfigurationOnly</span><span class="sxs-lookup"><span data-stu-id="46e9b-103">InPlaceHoldConfigurationOnly</span></span>

<span data-ttu-id="46e9b-104">L’élément **InPlaceHoldConfigurationOnly** Spécifie si pour inclure le blocage sur place configuration.</span><span class="sxs-lookup"><span data-stu-id="46e9b-104">The **InPlaceHoldConfigurationOnly** element specifies whether to include the in-place hold configuration.</span></span> 
  
```XML
<InPlaceHoldConfigurationOnly>true | false</InPlaceHoldConfigurationOnly>
```

 <span data-ttu-id="46e9b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="46e9b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46e9b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="46e9b-106">Attributes and elements</span></span>

<span data-ttu-id="46e9b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="46e9b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46e9b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="46e9b-108">Attributes</span></span>

<span data-ttu-id="46e9b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="46e9b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46e9b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="46e9b-110">Child elements</span></span>

<span data-ttu-id="46e9b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="46e9b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="46e9b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="46e9b-112">Parent elements</span></span>

[<span data-ttu-id="46e9b-113">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="46e9b-113">GetDiscoverySearchConfiguration</span></span>](getdiscoverysearchconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="46e9b-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="46e9b-114">Text value</span></span>

<span data-ttu-id="46e9b-115">Une valeur de texte de **la valeur true** pour l’élément **InPlaceHoldConfigurationOnly** indique que la configuration dans une archive permanente est incluse.</span><span class="sxs-lookup"><span data-stu-id="46e9b-115">A text value of **true** for the **InPlaceHoldConfigurationOnly** element indicates that the in-place hold configuration is included.</span></span> <span data-ttu-id="46e9b-116">La valeur **false** indique que la configuration dans une archive permanente n’est pas incluse.</span><span class="sxs-lookup"><span data-stu-id="46e9b-116">A value of **false** indicates that the in-place hold configuration is not included.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="46e9b-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="46e9b-117">Remarks</span></span>

<span data-ttu-id="46e9b-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="46e9b-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="46e9b-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="46e9b-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46e9b-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="46e9b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46e9b-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="46e9b-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="46e9b-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="46e9b-122">Schema name</span></span>  <br/> |<span data-ttu-id="46e9b-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="46e9b-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="46e9b-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="46e9b-124">Validation file</span></span>  <br/> |<span data-ttu-id="46e9b-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="46e9b-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="46e9b-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="46e9b-126">Can be empty</span></span>  <br/> ||
   

