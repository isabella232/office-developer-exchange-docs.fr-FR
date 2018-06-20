---
title: DomainSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a4ce19de-f560-4984-8047-ecbbc86c9b91
description: L’élément DomainSettingsErrors contient des informations d’erreur pour les paramètres qui ne peut pas être retourné.
ms.openlocfilehash: 6ecd23bc556ca32d724581a28cc7c117c6853207
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756049"
---
# <a name="domainsettingerrors-soap"></a><span data-ttu-id="4dec6-103">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4dec6-103">DomainSettingErrors (SOAP)</span></span>

<span data-ttu-id="4dec6-104">L’élément **DomainSettingsErrors** contient des informations d’erreur pour les paramètres qui ne peut pas être retourné.</span><span class="sxs-lookup"><span data-stu-id="4dec6-104">The **DomainSettingsErrors** element contains error information for settings that could not be returned.</span></span> 
  
```XML
<DomainSettingsErrors>
   <DomainSettingsError/>
</DomainSettingsErrors>
```

 <span data-ttu-id="4dec6-105">**DomainSettingsErrors**</span><span class="sxs-lookup"><span data-stu-id="4dec6-105">**DomainSettingsErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4dec6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4dec6-106">Attributes and elements</span></span>

<span data-ttu-id="4dec6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4dec6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4dec6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4dec6-108">Attributes</span></span>

<span data-ttu-id="4dec6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4dec6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4dec6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4dec6-110">Child elements</span></span>

|<span data-ttu-id="4dec6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4dec6-111">**Element**</span></span>|<span data-ttu-id="4dec6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4dec6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4dec6-113">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4dec6-113">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="4dec6-114">Représente une erreur s’est produite lors de la récupération d’un paramètre du domaine.</span><span class="sxs-lookup"><span data-stu-id="4dec6-114">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="4dec6-115">Cela représente une erreur à partir d’une demande d’opération [GetDomainSettings opération (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="4dec6-115">This represents an error from a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4dec6-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4dec6-116">Parent elements</span></span>

|<span data-ttu-id="4dec6-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4dec6-117">**Element**</span></span>|<span data-ttu-id="4dec6-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="4dec6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4dec6-119">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4dec6-119">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="4dec6-120">Contient les paramètres requis pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="4dec6-120">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4dec6-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4dec6-121">Text value</span></span>

<span data-ttu-id="4dec6-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4dec6-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4dec6-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4dec6-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4dec6-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4dec6-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4dec6-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4dec6-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4dec6-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="4dec6-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4dec6-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4dec6-127">Validation File</span></span>  <br/> |<span data-ttu-id="4dec6-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4dec6-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4dec6-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4dec6-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="4dec6-130">True</span><span class="sxs-lookup"><span data-stu-id="4dec6-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4dec6-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4dec6-131">See also</span></span>

- [<span data-ttu-id="4dec6-132">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4dec6-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

