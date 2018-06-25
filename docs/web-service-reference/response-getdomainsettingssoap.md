---
title: Réponse (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a5b052df-93bd-4fe1-ac30-83de9a3dfcd7
description: L’élément de réponse représente la réponse à un appel GetDomainSettings pour un domaine spécifique.
ms.openlocfilehash: 316d77104894cf5ed9121e7dab1c38646765c948
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829169"
---
# <a name="response-getdomainsettings-soap"></a><span data-ttu-id="fe637-103">Réponse (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe637-103">Response (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="fe637-104">L’élément de **réponse** représente la réponse à un appel **GetDomainSettings** pour un domaine spécifique.</span><span class="sxs-lookup"><span data-stu-id="fe637-104">The **Response** element represents the response to a **GetDomainSettings** call for an individual domain.</span></span> 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 <span data-ttu-id="fe637-105">**GetDomainSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="fe637-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fe637-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fe637-106">Attributes and elements</span></span>

<span data-ttu-id="fe637-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fe637-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe637-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fe637-108">Attributes</span></span>

<span data-ttu-id="fe637-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fe637-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe637-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fe637-110">Child elements</span></span>

|<span data-ttu-id="fe637-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fe637-111">**Element**</span></span>|<span data-ttu-id="fe637-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe637-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe637-113">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe637-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="fe637-114">Contient la réponse de chaque domaine demandé dans une requête **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="fe637-114">Contains the response for each domain requested in a **GetDomainSettings** request.</span></span>  <br/> |
|[<span data-ttu-id="fe637-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe637-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="fe637-116">Contient le code d’erreur qui est associé à la réponse, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="fe637-116">Contains the error code that is associated with the response, if applicable.</span></span>  <br/> |
|[<span data-ttu-id="fe637-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe637-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="fe637-118">Contient le message d’erreur qui est associé à la réponse, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="fe637-118">Contains the error message that is associated with the response, if applicable.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fe637-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fe637-119">Parent elements</span></span>

|<span data-ttu-id="fe637-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fe637-120">**Element**</span></span>|<span data-ttu-id="fe637-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe637-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe637-122">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe637-122">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="fe637-123">Retourne à l’appelant le domaine de paramètres de configuration.</span><span class="sxs-lookup"><span data-stu-id="fe637-123">Returns to the caller the domain configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fe637-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="fe637-124">Text value</span></span>

<span data-ttu-id="fe637-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fe637-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe637-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fe637-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe637-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fe637-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="fe637-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fe637-128">Schema Name</span></span>  <br/> |<span data-ttu-id="fe637-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="fe637-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="fe637-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fe637-130">Validation File</span></span>  <br/> |<span data-ttu-id="fe637-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fe637-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fe637-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fe637-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="fe637-133">True</span><span class="sxs-lookup"><span data-stu-id="fe637-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe637-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fe637-134">See also</span></span>



[<span data-ttu-id="fe637-135">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe637-135">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

