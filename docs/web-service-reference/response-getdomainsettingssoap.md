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
description: L’élément Response représente la réponse à un appel GetDomainSettings pour un domaine individuel.
ms.openlocfilehash: 67fe7aea4533058fa0df972e49a2069749dc258b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455582"
---
# <a name="response-getdomainsettings-soap"></a><span data-ttu-id="39efb-103">Réponse (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="39efb-103">Response (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="39efb-104">L’élément **Response** représente la réponse à un appel **GetDomainSettings** pour un domaine individuel.</span><span class="sxs-lookup"><span data-stu-id="39efb-104">The **Response** element represents the response to a **GetDomainSettings** call for an individual domain.</span></span> 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 <span data-ttu-id="39efb-105">**GetDomainSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="39efb-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39efb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="39efb-106">Attributes and elements</span></span>

<span data-ttu-id="39efb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="39efb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39efb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="39efb-108">Attributes</span></span>

<span data-ttu-id="39efb-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="39efb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39efb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="39efb-110">Child elements</span></span>

|<span data-ttu-id="39efb-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="39efb-111">**Element**</span></span>|<span data-ttu-id="39efb-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="39efb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39efb-113">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="39efb-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="39efb-114">Contient la réponse pour chaque domaine demandé dans une demande **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="39efb-114">Contains the response for each domain requested in a **GetDomainSettings** request.</span></span>  <br/> |
|[<span data-ttu-id="39efb-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="39efb-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="39efb-116">Contient le code d’erreur associé à la réponse, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="39efb-116">Contains the error code that is associated with the response, if applicable.</span></span>  <br/> |
|[<span data-ttu-id="39efb-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="39efb-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="39efb-118">Contient le message d’erreur associé à la réponse, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="39efb-118">Contains the error message that is associated with the response, if applicable.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="39efb-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="39efb-119">Parent elements</span></span>

|<span data-ttu-id="39efb-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="39efb-120">**Element**</span></span>|<span data-ttu-id="39efb-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="39efb-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39efb-122">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="39efb-122">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="39efb-123">Renvoie aux paramètres de configuration du domaine de l’appelant.</span><span class="sxs-lookup"><span data-stu-id="39efb-123">Returns to the caller the domain configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="39efb-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="39efb-124">Text value</span></span>

<span data-ttu-id="39efb-125">Aucune.</span><span class="sxs-lookup"><span data-stu-id="39efb-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39efb-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="39efb-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39efb-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="39efb-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="39efb-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="39efb-128">Schema Name</span></span>  <br/> |<span data-ttu-id="39efb-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="39efb-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="39efb-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="39efb-130">Validation File</span></span>  <br/> |<span data-ttu-id="39efb-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="39efb-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="39efb-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="39efb-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="39efb-133">True</span><span class="sxs-lookup"><span data-stu-id="39efb-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="39efb-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="39efb-134">See also</span></span>



[<span data-ttu-id="39efb-135">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="39efb-135">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

