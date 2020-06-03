---
title: ServerVersionInfo (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8662647b-e50a-4774-9ba3-a951ae6df781
description: L’élément ServerVersionInfo contient la version du serveur qui a traité la demande.
ms.openlocfilehash: b54b4833361ec78c7f8213473af4638965c7ddae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467647"
---
# <a name="serverversioninfo-soap"></a><span data-ttu-id="f1764-103">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f1764-103">ServerVersionInfo (SOAP)</span></span>

<span data-ttu-id="f1764-104">L’élément **ServerVersionInfo** contient la version du serveur qui a traité la demande.</span><span class="sxs-lookup"><span data-stu-id="f1764-104">The **ServerVersionInfo** element contains the version of the server that processed the request.</span></span> 
  
```XML
<ServerVersionInfo>
   <MajorVersion/>
   <MinorVersion/>
   <MajorBuildNumber/>
   <MinorBuildNumber/>
   <Version/>
</ServerVersionInfo>
```

 <span data-ttu-id="f1764-105">**ServerVersionInfo**</span><span class="sxs-lookup"><span data-stu-id="f1764-105">**ServerVersionInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1764-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f1764-106">Attributes and elements</span></span>

<span data-ttu-id="f1764-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f1764-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1764-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f1764-108">Attributes</span></span>

<span data-ttu-id="f1764-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f1764-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1764-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f1764-110">Child elements</span></span>

|<span data-ttu-id="f1764-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1764-111">**Element**</span></span>|<span data-ttu-id="f1764-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1764-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1764-113">MajorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f1764-113">MajorVersion (SOAP)</span></span>](majorversion-soap.md) <br/> |<span data-ttu-id="f1764-114">Numéro de version principale du serveur.</span><span class="sxs-lookup"><span data-stu-id="f1764-114">The major version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="f1764-115">MinorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f1764-115">MinorVersion (SOAP)</span></span>](minorversion-soap.md) <br/> |<span data-ttu-id="f1764-116">Numéro de version mineure pour le serveur.</span><span class="sxs-lookup"><span data-stu-id="f1764-116">The minor version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="f1764-117">MajorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f1764-117">MajorBuildNumber (SOAP)</span></span>](majorbuildnumber-soap.md) <br/> |<span data-ttu-id="f1764-118">Numéro de version principale du serveur.</span><span class="sxs-lookup"><span data-stu-id="f1764-118">The major build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="f1764-119">MinorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f1764-119">MinorBuildNumber (SOAP)</span></span>](minorbuildnumber-soap.md) <br/> |<span data-ttu-id="f1764-120">Numéro de version mineure du serveur.</span><span class="sxs-lookup"><span data-stu-id="f1764-120">The minor build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="f1764-121">Version (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f1764-121">Version (SOAP)</span></span>](version-soap.md) <br/> |<span data-ttu-id="f1764-122">Description de la version du produit serveur.</span><span class="sxs-lookup"><span data-stu-id="f1764-122">A description of the server product version.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1764-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f1764-123">Parent elements</span></span>

<span data-ttu-id="f1764-124">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f1764-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f1764-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="f1764-125">Remarks</span></span>

<span data-ttu-id="f1764-126">Cet élément est renvoyé dans l’en-tête SOAP.</span><span class="sxs-lookup"><span data-stu-id="f1764-126">This element is returned in the SOAP header.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1764-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f1764-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1764-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f1764-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f1764-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f1764-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f1764-130">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="f1764-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f1764-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f1764-131">Validation File</span></span>  <br/> |<span data-ttu-id="f1764-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f1764-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f1764-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f1764-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1764-134">True</span><span class="sxs-lookup"><span data-stu-id="f1764-134">True</span></span>  <br/> |
   

