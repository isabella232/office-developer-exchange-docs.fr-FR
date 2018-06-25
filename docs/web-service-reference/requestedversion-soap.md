---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: L’élément RequestedVersion spécifie la version minimale de service que le client souhaite le traitement sur la demande.
ms.openlocfilehash: 0d8682c33790d2d26001512ad9e2191ae52074d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829134"
---
# <a name="requestedversion-soap"></a><span data-ttu-id="ea3cb-103">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea3cb-103">RequestedVersion (SOAP)</span></span>

<span data-ttu-id="ea3cb-104">L’élément **RequestedVersion** spécifie la version minimale de service que le client souhaite le traitement sur la demande.</span><span class="sxs-lookup"><span data-stu-id="ea3cb-104">The **RequestedVersion** element specifies the minimum service version that the client wants the request to be processed on.</span></span> 
  
```XML
<RequestedVersion/>
```

 <span data-ttu-id="ea3cb-105">**ExchangeVersion**</span><span class="sxs-lookup"><span data-stu-id="ea3cb-105">**ExchangeVersion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea3cb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ea3cb-106">Attributes and elements</span></span>

<span data-ttu-id="ea3cb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ea3cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea3cb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ea3cb-108">Attributes</span></span>

<span data-ttu-id="ea3cb-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ea3cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea3cb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ea3cb-110">Child elements</span></span>

<span data-ttu-id="ea3cb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ea3cb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ea3cb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ea3cb-112">Parent elements</span></span>

|<span data-ttu-id="ea3cb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ea3cb-113">**Element**</span></span>|<span data-ttu-id="ea3cb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea3cb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea3cb-115">Demande (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea3cb-115">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="ea3cb-116">Contient les paramètres de configuration requise et les utilisateurs cibles.</span><span class="sxs-lookup"><span data-stu-id="ea3cb-116">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="ea3cb-117">Demande (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea3cb-117">Request (GetDomainSettings) (SOAP)</span></span>](request-getdomainsettingssoap.md) <br/> |<span data-ttu-id="ea3cb-118">Représente une demande pour obtenir les paramètres de domaine.</span><span class="sxs-lookup"><span data-stu-id="ea3cb-118">Represents a request to get domain settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ea3cb-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ea3cb-119">Text value</span></span>

<span data-ttu-id="ea3cb-120">La valeur de texte pour l’élément **RequestedVersion** peut être Exchange2010, Exchange2010_SP1, Exchange2010_SP2 ou Exchange2013.</span><span class="sxs-lookup"><span data-stu-id="ea3cb-120">The text value for the **RequestedVersion** element can be Exchange2010, Exchange2010_SP1, Exchange2010_SP2, or Exchange2013.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ea3cb-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="ea3cb-121">Remarks</span></span>

<span data-ttu-id="ea3cb-122">Si cet élément n’est pas présent, la dernière version de service est utilisée.</span><span class="sxs-lookup"><span data-stu-id="ea3cb-122">If this element is not present, the latest service version is used.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea3cb-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ea3cb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea3cb-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ea3cb-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ea3cb-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ea3cb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ea3cb-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ea3cb-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ea3cb-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ea3cb-127">Validation File</span></span>  <br/> |<span data-ttu-id="ea3cb-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ea3cb-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ea3cb-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ea3cb-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea3cb-130">False</span><span class="sxs-lookup"><span data-stu-id="ea3cb-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea3cb-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ea3cb-131">See also</span></span>



[<span data-ttu-id="ea3cb-132">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea3cb-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="ea3cb-133">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea3cb-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

