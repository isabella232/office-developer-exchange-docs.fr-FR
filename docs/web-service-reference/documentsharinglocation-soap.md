---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: L’élément DocumentSharingLocation contient des informations sur l’emplacement et les métadonnées pour un emplacement de partage de documents.
ms.openlocfilehash: 6fed933da979ab3e3fca51ba606127b7f0a4e3f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457059"
---
# <a name="documentsharinglocation-soap"></a><span data-ttu-id="c0486-103">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0486-103">DocumentSharingLocation (SOAP)</span></span>

<span data-ttu-id="c0486-104">L’élément **DocumentSharingLocation** contient des informations sur l’emplacement et les métadonnées pour un emplacement de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="c0486-104">The **DocumentSharingLocation** element contains location and metadata information for a document sharing location.</span></span> 
  
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

 <span data-ttu-id="c0486-105">**DocumentSharingLocation**</span><span class="sxs-lookup"><span data-stu-id="c0486-105">**DocumentSharingLocation**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0486-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c0486-106">Attributes and elements</span></span>

<span data-ttu-id="c0486-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c0486-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0486-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c0486-108">Attributes</span></span>

<span data-ttu-id="c0486-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c0486-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0486-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c0486-110">Child elements</span></span>

|<span data-ttu-id="c0486-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c0486-111">**Element**</span></span>|<span data-ttu-id="c0486-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c0486-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0486-113">ServiceUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0486-113">ServiceUrl (SOAP)</span></span>](serviceurl-soap.md) <br/> |<span data-ttu-id="c0486-114">Représente l’URL du service Web de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="c0486-114">Represents the URL of the document sharing web service.</span></span>  <br/> |
|[<span data-ttu-id="c0486-115">Locationurl, (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0486-115">LocationUrl (SOAP)</span></span>](locationurl-soap.md) <br/> |<span data-ttu-id="c0486-116">Représente l’URL de l’emplacement de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="c0486-116">Represents the URL of the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="c0486-117">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0486-117">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="c0486-118">Représente le nom de l’emplacement de partage de documents à utiliser dans l’interface utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c0486-118">Represents the name of the document sharing location to use in the UI.</span></span>  <br/> |
|[<span data-ttu-id="c0486-119">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0486-119">SupportedFileExtensions (SOAP)</span></span>](supportedfileextensions-soap.md) <br/> |<span data-ttu-id="c0486-120">Représente les extensions de fichiers qui peuvent être stockées dans l’emplacement de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="c0486-120">Represents the file extensions that can be stored in the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="c0486-121">ExternalAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0486-121">ExternalAccessAllowed (SOAP)</span></span>](externalaccessallowed-soap.md) <br/> |<span data-ttu-id="c0486-122">Indique si l’emplacement de partage de documents est disponible pour les connexions extérieures.</span><span class="sxs-lookup"><span data-stu-id="c0486-122">Indicates whether the document sharing location is available to outside connections.</span></span>  <br/> |
|[<span data-ttu-id="c0486-123">AnonymousAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0486-123">AnonymousAccessAllowed (SOAP)</span></span>](anonymousaccessallowed-soap.md) <br/> |<span data-ttu-id="c0486-124">Indique si l’accès à l’emplacement de partage nécessite un utilisateur authentifié.</span><span class="sxs-lookup"><span data-stu-id="c0486-124">Indicates whether access to the sharing location requires an authenticated user.</span></span>  <br/> |
|[<span data-ttu-id="c0486-125">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0486-125">CanModifyPermissions (SOAP)</span></span>](canmodifypermissions-soap.md) <br/> |<span data-ttu-id="c0486-126">Indique si l’utilisateur peut modifier les autorisations d’accès à l’emplacement de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="c0486-126">Indicates whether the user can modify access permissions to the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="c0486-127">IsDefault (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0486-127">IsDefault (SOAP)</span></span>](isdefault-soap.md) <br/> |<span data-ttu-id="c0486-128">Indique si l’emplacement de partage de documents est l’emplacement de partage par défaut de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c0486-128">Indicates whether the document sharing location is the user's default sharing location.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c0486-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c0486-129">Parent elements</span></span>

|<span data-ttu-id="c0486-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c0486-130">**Element**</span></span>|<span data-ttu-id="c0486-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="c0486-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0486-132">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0486-132">DocumentSharingLocations (SOAP)</span></span>](documentsharinglocations-soap.md) <br/> |<span data-ttu-id="c0486-133">Contient une liste des métadonnées et des emplacements de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="c0486-133">Contains a list of document sharing locations and metadata.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c0486-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c0486-134">Text value</span></span>

<span data-ttu-id="c0486-135">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c0486-135">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0486-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c0486-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0486-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c0486-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c0486-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c0486-138">Schema Name</span></span>  <br/> |<span data-ttu-id="c0486-139">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="c0486-139">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c0486-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c0486-140">Validation File</span></span>  <br/> |<span data-ttu-id="c0486-141">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c0486-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c0486-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c0486-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="c0486-143">True</span><span class="sxs-lookup"><span data-stu-id="c0486-143">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0486-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c0486-144">See also</span></span>

- [<span data-ttu-id="c0486-145">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0486-145">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="c0486-146">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="c0486-146">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="c0486-147">Éléments XML de découverte automatique SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="c0486-147">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

