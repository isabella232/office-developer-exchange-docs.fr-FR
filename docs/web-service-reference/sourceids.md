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
ms.openlocfilehash: 1c4990f2185788c5cfaab5483cb6a54a0d850596
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466107"
---
# <a name="sourceids"></a><span data-ttu-id="ce1b8-103">SourceIds</span><span class="sxs-lookup"><span data-stu-id="ce1b8-103">SourceIds</span></span>

<span data-ttu-id="ce1b8-104">L’élément **SourceIds** contient les identificateurs source à convertir.</span><span class="sxs-lookup"><span data-stu-id="ce1b8-104">The **SourceIds** element contains the source identifiers to convert.</span></span> 
  
[<span data-ttu-id="ce1b8-105">ConvertId</span><span class="sxs-lookup"><span data-stu-id="ce1b8-105">ConvertId</span></span>](convertid.md)
  
[<span data-ttu-id="ce1b8-106">SourceIds</span><span class="sxs-lookup"><span data-stu-id="ce1b8-106">SourceIds</span></span>](sourceids.md)
  
```xml
<SourceIds>
   <AlternateId/>
   <AlternatePublicFolderId/>
   <AlternatePublicFolderItemId/>
</SourceIds>
```

 <span data-ttu-id="ce1b8-107">**NonEmptyArrayOfAlternateIdsType**</span><span class="sxs-lookup"><span data-stu-id="ce1b8-107">**NonEmptyArrayOfAlternateIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce1b8-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ce1b8-108">Attributes and elements</span></span>

<span data-ttu-id="ce1b8-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ce1b8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce1b8-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="ce1b8-110">Attributes</span></span>

<span data-ttu-id="ce1b8-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ce1b8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce1b8-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ce1b8-112">Child elements</span></span>

|<span data-ttu-id="ce1b8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ce1b8-113">**Element**</span></span>|<span data-ttu-id="ce1b8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ce1b8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce1b8-115">AlternateId</span><span class="sxs-lookup"><span data-stu-id="ce1b8-115">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="ce1b8-116">Décrit un identificateur d’élément ou de dossier à convertir.</span><span class="sxs-lookup"><span data-stu-id="ce1b8-116">Describes an item or folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="ce1b8-117">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="ce1b8-117">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md) <br/> |<span data-ttu-id="ce1b8-118">Décrit un identificateur de dossier public à convertir.</span><span class="sxs-lookup"><span data-stu-id="ce1b8-118">Describes a public folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="ce1b8-119">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="ce1b8-119">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md) <br/> |<span data-ttu-id="ce1b8-120">Décrit un identificateur d’élément de dossier public à convertir.</span><span class="sxs-lookup"><span data-stu-id="ce1b8-120">Describes a public folder item identifier to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce1b8-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ce1b8-121">Parent elements</span></span>

|<span data-ttu-id="ce1b8-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ce1b8-122">**Element**</span></span>|<span data-ttu-id="ce1b8-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="ce1b8-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce1b8-124">ConvertId</span><span class="sxs-lookup"><span data-stu-id="ce1b8-124">ConvertId</span></span>](convertid.md) <br/> |<span data-ttu-id="ce1b8-125">Définit une demande de conversion des identificateurs d’élément et de dossier entre les formats Exchange pris en charge.</span><span class="sxs-lookup"><span data-stu-id="ce1b8-125">Defines a request to convert item and folder identifiers between Exchange supported formats.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ce1b8-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="ce1b8-126">Remarks</span></span>

<span data-ttu-id="ce1b8-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ce1b8-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce1b8-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ce1b8-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce1b8-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ce1b8-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ce1b8-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ce1b8-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ce1b8-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ce1b8-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ce1b8-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ce1b8-132">Validation File</span></span>  <br/> |<span data-ttu-id="ce1b8-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ce1b8-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ce1b8-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ce1b8-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce1b8-135">False</span><span class="sxs-lookup"><span data-stu-id="ce1b8-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce1b8-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ce1b8-136">See also</span></span>



[<span data-ttu-id="ce1b8-137">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="ce1b8-137">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="ce1b8-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ce1b8-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ce1b8-139">Conversion des identificateurs</span><span class="sxs-lookup"><span data-stu-id="ce1b8-139">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

