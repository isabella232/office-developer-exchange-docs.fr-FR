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
description: L’élément RedirectTarget (SOAP) contient la cible de l’URL de redirection ou de l’adresse de messagerie.
ms.openlocfilehash: 092d575560379d43b12dd98a3efa155b59c31450
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462198"
---
# <a name="redirecttarget-soap"></a><span data-ttu-id="2ca93-103">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ca93-103">RedirectTarget (SOAP)</span></span>

<span data-ttu-id="2ca93-104">L’élément [RedirectTarget (SOAP)](redirecttarget-soap.md) contient la cible de l’URL de redirection ou de l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="2ca93-104">The [RedirectTarget (SOAP)](redirecttarget-soap.md) element contains the target of the redirection URL or e-mail address.</span></span> 
  
```XML
<RedirectTarget/>
```

 <span data-ttu-id="2ca93-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="2ca93-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ca93-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2ca93-106">Attributes and elements</span></span>

<span data-ttu-id="2ca93-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2ca93-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ca93-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2ca93-108">Attributes</span></span>

<span data-ttu-id="2ca93-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2ca93-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ca93-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2ca93-110">Child elements</span></span>

<span data-ttu-id="2ca93-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ca93-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ca93-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2ca93-112">Parent elements</span></span>

|<span data-ttu-id="2ca93-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ca93-113">**Element**</span></span>|<span data-ttu-id="2ca93-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ca93-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ca93-115">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ca93-115">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="2ca93-116">Représente une réponse à une demande GetUserSettings pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="2ca93-116">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
|[<span data-ttu-id="2ca93-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ca93-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="2ca93-118">Contient les paramètres demandés pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="2ca93-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ca93-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="2ca93-119">Text value</span></span>

<span data-ttu-id="2ca93-120">La valeur texte contient la cible de l’URL de redirection ou de l’adresse de messagerie à utiliser pour une requête GetUserSettings ou GetDomainSettings ultérieure.</span><span class="sxs-lookup"><span data-stu-id="2ca93-120">The text value contains the target of the redirection URL or e-mail address that should be used for a subsequent GetUserSettings or GetDomainSettings request.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ca93-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2ca93-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ca93-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2ca93-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2ca93-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2ca93-123">Schema Name</span></span>  <br/> |<span data-ttu-id="2ca93-124">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="2ca93-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2ca93-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2ca93-125">Validation File</span></span>  <br/> |<span data-ttu-id="2ca93-126">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2ca93-126">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2ca93-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2ca93-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ca93-128">True</span><span class="sxs-lookup"><span data-stu-id="2ca93-128">True</span></span>  <br/> |
   

