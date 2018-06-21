---
title: DocumentSharingLocations (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 394f6015-721b-4800-9286-039d430f09b3
description: L’élément DocumentSharingLocations contient une liste d’emplacement et les informations de métadonnées pour un emplacement de partage de documents.
ms.openlocfilehash: 72d1ae9f01ad45441b4e255f2fb6353be2dc8d28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19756028"
---
# <a name="documentsharinglocations-soap"></a><span data-ttu-id="e324b-103">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e324b-103">DocumentSharingLocations (SOAP)</span></span>

<span data-ttu-id="e324b-104">L’élément **DocumentSharingLocations** contient une liste d’emplacement et les informations de métadonnées pour un emplacement de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="e324b-104">The **DocumentSharingLocations** element contains a list of location and metadata information for a document sharing location.</span></span> 
  
```XML
<DocumentSharingLocations>
   <DocumentSharingLocation />
</DocumentSharingLocations>
```

 <span data-ttu-id="e324b-105">**DocumentSharingLocations**</span><span class="sxs-lookup"><span data-stu-id="e324b-105">**DocumentSharingLocations**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e324b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e324b-106">Attributes and elements</span></span>

<span data-ttu-id="e324b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e324b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e324b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e324b-108">Attributes</span></span>

<span data-ttu-id="e324b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e324b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e324b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e324b-110">Child elements</span></span>

|<span data-ttu-id="e324b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e324b-111">**Element**</span></span>|<span data-ttu-id="e324b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e324b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e324b-113">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e324b-113">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="e324b-114">Contient l’emplacement et les métadonnées pour un emplacement de partage de document.</span><span class="sxs-lookup"><span data-stu-id="e324b-114">Contains the location and metadata for a document sharing location.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e324b-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e324b-115">Parent elements</span></span>

|<span data-ttu-id="e324b-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e324b-116">**Element**</span></span>|<span data-ttu-id="e324b-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="e324b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e324b-118">DocumentSharingLocationCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e324b-118">DocumentSharingLocationCollectionSetting (SOAP)</span></span>](documentsharinglocationcollectionsetting-soap.md) <br/> |<span data-ttu-id="e324b-119">Représente un utilisateur de paramètre qui est une collection de documentation de métadonnées et les emplacements de partage.</span><span class="sxs-lookup"><span data-stu-id="e324b-119">Represents a user setting that is a collection of documentation sharing locations and metadata.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="e324b-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e324b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e324b-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e324b-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e324b-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e324b-122">Schema Name</span></span>  <br/> |<span data-ttu-id="e324b-123">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="e324b-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e324b-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e324b-124">Validation File</span></span>  <br/> |<span data-ttu-id="e324b-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e324b-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e324b-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e324b-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="e324b-127">True</span><span class="sxs-lookup"><span data-stu-id="e324b-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e324b-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e324b-128">See also</span></span>

- [<span data-ttu-id="e324b-129">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e324b-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="e324b-130">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e324b-130">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="e324b-131">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e324b-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

