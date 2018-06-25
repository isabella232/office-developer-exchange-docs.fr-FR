---
title: Domaine (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 849629a0-0467-422f-88f6-3b8a95c17bba
description: L’élément de domaine contient un domaine fédéré dans une réponse GetFederationInformation ou un domaine pour lequel les paramètres de configuration sont demandées dans une requête GetDomainSettings.
ms.openlocfilehash: 411ca866800322ef06eeecc2ab92adc6f711917c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756029"
---
# <a name="domain-soap"></a><span data-ttu-id="4d33e-103">Domaine (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4d33e-103">Domain (SOAP)</span></span>

<span data-ttu-id="4d33e-104">L’élément de **domaine** contient un domaine fédéré dans une réponse **GetFederationInformation** ou un domaine pour lequel les paramètres de configuration sont demandées dans une requête **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="4d33e-104">The **Domain** element contains a federated domain in a **GetFederationInformation** response or contains a domain the configuration settings for which are requested in a **GetDomainSettings** request.</span></span> 
  
```XML
<Domain/> 
```

 <span data-ttu-id="4d33e-105">**string**</span><span class="sxs-lookup"><span data-stu-id="4d33e-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d33e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4d33e-106">Attributes and elements</span></span>

<span data-ttu-id="4d33e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4d33e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d33e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4d33e-108">Attributes</span></span>

<span data-ttu-id="4d33e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d33e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d33e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4d33e-110">Child elements</span></span>

<span data-ttu-id="4d33e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d33e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4d33e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4d33e-112">Parent elements</span></span>

|<span data-ttu-id="4d33e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4d33e-113">**Element**</span></span>|<span data-ttu-id="4d33e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d33e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d33e-115">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4d33e-115">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="4d33e-116">Représente les domaines pour lesquels les paramètres de configuration sont retournés dans une opération **GetDomainSettings** ou les domaines que l’organisation a fédérés dans une opération **GetFederationInformation** .</span><span class="sxs-lookup"><span data-stu-id="4d33e-116">Represents the domains the configuration settings for which are returned in a **GetDomainSettings** operation or the domains that the organization has federated in a **GetFederationInformation** operation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4d33e-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4d33e-117">Text value</span></span>

<span data-ttu-id="4d33e-118">La valeur de texte de l’élément de **domaine** représente un nom de domaine.</span><span class="sxs-lookup"><span data-stu-id="4d33e-118">The text value of the **Domain** element represents a domain name.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="4d33e-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4d33e-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d33e-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4d33e-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4d33e-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4d33e-121">Schema Name</span></span>  <br/> |<span data-ttu-id="4d33e-122">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="4d33e-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4d33e-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4d33e-123">Validation File</span></span>  <br/> |<span data-ttu-id="4d33e-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4d33e-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4d33e-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4d33e-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d33e-126">True</span><span class="sxs-lookup"><span data-stu-id="4d33e-126">True</span></span>  <br/> |
   

