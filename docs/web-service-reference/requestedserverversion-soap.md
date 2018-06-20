---
title: RequestedServerVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cf3f9d7a-2add-4457-b009-2929220f90b5
description: L’élément RequestedServerVersion spécifie la version du serveur une méthode de découverte automatique cibles d’appels.
ms.openlocfilehash: 6b9d31f3b7bca087652f04e4943becc5ac4e68e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829132"
---
# <a name="requestedserverversion-soap"></a><span data-ttu-id="ba523-103">RequestedServerVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ba523-103">RequestedServerVersion (SOAP)</span></span>

<span data-ttu-id="ba523-104">L’élément **RequestedServerVersion** spécifie la version du serveur une méthode de **découverte automatique** cibles d’appels.</span><span class="sxs-lookup"><span data-stu-id="ba523-104">The **RequestedServerVersion** element specifies the server version that an **Autodiscover** method call targets.</span></span> 
  
```XML
<RequestedServerVersion/>
```

 <span data-ttu-id="ba523-105">**ExchangeVersion**</span><span class="sxs-lookup"><span data-stu-id="ba523-105">**ExchangeVersion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba523-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ba523-106">Attributes and elements</span></span>

<span data-ttu-id="ba523-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ba523-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba523-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ba523-108">Attributes</span></span>

<span data-ttu-id="ba523-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba523-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba523-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ba523-110">Child elements</span></span>

<span data-ttu-id="ba523-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba523-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba523-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ba523-112">Parent elements</span></span>

<span data-ttu-id="ba523-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba523-113">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ba523-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ba523-114">Text value</span></span>

<span data-ttu-id="ba523-115">La valeur de texte de l’élément **RequestedServerVersion** spécifie la version du serveur une méthode de **découverte automatique** cibles d’appels.</span><span class="sxs-lookup"><span data-stu-id="ba523-115">The text value of the **RequestedServerVersion** element specifies the server version that an **Autodiscover** method call targets.</span></span> <span data-ttu-id="ba523-116">Le tableau suivant répertorie les versions de serveur valide.</span><span class="sxs-lookup"><span data-stu-id="ba523-116">The following table lists the valid server versions.</span></span> 
  
|<span data-ttu-id="ba523-117">**Valeur texte**</span><span class="sxs-lookup"><span data-stu-id="ba523-117">**Text value**</span></span>|<span data-ttu-id="ba523-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba523-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ba523-119">Exchange2007_SP1</span><span class="sxs-lookup"><span data-stu-id="ba523-119">Exchange2007_SP1</span></span>  <br/> |<span data-ttu-id="ba523-120">Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ba523-120">Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|<span data-ttu-id="ba523-121">Exchange2010</span><span class="sxs-lookup"><span data-stu-id="ba523-121">Exchange2010</span></span>  <br/> |<span data-ttu-id="ba523-122">Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="ba523-122">Exchange Server 2010.</span></span>  <br/> |
|<span data-ttu-id="ba523-123">Exchange2010_SP1</span><span class="sxs-lookup"><span data-stu-id="ba523-123">Exchange2010_SP1</span></span>  <br/> |<span data-ttu-id="ba523-124">Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ba523-124">Exchange Server 2010 Service Pack 1 (SP1).</span></span>  <br/> |
|<span data-ttu-id="ba523-125">Exchange2010_SP2</span><span class="sxs-lookup"><span data-stu-id="ba523-125">Exchange2010_SP2</span></span>  <br/> |<span data-ttu-id="ba523-126">Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="ba523-126">Exchange Server 2010 Service Pack 2 (SP2).</span></span>  <br/> |
|<span data-ttu-id="ba523-127">Exchange2013</span><span class="sxs-lookup"><span data-stu-id="ba523-127">Exchange2013</span></span>  <br/> |<span data-ttu-id="ba523-128">Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ba523-128">Exchange Server 2013.</span></span> <span data-ttu-id="ba523-129">Le champ Exchange2013 est applicable pour les clients qui ciblent Exchange Online et versions d’Exchange commençant par Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ba523-129">The Exchange2013 field is applicable for clients that target Exchange Online and versions of Exchange starting with Exchange Server 2013.</span></span>  <br/> |
|<span data-ttu-id="ba523-130">Exchange2013_SP1</span><span class="sxs-lookup"><span data-stu-id="ba523-130">Exchange2013_SP1</span></span>  <br/> |<span data-ttu-id="ba523-131">Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ba523-131">Exchange Server 2013 Service Pack 1 (SP1).</span></span> <span data-ttu-id="ba523-132">Le champ Exchange2013_SP1 est applicable pour les clients qui ciblent Exchange Online et versions d’Exchange commençant par Exchange Server 2013 SP1.</span><span class="sxs-lookup"><span data-stu-id="ba523-132">The Exchange2013_SP1 field is applicable for clients that target Exchange Online and versions of Exchange starting with Exchange Server 2013 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ba523-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="ba523-133">Remarks</span></span>

<span data-ttu-id="ba523-134">L’élément **RequestedServerVersion** est définie dans l’en-tête SOAP.</span><span class="sxs-lookup"><span data-stu-id="ba523-134">The **RequestedServerVersion** element is set in the SOAP header.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ba523-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ba523-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba523-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ba523-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ba523-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ba523-137">Schema Name</span></span>  <br/> |<span data-ttu-id="ba523-138">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ba523-138">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ba523-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ba523-139">Validation File</span></span>  <br/> |<span data-ttu-id="ba523-140">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ba523-140">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ba523-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ba523-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba523-142">True</span><span class="sxs-lookup"><span data-stu-id="ba523-142">True</span></span>  <br/> |
   

