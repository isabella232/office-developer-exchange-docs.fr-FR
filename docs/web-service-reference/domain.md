---
title: Domaine
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Domain
api_type:
- schema
ms.assetid: 7e45a061-856f-4b44-b053-a7c4d5ad569e
description: L’élément de domaine identifie un domaine SMTP unique.
ms.openlocfilehash: 78eb1edfd347a513b84b9c15d143d76425041e85
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756032"
---
# <a name="domain"></a><span data-ttu-id="8d18b-103">Domaine</span><span class="sxs-lookup"><span data-stu-id="8d18b-103">Domain</span></span>

<span data-ttu-id="8d18b-104">L’élément de **domaine** identifie un domaine SMTP unique.</span><span class="sxs-lookup"><span data-stu-id="8d18b-104">The **Domain** element identifies a single SMTP domain.</span></span> 
  
```xml
<Domain Name="" IncludeSubdomains="" />
```

 <span data-ttu-id="8d18b-105">**StmpDomain**</span><span class="sxs-lookup"><span data-stu-id="8d18b-105">**StmpDomain**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d18b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8d18b-106">Attributes and elements</span></span>

<span data-ttu-id="8d18b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8d18b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d18b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8d18b-108">Attributes</span></span>

|<span data-ttu-id="8d18b-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="8d18b-109">**Attribute**</span></span>|<span data-ttu-id="8d18b-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="8d18b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8d18b-111">Nom</span><span class="sxs-lookup"><span data-stu-id="8d18b-111">Name</span></span>  <br/> |<span data-ttu-id="8d18b-112">Identifie le nom d’un domaine.</span><span class="sxs-lookup"><span data-stu-id="8d18b-112">Identifies the name of a domain.</span></span> <span data-ttu-id="8d18b-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="8d18b-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="8d18b-114">IncludeSubdomains</span><span class="sxs-lookup"><span data-stu-id="8d18b-114">IncludeSubdomains</span></span>  <br/> |<span data-ttu-id="8d18b-115">Indique si les sous-domaines du domaine identifié par l’attribut **Name** sont considérés comme internes.</span><span class="sxs-lookup"><span data-stu-id="8d18b-115">Indicates whether subdomains of the domain identified by the **Name** attribute are considered internal.</span></span> <span data-ttu-id="8d18b-116">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="8d18b-116">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8d18b-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8d18b-117">Child elements</span></span>

<span data-ttu-id="8d18b-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8d18b-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d18b-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8d18b-119">Parent elements</span></span>

|<span data-ttu-id="8d18b-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8d18b-120">**Element**</span></span>|<span data-ttu-id="8d18b-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="8d18b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d18b-122">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="8d18b-122">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="8d18b-123">Identifie la liste des domaines SMTP internes de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="8d18b-123">Identifies the list of internal SMTP domains of the organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d18b-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8d18b-124">Text value</span></span>

<span data-ttu-id="8d18b-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8d18b-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8d18b-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="8d18b-126">Remarks</span></span>

<span data-ttu-id="8d18b-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8d18b-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d18b-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8d18b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d18b-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8d18b-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d18b-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8d18b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="8d18b-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8d18b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d18b-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8d18b-132">Validation File</span></span>  <br/> |<span data-ttu-id="8d18b-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8d18b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d18b-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8d18b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d18b-135">False</span><span class="sxs-lookup"><span data-stu-id="8d18b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d18b-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8d18b-136">See also</span></span>

- [<span data-ttu-id="8d18b-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8d18b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

