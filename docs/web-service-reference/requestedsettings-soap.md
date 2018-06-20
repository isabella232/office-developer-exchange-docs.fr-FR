---
title: RequestedSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8d713d22-580c-49a5-99f5-ee532443e89a
description: L’élément RequestedSettings contient les noms des paramètres de configuration demandé.
ms.openlocfilehash: 025f86d417ea2041a3247ac67b065d75c8f75599
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829136"
---
# <a name="requestedsettings-soap"></a><span data-ttu-id="d881b-103">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d881b-103">RequestedSettings (SOAP)</span></span>

<span data-ttu-id="d881b-104">L’élément **RequestedSettings** contient les noms des paramètres de configuration demandé.</span><span class="sxs-lookup"><span data-stu-id="d881b-104">The **RequestedSettings** element contains the names of the requested configuration settings.</span></span> 
  
```XML
<RequestedSettings>
   <Setting/>
</RequestedSettings>
```

 <span data-ttu-id="d881b-105">**RequestedSettings**</span><span class="sxs-lookup"><span data-stu-id="d881b-105">**RequestedSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d881b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d881b-106">Attributes and elements</span></span>

<span data-ttu-id="d881b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d881b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d881b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d881b-108">Attributes</span></span>

<span data-ttu-id="d881b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d881b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d881b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d881b-110">Child elements</span></span>

|<span data-ttu-id="d881b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d881b-111">**Element**</span></span>|<span data-ttu-id="d881b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d881b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d881b-113">Paramètre (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d881b-113">Setting (SOAP)</span></span>](setting-soap.md) <br/> |<span data-ttu-id="d881b-114">Représente un paramètre de configuration à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="d881b-114">Represents a configuration setting to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d881b-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d881b-115">Parent elements</span></span>

|<span data-ttu-id="d881b-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d881b-116">**Element**</span></span>|<span data-ttu-id="d881b-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d881b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d881b-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d881b-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="d881b-119">Représente une demande pour récupérer les paramètres spécifiés pour un ou plusieurs utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="d881b-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="d881b-120">Demande (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d881b-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="d881b-121">Contient les paramètres de configuration requise et les utilisateurs cibles.</span><span class="sxs-lookup"><span data-stu-id="d881b-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="d881b-122">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d881b-122">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="d881b-123">Représente une demande [d’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="d881b-123">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="d881b-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d881b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d881b-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d881b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d881b-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d881b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d881b-127">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="d881b-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d881b-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d881b-128">Validation File</span></span>  <br/> |<span data-ttu-id="d881b-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d881b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d881b-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d881b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d881b-131">True</span><span class="sxs-lookup"><span data-stu-id="d881b-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d881b-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d881b-132">See also</span></span>



[<span data-ttu-id="d881b-133">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d881b-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="d881b-134">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d881b-134">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

