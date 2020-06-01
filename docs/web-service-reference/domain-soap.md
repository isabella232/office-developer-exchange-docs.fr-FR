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
description: L’élément Domain contient un domaine fédéré dans une réponse GetFederationInformation ou contient un domaine dont les paramètres de configuration sont demandés dans une demande GetDomainSettings.
ms.openlocfilehash: f90c608ee1fc3356a227bca6411eaeff0c1e8b22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456982"
---
# <a name="domain-soap"></a><span data-ttu-id="d02f4-103">Domaine (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d02f4-103">Domain (SOAP)</span></span>

<span data-ttu-id="d02f4-104">L’élément **Domain** contient un domaine fédéré dans une réponse **GetFederationInformation** ou contient un domaine dont les paramètres de configuration sont demandés dans une demande **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="d02f4-104">The **Domain** element contains a federated domain in a **GetFederationInformation** response or contains a domain the configuration settings for which are requested in a **GetDomainSettings** request.</span></span> 
  
```XML
<Domain/> 
```

 <span data-ttu-id="d02f4-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="d02f4-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d02f4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d02f4-106">Attributes and elements</span></span>

<span data-ttu-id="d02f4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d02f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d02f4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d02f4-108">Attributes</span></span>

<span data-ttu-id="d02f4-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d02f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d02f4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d02f4-110">Child elements</span></span>

<span data-ttu-id="d02f4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d02f4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d02f4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d02f4-112">Parent elements</span></span>

|<span data-ttu-id="d02f4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d02f4-113">**Element**</span></span>|<span data-ttu-id="d02f4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d02f4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d02f4-115">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d02f4-115">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="d02f4-116">Représente les domaines pour lesquels les paramètres de configuration sont renvoyés dans une opération **GetDomainSettings** ou les domaines que l’organisation a fédérés dans une opération **GetFederationInformation** .</span><span class="sxs-lookup"><span data-stu-id="d02f4-116">Represents the domains the configuration settings for which are returned in a **GetDomainSettings** operation or the domains that the organization has federated in a **GetFederationInformation** operation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d02f4-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="d02f4-117">Text value</span></span>

<span data-ttu-id="d02f4-118">La valeur de texte de l’élément de **domaine** représente un nom de domaine.</span><span class="sxs-lookup"><span data-stu-id="d02f4-118">The text value of the **Domain** element represents a domain name.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d02f4-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d02f4-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d02f4-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d02f4-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d02f4-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d02f4-121">Schema Name</span></span>  <br/> |<span data-ttu-id="d02f4-122">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="d02f4-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d02f4-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d02f4-123">Validation File</span></span>  <br/> |<span data-ttu-id="d02f4-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d02f4-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d02f4-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d02f4-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="d02f4-126">True</span><span class="sxs-lookup"><span data-stu-id="d02f4-126">True</span></span>  <br/> |
   

