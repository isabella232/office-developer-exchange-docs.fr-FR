---
title: RequestServerVersion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestServerVersion
api_type:
- schema
ms.assetid: af4032d5-42b3-463e-9d0a-8236d78e5b75
description: L’élément RequestServerVersion contient les informations de contrôle de version qui identifie la version de schéma cible pour une demande.
ms.openlocfilehash: 0092d90a5fc479363f6d774b793c7148ad29f21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829143"
---
# <a name="requestserverversion"></a><span data-ttu-id="034e5-103">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="034e5-103">RequestServerVersion</span></span>

<span data-ttu-id="034e5-104">L’élément **RequestServerVersion** contient les informations de contrôle de version qui identifie la version de schéma cible pour une demande.</span><span class="sxs-lookup"><span data-stu-id="034e5-104">The **RequestServerVersion** element contains the versioning information that identifies the schema version to target for a request.</span></span> 
  
```XML
<RequestServerVersion Version=""/>
```

 <span data-ttu-id="034e5-105">**ExchangeVersionType**</span><span class="sxs-lookup"><span data-stu-id="034e5-105">**ExchangeVersionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="034e5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="034e5-106">Attributes and elements</span></span>

<span data-ttu-id="034e5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="034e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="034e5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="034e5-108">Attributes</span></span>

|<span data-ttu-id="034e5-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="034e5-109">**Attribute**</span></span>|<span data-ttu-id="034e5-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="034e5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="034e5-111">Version</span><span class="sxs-lookup"><span data-stu-id="034e5-111">Version</span></span>  <br/> |<span data-ttu-id="034e5-112">Décrit la version cible pour la demande.</span><span class="sxs-lookup"><span data-stu-id="034e5-112">Describes the version to target for the request.</span></span> <span data-ttu-id="034e5-113">Cet attribut est requis lorsque la version du serveur cible est une version d’Exchange commençant par Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="034e5-113">This attribute is required when the target server version is a version of Exchange starting with Exchange Server 2010.</span></span>  <br/> |
   
#### <a name="version-attribute-values"></a><span data-ttu-id="034e5-114">Valeurs d’attribut version</span><span class="sxs-lookup"><span data-stu-id="034e5-114">Version attribute values</span></span>

|<span data-ttu-id="034e5-115">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="034e5-115">**Value**</span></span>|<span data-ttu-id="034e5-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="034e5-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="034e5-117">Exchange2007</span><span class="sxs-lookup"><span data-stu-id="034e5-117">Exchange2007</span></span>  <br/> |<span data-ttu-id="034e5-118">Cible : les fichiers de schéma pour la version initiale d’Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="034e5-118">Target the schema files for the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="034e5-119">Exchange2007_SP1</span><span class="sxs-lookup"><span data-stu-id="034e5-119">Exchange2007_SP1</span></span>  <br/> |<span data-ttu-id="034e5-120">Cible : les fichiers de schéma pour Exchange 2007 Service Pack 1 (SP1), Exchange 2007 Service Pack 2 (SP2) et Exchange 2007 Service Pack 3 (SP3).</span><span class="sxs-lookup"><span data-stu-id="034e5-120">Target the schema files for Exchange 2007 Service Pack 1 (SP1), Exchange 2007 Service Pack 2 (SP2), and Exchange 2007 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="034e5-121">Exchange2010</span><span class="sxs-lookup"><span data-stu-id="034e5-121">Exchange2010</span></span>  <br/> |<span data-ttu-id="034e5-122">Cible : les fichiers de schéma pour Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="034e5-122">Target the schema files for Exchange 2010.</span></span>  <br/> |
|<span data-ttu-id="034e5-123">Exchange2010_SP1</span><span class="sxs-lookup"><span data-stu-id="034e5-123">Exchange2010_SP1</span></span>  <br/> |<span data-ttu-id="034e5-124">Cible : les fichiers de schéma pour Exchange 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="034e5-124">Target the schema files for Exchange 2010 Service Pack 1 (SP1).</span></span>  <br/> |
|<span data-ttu-id="034e5-125">Exchange2010_SP2</span><span class="sxs-lookup"><span data-stu-id="034e5-125">Exchange2010_SP2</span></span>  <br/> |<span data-ttu-id="034e5-126">Cible : les fichiers de schéma pour Exchange 2010 Service Pack 2 (SP2) et Exchange 2010 Service Pack 3 (SP3).</span><span class="sxs-lookup"><span data-stu-id="034e5-126">Target the schema files for Exchange 2010 Service Pack 2 (SP2) and Exchange 2010 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="034e5-127">Exchange2013</span><span class="sxs-lookup"><span data-stu-id="034e5-127">Exchange2013</span></span>  <br/> |<span data-ttu-id="034e5-128">Cible : les fichiers de schéma pour Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="034e5-128">Target the schema files for Exchange 2013.</span></span>  <br/> |
|<span data-ttu-id="034e5-129">Exchange2013_SP1</span><span class="sxs-lookup"><span data-stu-id="034e5-129">Exchange2013_SP1</span></span>  <br/> |<span data-ttu-id="034e5-130">Cible : les fichiers de schéma pour Exchange 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="034e5-130">Target the schema files for Exchange 2013 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="034e5-131">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="034e5-131">Child elements</span></span>

<span data-ttu-id="034e5-132">Aucun.</span><span class="sxs-lookup"><span data-stu-id="034e5-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="034e5-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="034e5-133">Parent elements</span></span>

<span data-ttu-id="034e5-134">L’élément **RequestServerVersion** se trouve dans l’en-tête SOAP.</span><span class="sxs-lookup"><span data-stu-id="034e5-134">The **RequestServerVersion** element is located in the SOAP header.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="034e5-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="034e5-135">Remarks</span></span>

<span data-ttu-id="034e5-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="034e5-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="034e5-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="034e5-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="034e5-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="034e5-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="034e5-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="034e5-139">Schema Name</span></span>  <br/> |<span data-ttu-id="034e5-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="034e5-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="034e5-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="034e5-141">Validation File</span></span>  <br/> |<span data-ttu-id="034e5-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="034e5-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="034e5-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="034e5-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="034e5-144">False</span><span class="sxs-lookup"><span data-stu-id="034e5-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="034e5-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="034e5-145">See also</span></span>



- [<span data-ttu-id="034e5-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="034e5-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="034e5-147">Demandes de contrôle de version</span><span class="sxs-lookup"><span data-stu-id="034e5-147">Versioning Requests</span></span>](http://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

