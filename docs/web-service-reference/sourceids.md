---
title: SourceIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SourceIds
api_type:
- schema
ms.assetid: 0043abd5-ba9c-4d67-8832-325f32bf7651
description: L’élément SourceIds contient les identificateurs source à convertir.
ms.openlocfilehash: c9ee9fd01367f714e1cb3770e2be5161cb45d98f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829522"
---
# <a name="sourceids"></a><span data-ttu-id="9b6c8-103">SourceIds</span><span class="sxs-lookup"><span data-stu-id="9b6c8-103">SourceIds</span></span>

<span data-ttu-id="9b6c8-104">L’élément **SourceIds** contient les identificateurs source à convertir.</span><span class="sxs-lookup"><span data-stu-id="9b6c8-104">The **SourceIds** element contains the source identifiers to convert.</span></span> 
  
[<span data-ttu-id="9b6c8-105">ConvertId</span><span class="sxs-lookup"><span data-stu-id="9b6c8-105">ConvertId</span></span>](convertid.md)
  
[<span data-ttu-id="9b6c8-106">SourceIds</span><span class="sxs-lookup"><span data-stu-id="9b6c8-106">SourceIds</span></span>](sourceids.md)
  
```xml
<SourceIds>
   <AlternateId/>
   <AlternatePublicFolderId/>
   <AlternatePublicFolderItemId/>
</SourceIds>
```

 <span data-ttu-id="9b6c8-107">**NonEmptyArrayOfAlternateIdsType**</span><span class="sxs-lookup"><span data-stu-id="9b6c8-107">**NonEmptyArrayOfAlternateIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b6c8-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9b6c8-108">Attributes and elements</span></span>

<span data-ttu-id="9b6c8-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9b6c8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b6c8-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="9b6c8-110">Attributes</span></span>

<span data-ttu-id="9b6c8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9b6c8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b6c8-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9b6c8-112">Child elements</span></span>

|<span data-ttu-id="9b6c8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9b6c8-113">**Element**</span></span>|<span data-ttu-id="9b6c8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9b6c8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b6c8-115">AlternateId</span><span class="sxs-lookup"><span data-stu-id="9b6c8-115">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="9b6c8-116">Décrit un identificateur d’élément ou le dossier à convertir.</span><span class="sxs-lookup"><span data-stu-id="9b6c8-116">Describes an item or folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="9b6c8-117">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="9b6c8-117">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md) <br/> |<span data-ttu-id="9b6c8-118">Décrit un identificateur de dossier public à convertir.</span><span class="sxs-lookup"><span data-stu-id="9b6c8-118">Describes a public folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="9b6c8-119">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="9b6c8-119">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md) <br/> |<span data-ttu-id="9b6c8-120">Décrit un identificateur d’élément de dossier public à convertir.</span><span class="sxs-lookup"><span data-stu-id="9b6c8-120">Describes a public folder item identifier to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b6c8-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9b6c8-121">Parent elements</span></span>

|<span data-ttu-id="9b6c8-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9b6c8-122">**Element**</span></span>|<span data-ttu-id="9b6c8-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="9b6c8-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b6c8-124">ConvertId</span><span class="sxs-lookup"><span data-stu-id="9b6c8-124">ConvertId</span></span>](convertid.md) <br/> |<span data-ttu-id="9b6c8-125">Définit une demande de convertir les identificateurs d’éléments et dossiers entre les formats Exchange pris en charge.</span><span class="sxs-lookup"><span data-stu-id="9b6c8-125">Defines a request to convert item and folder identifiers between Exchange supported formats.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b6c8-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="9b6c8-126">Remarks</span></span>

<span data-ttu-id="9b6c8-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute le serveur Exchange qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="9b6c8-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b6c8-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9b6c8-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b6c8-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9b6c8-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9b6c8-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9b6c8-130">Schema Name</span></span>  <br/> |<span data-ttu-id="9b6c8-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9b6c8-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9b6c8-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9b6c8-132">Validation File</span></span>  <br/> |<span data-ttu-id="9b6c8-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9b6c8-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9b6c8-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9b6c8-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b6c8-135">False</span><span class="sxs-lookup"><span data-stu-id="9b6c8-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b6c8-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9b6c8-136">See also</span></span>



[<span data-ttu-id="9b6c8-137">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="9b6c8-137">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="9b6c8-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9b6c8-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="9b6c8-139">Conversion des identificateurs</span><span class="sxs-lookup"><span data-stu-id="9b6c8-139">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

