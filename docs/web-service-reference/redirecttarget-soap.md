---
title: RedirectTarget (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: L’élément RedirectTarget (SOAP) contient la cible de la redirection URL ou adresse de messagerie.
ms.openlocfilehash: 3a8a0c39c6889730c9d17778c6a26f84fcbcd4a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829019"
---
# <a name="redirecttarget-soap"></a><span data-ttu-id="fb300-103">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fb300-103">RedirectTarget (SOAP)</span></span>

<span data-ttu-id="fb300-104">L’élément [RedirectTarget (SOAP)](redirecttarget-soap.md) contient la cible de la redirection URL ou adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="fb300-104">The [RedirectTarget (SOAP)](redirecttarget-soap.md) element contains the target of the redirection URL or e-mail address.</span></span> 
  
```XML
<RedirectTarget/>
```

 <span data-ttu-id="fb300-105">**string**</span><span class="sxs-lookup"><span data-stu-id="fb300-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb300-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fb300-106">Attributes and elements</span></span>

<span data-ttu-id="fb300-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fb300-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb300-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fb300-108">Attributes</span></span>

<span data-ttu-id="fb300-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fb300-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb300-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fb300-110">Child elements</span></span>

<span data-ttu-id="fb300-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fb300-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb300-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fb300-112">Parent elements</span></span>

|<span data-ttu-id="fb300-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fb300-113">**Element**</span></span>|<span data-ttu-id="fb300-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb300-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb300-115">Réponse de l’utilisateur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fb300-115">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="fb300-116">Représente une réponse à une demande de GetUserSettings pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="fb300-116">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
|[<span data-ttu-id="fb300-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fb300-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="fb300-118">Contient les paramètres requis pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="fb300-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb300-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="fb300-119">Text value</span></span>

<span data-ttu-id="fb300-120">La valeur de texte contient la cible de la redirection URL ou l’adresse électronique qui doit être utilisé pour un GetUserSettings ultérieures ou demander des GetDomainSettings.</span><span class="sxs-lookup"><span data-stu-id="fb300-120">The text value contains the target of the redirection URL or e-mail address that should be used for a subsequent GetUserSettings or GetDomainSettings request.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb300-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fb300-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb300-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fb300-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="fb300-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fb300-123">Schema Name</span></span>  <br/> |<span data-ttu-id="fb300-124">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="fb300-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="fb300-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fb300-125">Validation File</span></span>  <br/> |<span data-ttu-id="fb300-126">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fb300-126">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb300-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fb300-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb300-128">True</span><span class="sxs-lookup"><span data-stu-id="fb300-128">True</span></span>  <br/> |
   

