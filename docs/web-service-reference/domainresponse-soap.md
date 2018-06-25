---
title: DomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: L’élément DomainResponse contient les paramètres requis pour le domaine spécifié.
ms.openlocfilehash: c40f33a278b5032913329a7cd64346b572f5df2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756033"
---
# <a name="domainresponse-soap"></a><span data-ttu-id="6e689-103">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e689-103">DomainResponse (SOAP)</span></span>

<span data-ttu-id="6e689-104">L’élément **DomainResponse** contient les paramètres requis pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="6e689-104">The **DomainResponse** element contains the requested settings for the specified domain.</span></span> 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 <span data-ttu-id="6e689-105">**DomainResponse**</span><span class="sxs-lookup"><span data-stu-id="6e689-105">**DomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e689-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6e689-106">Attributes and elements</span></span>

<span data-ttu-id="6e689-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6e689-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e689-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6e689-108">Attributes</span></span>

<span data-ttu-id="6e689-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6e689-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e689-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6e689-110">Child elements</span></span>

|<span data-ttu-id="6e689-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6e689-111">**Element**</span></span>|<span data-ttu-id="6e689-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="6e689-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e689-113">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e689-113">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="6e689-114">Contient des informations d’erreur pour les paramètres qui ne peut pas être retourné.</span><span class="sxs-lookup"><span data-stu-id="6e689-114">Contains error information for settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="6e689-115">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e689-115">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="6e689-116">Représente les paramètres de domaine qui ont été envoyés dans une requête de découverte automatique ou renvoyés par une réponse de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="6e689-116">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="6e689-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e689-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="6e689-118">Identifie la cible de la redirection.</span><span class="sxs-lookup"><span data-stu-id="6e689-118">Identifies the target of the redirection.</span></span> <span data-ttu-id="6e689-119">La cible peut être une URL ou une adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="6e689-119">The target can be either a URL or an e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="6e689-120">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e689-120">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="6e689-121">Spécifie le code d’erreur qui est associé à la demande spécifique.</span><span class="sxs-lookup"><span data-stu-id="6e689-121">Specifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="6e689-122">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e689-122">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="6e689-123">Spécifie le message d’erreur qui est associé à la demande spécifique.</span><span class="sxs-lookup"><span data-stu-id="6e689-123">Specifies the error message that is associated with the specific request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e689-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6e689-124">Parent elements</span></span>

|<span data-ttu-id="6e689-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6e689-125">**Element**</span></span>|<span data-ttu-id="6e689-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="6e689-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e689-127">ArrayOfDomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e689-127">ArrayOfDomainResponse (SOAP)</span></span>](arrayofdomainresponse-soap.md) <br/> |<span data-ttu-id="6e689-128">Contient un tableau d’éléments **DomainResponse** .</span><span class="sxs-lookup"><span data-stu-id="6e689-128">Contains an array of **DomainResponse** elements.</span></span> <span data-ttu-id="6e689-129">Chaque élément **DomainResponse** contient les paramètres requis pour l’utilisateur spécifié.</span><span class="sxs-lookup"><span data-stu-id="6e689-129">Each **DomainResponse** element contains the requested settings for the specified user.</span></span>  <br/> |
|[<span data-ttu-id="6e689-130">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e689-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="6e689-131">Contient les réponses pour chaque domaine.</span><span class="sxs-lookup"><span data-stu-id="6e689-131">Contains the responses for each domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e689-132">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6e689-132">Text value</span></span>

<span data-ttu-id="6e689-133">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6e689-133">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e689-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6e689-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e689-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6e689-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6e689-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6e689-136">Schema Name</span></span>  <br/> |<span data-ttu-id="6e689-137">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="6e689-137">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6e689-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6e689-138">Validation File</span></span>  <br/> |<span data-ttu-id="6e689-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6e689-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e689-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6e689-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e689-141">True</span><span class="sxs-lookup"><span data-stu-id="6e689-141">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e689-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6e689-142">See also</span></span>

- [<span data-ttu-id="6e689-143">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e689-143">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

