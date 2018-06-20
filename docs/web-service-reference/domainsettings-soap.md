---
title: DomainSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f3d37f5a-c9ea-4ed9-a011-94d33bda64d1
description: L’élément DomainSettings représente les paramètres de domaine qui ont été envoyés dans une requête de découverte automatique ou renvoyés par une réponse de découverte automatique.
ms.openlocfilehash: 961051399dc8babd8cba6eeaf43456071d0f40a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756050"
---
# <a name="domainsettings-soap"></a><span data-ttu-id="ec075-103">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec075-103">DomainSettings (SOAP)</span></span>

<span data-ttu-id="ec075-104">L’élément **DomainSettings** représente les paramètres de domaine qui ont été envoyés dans une requête de découverte automatique ou renvoyés par une réponse de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="ec075-104">The **DomainSettings** element represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span> 
  
```XML
<DomainSettings>
   <DomainSetting/>
</DomainSettings>
```

 <span data-ttu-id="ec075-105">**DomainSettings**</span><span class="sxs-lookup"><span data-stu-id="ec075-105">**DomainSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec075-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ec075-106">Attributes and elements</span></span>

<span data-ttu-id="ec075-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ec075-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec075-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ec075-108">Attributes</span></span>

<span data-ttu-id="ec075-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ec075-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec075-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ec075-110">Child elements</span></span>

|<span data-ttu-id="ec075-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ec075-111">**Element**</span></span>|<span data-ttu-id="ec075-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec075-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec075-113">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec075-113">DomainSetting (SOAP)</span></span>](domainsetting-soap.md) <br/> |<span data-ttu-id="ec075-114">Contient les paramètres de domaine qui sont renvoyées par une demande [d’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="ec075-114">Contains domain settings that are returned by a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec075-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ec075-115">Parent elements</span></span>

|<span data-ttu-id="ec075-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ec075-116">**Element**</span></span>|<span data-ttu-id="ec075-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec075-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec075-118">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec075-118">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="ec075-119">Contient les paramètres requis pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="ec075-119">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ec075-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ec075-120">Text value</span></span>

<span data-ttu-id="ec075-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ec075-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec075-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ec075-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec075-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ec075-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ec075-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ec075-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ec075-125">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ec075-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ec075-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ec075-126">Validation File</span></span>  <br/> |<span data-ttu-id="ec075-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ec075-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ec075-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ec075-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec075-129">True</span><span class="sxs-lookup"><span data-stu-id="ec075-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec075-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ec075-130">See also</span></span>

- [<span data-ttu-id="ec075-131">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec075-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

