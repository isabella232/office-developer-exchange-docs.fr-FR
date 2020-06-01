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
description: L’élément domaine identifie un domaine SMTP unique.
ms.openlocfilehash: 3bf8e132b5fa588171ac4f3c095692bc68394663
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461330"
---
# <a name="domain"></a><span data-ttu-id="08a94-103">Domaine</span><span class="sxs-lookup"><span data-stu-id="08a94-103">Domain</span></span>

<span data-ttu-id="08a94-104">L’élément **domaine** identifie un domaine SMTP unique.</span><span class="sxs-lookup"><span data-stu-id="08a94-104">The **Domain** element identifies a single SMTP domain.</span></span> 
  
```xml
<Domain Name="" IncludeSubdomains="" />
```

 <span data-ttu-id="08a94-105">**StmpDomain**</span><span class="sxs-lookup"><span data-stu-id="08a94-105">**StmpDomain**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08a94-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="08a94-106">Attributes and elements</span></span>

<span data-ttu-id="08a94-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="08a94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08a94-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="08a94-108">Attributes</span></span>

|<span data-ttu-id="08a94-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="08a94-109">**Attribute**</span></span>|<span data-ttu-id="08a94-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="08a94-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="08a94-111">Nom</span><span class="sxs-lookup"><span data-stu-id="08a94-111">Name</span></span>  <br/> |<span data-ttu-id="08a94-112">Identifie le nom d’un domaine.</span><span class="sxs-lookup"><span data-stu-id="08a94-112">Identifies the name of a domain.</span></span> <span data-ttu-id="08a94-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="08a94-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="08a94-114">IncludeSubdomains</span><span class="sxs-lookup"><span data-stu-id="08a94-114">IncludeSubdomains</span></span>  <br/> |<span data-ttu-id="08a94-115">Indique si les sous-domaines du domaine identifiés par l’attribut **Name** sont considérés comme internes.</span><span class="sxs-lookup"><span data-stu-id="08a94-115">Indicates whether subdomains of the domain identified by the **Name** attribute are considered internal.</span></span> <span data-ttu-id="08a94-116">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="08a94-116">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="08a94-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="08a94-117">Child elements</span></span>

<span data-ttu-id="08a94-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08a94-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08a94-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="08a94-119">Parent elements</span></span>

|<span data-ttu-id="08a94-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="08a94-120">**Element**</span></span>|<span data-ttu-id="08a94-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="08a94-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08a94-122">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="08a94-122">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="08a94-123">Identifie la liste des domaines SMTP internes de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="08a94-123">Identifies the list of internal SMTP domains of the organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="08a94-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="08a94-124">Text value</span></span>

<span data-ttu-id="08a94-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08a94-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="08a94-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="08a94-126">Remarks</span></span>

<span data-ttu-id="08a94-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="08a94-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08a94-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="08a94-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08a94-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="08a94-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08a94-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="08a94-130">Schema Name</span></span>  <br/> |<span data-ttu-id="08a94-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="08a94-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="08a94-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="08a94-132">Validation File</span></span>  <br/> |<span data-ttu-id="08a94-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="08a94-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08a94-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="08a94-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="08a94-135">False</span><span class="sxs-lookup"><span data-stu-id="08a94-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08a94-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="08a94-136">See also</span></span>

- [<span data-ttu-id="08a94-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="08a94-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

