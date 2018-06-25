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
ms.openlocfilehash: b02071e4997aba91fb538d52df2612fe6fd32800
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829385"
---
# <a name="serverversioninfo-soap"></a><span data-ttu-id="6e346-103">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e346-103">ServerVersionInfo (SOAP)</span></span>

<span data-ttu-id="6e346-104">L’élément **ServerVersionInfo** contient la version du serveur qui a traité la demande.</span><span class="sxs-lookup"><span data-stu-id="6e346-104">The **ServerVersionInfo** element contains the version of the server that processed the request.</span></span> 
  
```XML
<ServerVersionInfo>
   <MajorVersion/>
   <MinorVersion/>
   <MajorBuildNumber/>
   <MinorBuildNumber/>
   <Version/>
</ServerVersionInfo>
```

 <span data-ttu-id="6e346-105">**ServerVersionInfo**</span><span class="sxs-lookup"><span data-stu-id="6e346-105">**ServerVersionInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e346-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6e346-106">Attributes and elements</span></span>

<span data-ttu-id="6e346-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6e346-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e346-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6e346-108">Attributes</span></span>

<span data-ttu-id="6e346-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6e346-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e346-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6e346-110">Child elements</span></span>

|<span data-ttu-id="6e346-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6e346-111">**Element**</span></span>|<span data-ttu-id="6e346-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="6e346-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e346-113">MajorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e346-113">MajorVersion (SOAP)</span></span>](majorversion-soap.md) <br/> |<span data-ttu-id="6e346-114">Le numéro de version principal pour le serveur.</span><span class="sxs-lookup"><span data-stu-id="6e346-114">The major version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="6e346-115">MinorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e346-115">MinorVersion (SOAP)</span></span>](minorversion-soap.md) <br/> |<span data-ttu-id="6e346-116">Numéro de version secondaire pour le serveur.</span><span class="sxs-lookup"><span data-stu-id="6e346-116">The minor version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="6e346-117">MajorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e346-117">MajorBuildNumber (SOAP)</span></span>](majorbuildnumber-soap.md) <br/> |<span data-ttu-id="6e346-118">Numéro de version majeur pour le serveur.</span><span class="sxs-lookup"><span data-stu-id="6e346-118">The major build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="6e346-119">MinorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e346-119">MinorBuildNumber (SOAP)</span></span>](minorbuildnumber-soap.md) <br/> |<span data-ttu-id="6e346-120">Numéro de version secondaire pour le serveur.</span><span class="sxs-lookup"><span data-stu-id="6e346-120">The minor build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="6e346-121">Version (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e346-121">Version (SOAP)</span></span>](version-soap.md) <br/> |<span data-ttu-id="6e346-122">Description de la version de produit du serveur.</span><span class="sxs-lookup"><span data-stu-id="6e346-122">A description of the server product version.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e346-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6e346-123">Parent elements</span></span>

<span data-ttu-id="6e346-124">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6e346-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e346-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="6e346-125">Remarks</span></span>

<span data-ttu-id="6e346-126">Cet élément est retourné dans l’en-tête SOAP.</span><span class="sxs-lookup"><span data-stu-id="6e346-126">This element is returned in the SOAP header.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e346-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6e346-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e346-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6e346-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6e346-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6e346-129">Schema Name</span></span>  <br/> |<span data-ttu-id="6e346-130">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="6e346-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6e346-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6e346-131">Validation File</span></span>  <br/> |<span data-ttu-id="6e346-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6e346-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e346-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6e346-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e346-134">True</span><span class="sxs-lookup"><span data-stu-id="6e346-134">True</span></span>  <br/> |
   

