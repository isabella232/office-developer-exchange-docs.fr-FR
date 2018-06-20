---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: L’élément DocumentSharingLocation contient l’emplacement et les informations de métadonnées pour un emplacement de partage de documents.
ms.openlocfilehash: d258efecb46d570138c7c2c78ed9d2fa9a275103
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756024"
---
# <a name="documentsharinglocation-soap"></a><span data-ttu-id="0fd05-103">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0fd05-103">DocumentSharingLocation (SOAP)</span></span>

<span data-ttu-id="0fd05-104">L’élément **DocumentSharingLocation** contient l’emplacement et les informations de métadonnées pour un emplacement de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="0fd05-104">The **DocumentSharingLocation** element contains location and metadata information for a document sharing location.</span></span> 
  
```XML
<DocumentSharingLocation>
   <ServiceUrl />
   <LocationUrl />
   <DisplayName />
   <SupportedFileExtensions />
   <ExternalAccessAllowed />
   <AnonymousAccessAllowed />
   <CanModifyPermissions />
   <IsDefault />
</DocumentSharingLocation>
```

 <span data-ttu-id="0fd05-105">**DocumentSharingLocation**</span><span class="sxs-lookup"><span data-stu-id="0fd05-105">**DocumentSharingLocation**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0fd05-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0fd05-106">Attributes and elements</span></span>

<span data-ttu-id="0fd05-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0fd05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0fd05-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0fd05-108">Attributes</span></span>

<span data-ttu-id="0fd05-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0fd05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0fd05-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0fd05-110">Child elements</span></span>

|<span data-ttu-id="0fd05-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0fd05-111">**Element**</span></span>|<span data-ttu-id="0fd05-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0fd05-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fd05-113">ServiceUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0fd05-113">ServiceUrl (SOAP)</span></span>](serviceurl-soap.md) <br/> |<span data-ttu-id="0fd05-114">Représente l’URL du service web de partage de document.</span><span class="sxs-lookup"><span data-stu-id="0fd05-114">Represents the URL of the document sharing web service.</span></span>  <br/> |
|[<span data-ttu-id="0fd05-115">LocationUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0fd05-115">LocationUrl (SOAP)</span></span>](locationurl-soap.md) <br/> |<span data-ttu-id="0fd05-116">Représente l’URL de l’emplacement de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="0fd05-116">Represents the URL of the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="0fd05-117">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0fd05-117">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="0fd05-118">Représente le nom de l’emplacement à utiliser dans l’interface utilisateur de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="0fd05-118">Represents the name of the document sharing location to use in the UI.</span></span>  <br/> |
|[<span data-ttu-id="0fd05-119">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0fd05-119">SupportedFileExtensions (SOAP)</span></span>](supportedfileextensions-soap.md) <br/> |<span data-ttu-id="0fd05-120">Représente les extensions de fichier qui peuvent être stockées dans l’emplacement de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="0fd05-120">Represents the file extensions that can be stored in the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="0fd05-121">ExternalAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0fd05-121">ExternalAccessAllowed (SOAP)</span></span>](externalaccessallowed-soap.md) <br/> |<span data-ttu-id="0fd05-122">Indique si l’emplacement de partage de documents sont disponible à l’extérieur des connexions.</span><span class="sxs-lookup"><span data-stu-id="0fd05-122">Indicates whether the document sharing location is available to outside connections.</span></span>  <br/> |
|[<span data-ttu-id="0fd05-123">AnonymousAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0fd05-123">AnonymousAccessAllowed (SOAP)</span></span>](anonymousaccessallowed-soap.md) <br/> |<span data-ttu-id="0fd05-124">Indique si l’accès à l’emplacement de partage requiert qu’un utilisateur authentifié.</span><span class="sxs-lookup"><span data-stu-id="0fd05-124">Indicates whether access to the sharing location requires an authenticated user.</span></span>  <br/> |
|[<span data-ttu-id="0fd05-125">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0fd05-125">CanModifyPermissions (SOAP)</span></span>](canmodifypermissions-soap.md) <br/> |<span data-ttu-id="0fd05-126">Indique si l’utilisateur peut modifier les autorisations d’accès à l’emplacement de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="0fd05-126">Indicates whether the user can modify access permissions to the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="0fd05-127">IsDefault (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0fd05-127">IsDefault (SOAP)</span></span>](isdefault-soap.md) <br/> |<span data-ttu-id="0fd05-128">Indique si l’emplacement de partage de documents sont par défaut de l’utilisateur à l’emplacement de partage.</span><span class="sxs-lookup"><span data-stu-id="0fd05-128">Indicates whether the document sharing location is the user's default sharing location.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0fd05-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0fd05-129">Parent elements</span></span>

|<span data-ttu-id="0fd05-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0fd05-130">**Element**</span></span>|<span data-ttu-id="0fd05-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="0fd05-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fd05-132">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0fd05-132">DocumentSharingLocations (SOAP)</span></span>](documentsharinglocations-soap.md) <br/> |<span data-ttu-id="0fd05-133">Contient une liste d’emplacements et les métadonnées de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="0fd05-133">Contains a list of document sharing locations and metadata.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0fd05-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0fd05-134">Text value</span></span>

<span data-ttu-id="0fd05-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0fd05-135">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0fd05-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0fd05-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0fd05-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0fd05-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0fd05-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0fd05-138">Schema Name</span></span>  <br/> |<span data-ttu-id="0fd05-139">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="0fd05-139">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0fd05-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0fd05-140">Validation File</span></span>  <br/> |<span data-ttu-id="0fd05-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0fd05-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0fd05-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0fd05-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="0fd05-143">True</span><span class="sxs-lookup"><span data-stu-id="0fd05-143">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0fd05-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0fd05-144">See also</span></span>

- [<span data-ttu-id="0fd05-145">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0fd05-145">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="0fd05-146">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0fd05-146">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="0fd05-147">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0fd05-147">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)
