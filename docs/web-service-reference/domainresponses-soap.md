---
title: DomainResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d9c7fd91-22cd-4c72-a841-25cb9d415e0c
description: L’élément DomainResponses contient un tableau de réponses pour les paramètres de chaque domaine demandé.
ms.openlocfilehash: 77a3efc1605337ab436f6aea2b61a67f22e4f8ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756039"
---
# <a name="domainresponses-soap"></a><span data-ttu-id="2ea2f-103">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ea2f-103">DomainResponses (SOAP)</span></span>

<span data-ttu-id="2ea2f-104">L’élément **DomainResponses** contient un tableau de réponses pour les paramètres de chaque domaine demandé.</span><span class="sxs-lookup"><span data-stu-id="2ea2f-104">The **DomainResponses** element contains an array of responses for each requested domain's settings.</span></span> 
  
```XML
<DomainResponses>
   <DomainResponse/>
</DomainResponses>
```

 <span data-ttu-id="2ea2f-105">**ArrayOfDomainResponse**</span><span class="sxs-lookup"><span data-stu-id="2ea2f-105">**ArrayOfDomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ea2f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2ea2f-106">Attributes and elements</span></span>

<span data-ttu-id="2ea2f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2ea2f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ea2f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2ea2f-108">Attributes</span></span>

<span data-ttu-id="2ea2f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ea2f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ea2f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2ea2f-110">Child elements</span></span>

|<span data-ttu-id="2ea2f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ea2f-111">**Element**</span></span>|<span data-ttu-id="2ea2f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ea2f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ea2f-113">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ea2f-113">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="2ea2f-114">Contient les paramètres requis pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="2ea2f-114">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2ea2f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2ea2f-115">Parent elements</span></span>

|<span data-ttu-id="2ea2f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ea2f-116">**Element**</span></span>|<span data-ttu-id="2ea2f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ea2f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ea2f-118">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ea2f-118">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="2ea2f-119">Représente la réponse à une demande de [l’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) pour un domaine et renvoie les paramètres de domaine.</span><span class="sxs-lookup"><span data-stu-id="2ea2f-119">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request for a domain, and returns the domain settings.</span></span>  <br/> |
|[<span data-ttu-id="2ea2f-120">Réponse (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ea2f-120">Response (GetDomainSettings) (SOAP)</span></span>](response-getdomainsettingssoap.md) <br/> |<span data-ttu-id="2ea2f-121">Représente la réponse à un appel de [l’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) pour un domaine spécifique.</span><span class="sxs-lookup"><span data-stu-id="2ea2f-121">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ea2f-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2ea2f-122">Text value</span></span>

<span data-ttu-id="2ea2f-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ea2f-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ea2f-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2ea2f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ea2f-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2ea2f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2ea2f-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2ea2f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="2ea2f-127">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="2ea2f-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2ea2f-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2ea2f-128">Validation File</span></span>  <br/> |<span data-ttu-id="2ea2f-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2ea2f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2ea2f-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2ea2f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ea2f-131">True</span><span class="sxs-lookup"><span data-stu-id="2ea2f-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ea2f-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2ea2f-132">See also</span></span>

- [<span data-ttu-id="2ea2f-133">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ea2f-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

