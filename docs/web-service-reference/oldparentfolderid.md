---
title: OldParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldParentFolderId
api_type:
- schema
ms.assetid: da1b8c88-c650-455d-b749-0cd160b012d8
description: L’élément OldParentFolderId contient l’identificateur du dossier parent d’un élément ou d’un dossier qui a été copié ou déplacé.
ms.openlocfilehash: ad787e95f95b551393878b15783461d93ac08481
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467227"
---
# <a name="oldparentfolderid"></a><span data-ttu-id="d29c4-103">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d29c4-103">OldParentFolderId</span></span>

<span data-ttu-id="d29c4-104">L’élément **OldParentFolderId** contient l’identificateur du dossier parent d’un élément ou d’un dossier qui a été copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="d29c4-104">The **OldParentFolderId** element contains the identifier of the parent folder of an item or folder that was copied or moved.</span></span> 
  
```xml
<OldParentFolderId Id="" ChangeKey=""/>
```

 <span data-ttu-id="d29c4-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="d29c4-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d29c4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d29c4-106">Attributes and elements</span></span>

<span data-ttu-id="d29c4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d29c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d29c4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d29c4-108">Attributes</span></span>

|<span data-ttu-id="d29c4-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d29c4-109">**Attribute**</span></span>|<span data-ttu-id="d29c4-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d29c4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d29c4-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="d29c4-111">**Id**</span></span> <br/> |<span data-ttu-id="d29c4-112">Contient une chaîne qui identifie un dossier dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="d29c4-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="d29c4-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="d29c4-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d29c4-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="d29c4-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="d29c4-115">Contient une chaîne qui identifie la version d’un dossier identifiée par l’attribut ID.</span><span class="sxs-lookup"><span data-stu-id="d29c4-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="d29c4-116">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d29c4-116">This attribute is optional.</span></span> <span data-ttu-id="d29c4-117">Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.</span><span class="sxs-lookup"><span data-stu-id="d29c4-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d29c4-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d29c4-118">Child elements</span></span>

<span data-ttu-id="d29c4-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d29c4-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d29c4-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d29c4-120">Parent elements</span></span>

|<span data-ttu-id="d29c4-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d29c4-121">**Element**</span></span>|<span data-ttu-id="d29c4-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="d29c4-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d29c4-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="d29c4-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="d29c4-124">Représente un événement dans lequel un élément ou un dossier est copié.</span><span class="sxs-lookup"><span data-stu-id="d29c4-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="d29c4-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="d29c4-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="d29c4-126">Représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent vers un autre dossier parent.</span><span class="sxs-lookup"><span data-stu-id="d29c4-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d29c4-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="d29c4-127">Remarks</span></span>

<span data-ttu-id="d29c4-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d29c4-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d29c4-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d29c4-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d29c4-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d29c4-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d29c4-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d29c4-131">Schema Name</span></span>  <br/> |<span data-ttu-id="d29c4-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d29c4-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="d29c4-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d29c4-133">Validation File</span></span>  <br/> |<span data-ttu-id="d29c4-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d29c4-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d29c4-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d29c4-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="d29c4-136">False</span><span class="sxs-lookup"><span data-stu-id="d29c4-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d29c4-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d29c4-137">See also</span></span>



[<span data-ttu-id="d29c4-138">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="d29c4-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d29c4-139">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="d29c4-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d29c4-140">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="d29c4-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="d29c4-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d29c4-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

