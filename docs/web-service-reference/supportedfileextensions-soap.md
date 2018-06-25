---
title: SupportedFileExtensions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 6f73d18c-7bb1-4ab6-a23b-6d948e590b53
description: L’élément SupportedFileExtensions répertorie les extensions de fichier qui peuvent être stockées dans un emplacement de partage de documents.
ms.openlocfilehash: 0f1dbbce2b836fe05e4bc612c607302783d5e05d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838653"
---
# <a name="supportedfileextensions-soap"></a><span data-ttu-id="0cf5e-103">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0cf5e-103">SupportedFileExtensions (SOAP)</span></span>

<span data-ttu-id="0cf5e-104">L’élément **SupportedFileExtensions** répertorie les extensions de fichier qui peuvent être stockées dans un emplacement de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="0cf5e-104">The **SupportedFileExtensions** element lists the file extensions that can be stored in a document sharing location.</span></span> 
  
```XML
<SupportedFileExtensions /> 
```

 <span data-ttu-id="0cf5e-105">**ArrayOfFileExtension**</span><span class="sxs-lookup"><span data-stu-id="0cf5e-105">**ArrayOfFileExtension**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0cf5e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0cf5e-106">Attributes and elements</span></span>

<span data-ttu-id="0cf5e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0cf5e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0cf5e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0cf5e-108">Attributes</span></span>

<span data-ttu-id="0cf5e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0cf5e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0cf5e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0cf5e-110">Child elements</span></span>

|<span data-ttu-id="0cf5e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0cf5e-111">**Element**</span></span>|<span data-ttu-id="0cf5e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0cf5e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cf5e-113">FileExtension (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0cf5e-113">FileExtension (SOAP)</span></span>](fileextension-soap.md) <br/> |<span data-ttu-id="0cf5e-114">Représente une extension de fichier.</span><span class="sxs-lookup"><span data-stu-id="0cf5e-114">Represents a file extension.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0cf5e-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0cf5e-115">Parent elements</span></span>

|<span data-ttu-id="0cf5e-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0cf5e-116">**Element**</span></span>|<span data-ttu-id="0cf5e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="0cf5e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cf5e-118">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0cf5e-118">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="0cf5e-119">Représente les informations d’emplacement et les métadonnées pour un emplacement de partage de document.</span><span class="sxs-lookup"><span data-stu-id="0cf5e-119">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="0cf5e-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0cf5e-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0cf5e-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0cf5e-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0cf5e-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0cf5e-122">Schema Name</span></span>  <br/> |<span data-ttu-id="0cf5e-123">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="0cf5e-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0cf5e-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0cf5e-124">Validation File</span></span>  <br/> |<span data-ttu-id="0cf5e-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0cf5e-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0cf5e-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0cf5e-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="0cf5e-127">True</span><span class="sxs-lookup"><span data-stu-id="0cf5e-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0cf5e-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0cf5e-128">See also</span></span>



[<span data-ttu-id="0cf5e-129">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0cf5e-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="0cf5e-130">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0cf5e-130">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="0cf5e-131">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0cf5e-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

