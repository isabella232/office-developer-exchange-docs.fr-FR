---
title: GetDomainSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5ac0ff6d-9e02-4e4c-973d-cd9e076661d5
description: L’élément GetDomainSettingsRequest représente une demande d’opération GetDomainSettings opération (SOAP).
ms.openlocfilehash: 4de525a9ba47a0d9afb0d6db9200fe32845f31d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756581"
---
# <a name="getdomainsettingsrequest-soap"></a><span data-ttu-id="1d0f8-103">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1d0f8-103">GetDomainSettingsRequest (SOAP)</span></span>

<span data-ttu-id="1d0f8-104">L’élément **GetDomainSettingsRequest** représente une demande d’opération [GetDomainSettings opération (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="1d0f8-104">The **GetDomainSettingsRequest** element represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<GetDomainSettingsRequest>
   <Domains/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetDomainSettingsRequest>
```

 <span data-ttu-id="1d0f8-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="1d0f8-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d0f8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1d0f8-106">Attributes and elements</span></span>

<span data-ttu-id="1d0f8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1d0f8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d0f8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1d0f8-108">Attributes</span></span>

<span data-ttu-id="1d0f8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1d0f8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d0f8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1d0f8-110">Child elements</span></span>

|<span data-ttu-id="1d0f8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1d0f8-111">**Element**</span></span>|<span data-ttu-id="1d0f8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1d0f8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d0f8-113">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1d0f8-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="1d0f8-114">Représente une collection d’identificateurs de domaine.</span><span class="sxs-lookup"><span data-stu-id="1d0f8-114">Represents a collection of domain identifiers.</span></span>  <br/> |
|[<span data-ttu-id="1d0f8-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1d0f8-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="1d0f8-116">Contient les noms des paramètres de configuration du domaine demandé.</span><span class="sxs-lookup"><span data-stu-id="1d0f8-116">Contains the names of the requested domain configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="1d0f8-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1d0f8-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="1d0f8-118">Spécifie la version du serveur qui utilise le fournisseur.</span><span class="sxs-lookup"><span data-stu-id="1d0f8-118">Specifies the server version that the provider will use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d0f8-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1d0f8-119">Parent elements</span></span>

<span data-ttu-id="1d0f8-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1d0f8-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="1d0f8-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1d0f8-121">Text value</span></span>

<span data-ttu-id="1d0f8-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1d0f8-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d0f8-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1d0f8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d0f8-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1d0f8-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1d0f8-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1d0f8-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1d0f8-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="1d0f8-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1d0f8-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1d0f8-127">Validation File</span></span>  <br/> |<span data-ttu-id="1d0f8-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1d0f8-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1d0f8-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1d0f8-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d0f8-130">True</span><span class="sxs-lookup"><span data-stu-id="1d0f8-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d0f8-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1d0f8-131">See also</span></span>



[<span data-ttu-id="1d0f8-132">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1d0f8-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

