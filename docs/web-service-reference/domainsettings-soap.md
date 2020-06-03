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
description: L’élément DomainSettings représente les paramètres de domaine qui ont été envoyés dans une demande de découverte automatique ou renvoyés par une réponse de découverte automatique.
ms.openlocfilehash: 67e3753b0cf5c7c653664ff087f697ce7ae2b7a4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530697"
---
# <a name="domainsettings-soap"></a><span data-ttu-id="356d0-103">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="356d0-103">DomainSettings (SOAP)</span></span>

<span data-ttu-id="356d0-104">L’élément **DomainSettings** représente les paramètres de domaine qui ont été envoyés dans une demande de découverte automatique ou renvoyés par une réponse de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="356d0-104">The **DomainSettings** element represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span> 
  
```XML
<DomainSettings>
   <DomainSetting/>
</DomainSettings>
```

 <span data-ttu-id="356d0-105">**DomainSettings**</span><span class="sxs-lookup"><span data-stu-id="356d0-105">**DomainSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="356d0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="356d0-106">Attributes and elements</span></span>

<span data-ttu-id="356d0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="356d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="356d0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="356d0-108">Attributes</span></span>

<span data-ttu-id="356d0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="356d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="356d0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="356d0-110">Child elements</span></span>

|<span data-ttu-id="356d0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="356d0-111">**Element**</span></span>|<span data-ttu-id="356d0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="356d0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="356d0-113">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="356d0-113">DomainSetting (SOAP)</span></span>](domainsetting-soap.md) <br/> |<span data-ttu-id="356d0-114">Contient les paramètres de domaine qui sont renvoyés par une demande [SOAP (GetDomainSettings Operation)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="356d0-114">Contains domain settings that are returned by a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="356d0-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="356d0-115">Parent elements</span></span>

|<span data-ttu-id="356d0-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="356d0-116">**Element**</span></span>|<span data-ttu-id="356d0-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="356d0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="356d0-118">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="356d0-118">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="356d0-119">Contient les paramètres demandés pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="356d0-119">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="356d0-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="356d0-120">Text value</span></span>

<span data-ttu-id="356d0-121">Aucune.</span><span class="sxs-lookup"><span data-stu-id="356d0-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="356d0-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="356d0-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="356d0-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="356d0-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="356d0-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="356d0-124">Schema Name</span></span>  <br/> |<span data-ttu-id="356d0-125">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="356d0-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="356d0-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="356d0-126">Validation File</span></span>  <br/> |<span data-ttu-id="356d0-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="356d0-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="356d0-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="356d0-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="356d0-129">True</span><span class="sxs-lookup"><span data-stu-id="356d0-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="356d0-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="356d0-130">See also</span></span>

- [<span data-ttu-id="356d0-131">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="356d0-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

