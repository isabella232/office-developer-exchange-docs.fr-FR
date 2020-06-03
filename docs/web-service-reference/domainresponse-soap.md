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
description: L’élément DomainResponse contient les paramètres demandés pour le domaine spécifié.
ms.openlocfilehash: dea6e36c51ceea53201b668cfba616c03a44df86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456961"
---
# <a name="domainresponse-soap"></a><span data-ttu-id="ad55e-103">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad55e-103">DomainResponse (SOAP)</span></span>

<span data-ttu-id="ad55e-104">L’élément **DomainResponse** contient les paramètres demandés pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="ad55e-104">The **DomainResponse** element contains the requested settings for the specified domain.</span></span> 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 <span data-ttu-id="ad55e-105">**DomainResponse**</span><span class="sxs-lookup"><span data-stu-id="ad55e-105">**DomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad55e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad55e-106">Attributes and elements</span></span>

<span data-ttu-id="ad55e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad55e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad55e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad55e-108">Attributes</span></span>

<span data-ttu-id="ad55e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ad55e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad55e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad55e-110">Child elements</span></span>

|<span data-ttu-id="ad55e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad55e-111">**Element**</span></span>|<span data-ttu-id="ad55e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad55e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad55e-113">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad55e-113">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="ad55e-114">Contient des informations d’erreur pour les paramètres qui n’ont pas pu être renvoyés.</span><span class="sxs-lookup"><span data-stu-id="ad55e-114">Contains error information for settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="ad55e-115">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad55e-115">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="ad55e-116">Représente les paramètres de domaine qui ont été envoyés dans une demande de découverte automatique ou renvoyés par une réponse de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="ad55e-116">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="ad55e-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad55e-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="ad55e-118">Identifie la cible de la redirection.</span><span class="sxs-lookup"><span data-stu-id="ad55e-118">Identifies the target of the redirection.</span></span> <span data-ttu-id="ad55e-119">La cible peut être une URL ou une adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="ad55e-119">The target can be either a URL or an e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="ad55e-120">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad55e-120">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="ad55e-121">Spécifie le code d’erreur associé à la demande spécifique.</span><span class="sxs-lookup"><span data-stu-id="ad55e-121">Specifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="ad55e-122">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad55e-122">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="ad55e-123">Spécifie le message d’erreur qui est associé à la demande spécifique.</span><span class="sxs-lookup"><span data-stu-id="ad55e-123">Specifies the error message that is associated with the specific request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad55e-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad55e-124">Parent elements</span></span>

|<span data-ttu-id="ad55e-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad55e-125">**Element**</span></span>|<span data-ttu-id="ad55e-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad55e-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad55e-127">ArrayOfDomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad55e-127">ArrayOfDomainResponse (SOAP)</span></span>](arrayofdomainresponse-soap.md) <br/> |<span data-ttu-id="ad55e-128">Contient un tableau d’éléments **DomainResponse** .</span><span class="sxs-lookup"><span data-stu-id="ad55e-128">Contains an array of **DomainResponse** elements.</span></span> <span data-ttu-id="ad55e-129">Chaque élément **DomainResponse** contient les paramètres demandés pour l’utilisateur spécifié.</span><span class="sxs-lookup"><span data-stu-id="ad55e-129">Each **DomainResponse** element contains the requested settings for the specified user.</span></span>  <br/> |
|[<span data-ttu-id="ad55e-130">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad55e-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="ad55e-131">Contient les réponses pour chaque domaine.</span><span class="sxs-lookup"><span data-stu-id="ad55e-131">Contains the responses for each domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad55e-132">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ad55e-132">Text value</span></span>

<span data-ttu-id="ad55e-133">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ad55e-133">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad55e-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad55e-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad55e-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad55e-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ad55e-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad55e-136">Schema Name</span></span>  <br/> |<span data-ttu-id="ad55e-137">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ad55e-137">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ad55e-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ad55e-138">Validation File</span></span>  <br/> |<span data-ttu-id="ad55e-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ad55e-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ad55e-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad55e-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad55e-141">True</span><span class="sxs-lookup"><span data-stu-id="ad55e-141">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad55e-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad55e-142">See also</span></span>

- [<span data-ttu-id="ad55e-143">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad55e-143">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

