---
title: DomainSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bad5399c-0762-4979-9c15-58cf4b7b6278
description: L’élément DomainSetting contient les paramètres de domaine qui sont renvoyées par la requête d’opération GetDomainSettings opération (SOAP).
ms.openlocfilehash: f1c7a30ee221c5f3ca1358d0f3c3aca5c3467159
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756045"
---
# <a name="domainsetting-soap"></a><span data-ttu-id="3602c-103">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3602c-103">DomainSetting (SOAP)</span></span>

<span data-ttu-id="3602c-104">L’élément **DomainSetting** contient les paramètres de domaine qui sont renvoyées par la requête d’opération [GetDomainSettings opération (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="3602c-104">The **DomainSetting** element contains domain settings that are returned by the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<DomainSetting>
   <Name/>
</DomainSetting>
```

 <span data-ttu-id="3602c-105">**DomainSetting**</span><span class="sxs-lookup"><span data-stu-id="3602c-105">**DomainSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3602c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3602c-106">Attributes and elements</span></span>

<span data-ttu-id="3602c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3602c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3602c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3602c-108">Attributes</span></span>

<span data-ttu-id="3602c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3602c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3602c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3602c-110">Child elements</span></span>

|<span data-ttu-id="3602c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3602c-111">**Element**</span></span>|<span data-ttu-id="3602c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3602c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3602c-113">Nom (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3602c-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="3602c-114">Représente le nom d’un paramètre.</span><span class="sxs-lookup"><span data-stu-id="3602c-114">Represents the name of a setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3602c-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3602c-115">Parent elements</span></span>

|<span data-ttu-id="3602c-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3602c-116">**Element**</span></span>|<span data-ttu-id="3602c-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="3602c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3602c-118">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3602c-118">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="3602c-119">Représente les paramètres de domaine qui ont été envoyés dans une requête de découverte automatique ou renvoyés par une réponse de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="3602c-119">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3602c-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3602c-120">Text value</span></span>

<span data-ttu-id="3602c-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3602c-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3602c-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3602c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3602c-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3602c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3602c-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3602c-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3602c-125">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="3602c-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3602c-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3602c-126">Validation File</span></span>  <br/> |<span data-ttu-id="3602c-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3602c-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3602c-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3602c-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="3602c-129">True</span><span class="sxs-lookup"><span data-stu-id="3602c-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3602c-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3602c-130">See also</span></span>

- [<span data-ttu-id="3602c-131">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3602c-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

