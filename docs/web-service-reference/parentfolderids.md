---
title: ParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderIds
api_type:
- schema
ms.assetid: e7998023-e5e0-465c-91fa-2aa6d1559f64
description: L’élément ParentFolderIds identifie les dossiers pour les opérations FindItem et FindFolder à rechercher.
ms.openlocfilehash: 4dd23b45dcc397e29e67fc08b29dd773e50f0db1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828688"
---
# <a name="parentfolderids"></a><span data-ttu-id="342c0-103">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="342c0-103">ParentFolderIds</span></span>

<span data-ttu-id="342c0-104">L’élément **ParentFolderIds** identifie les dossiers pour les opérations FindItem et FindFolder à rechercher.</span><span class="sxs-lookup"><span data-stu-id="342c0-104">The **ParentFolderIds** element identifies folders for the FindItem and FindFolder operations to search.</span></span> 
  
```xml
<ParentFolderIds>
   <DistinguishedFolderId/>
<ParentFolderIds>
```

<span data-ttu-id="342c0-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="342c0-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="342c0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="342c0-106">Attributes and elements</span></span>

<span data-ttu-id="342c0-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="342c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="342c0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="342c0-108">Attributes</span></span>

<span data-ttu-id="342c0-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="342c0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="342c0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="342c0-110">Child elements</span></span>

|<span data-ttu-id="342c0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="342c0-111">**Element**</span></span>|<span data-ttu-id="342c0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="342c0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="342c0-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="342c0-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="342c0-114">Contient la clé d’identificateur et de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="342c0-114">Contains the identifier and change key of a folder.</span></span> <span data-ttu-id="342c0-115">L’élément **ParentFolderIds** doit utiliser cet élément ou l’élément [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="342c0-115">The **ParentFolderIds** element must use either this element or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="342c0-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="342c0-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="342c0-117">Identifie les dossiers Microsoft Exchange Server 2007 qui peuvent être référencés par son nom.</span><span class="sxs-lookup"><span data-stu-id="342c0-117">Identifies Microsoft Exchange Server 2007 folders that can be referenced by name.</span></span> <span data-ttu-id="342c0-118">L’élément **ParentFolderIds** doit utiliser cet élément ou l’élément [FolderId](folderid.md) .</span><span class="sxs-lookup"><span data-stu-id="342c0-118">The **ParentFolderIds** element must use either this element or the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="342c0-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="342c0-119">Parent elements</span></span>

|<span data-ttu-id="342c0-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="342c0-120">**Element**</span></span>|<span data-ttu-id="342c0-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="342c0-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="342c0-122">FindFolder</span><span class="sxs-lookup"><span data-stu-id="342c0-122">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="342c0-123">Définit une demande pour identifier les dossiers dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="342c0-123">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="342c0-124">FindItem</span><span class="sxs-lookup"><span data-stu-id="342c0-124">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="342c0-125">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="342c0-125">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="342c0-126">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="342c0-126">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="342c0-127">Définit une demande de résolution de noms ambigus.</span><span class="sxs-lookup"><span data-stu-id="342c0-127">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="342c0-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="342c0-128">Remarks</span></span>

<span data-ttu-id="342c0-129">L’élément **ParentFolderIds** doit utiliser l' [ID FolderId](folderid.md) ou l’élément [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="342c0-129">The **ParentFolderIds** element must use either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> <span data-ttu-id="342c0-130">Un nombre illimité de dossiers peut être défini pour la recherche.</span><span class="sxs-lookup"><span data-stu-id="342c0-130">An unlimited number of folders can be defined for the search.</span></span> 
  
## <a name="example"></a><span data-ttu-id="342c0-131">Exemple</span><span class="sxs-lookup"><span data-stu-id="342c0-131">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="342c0-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="342c0-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="342c0-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="342c0-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="342c0-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="342c0-134">Schema Name</span></span>  <br/> |<span data-ttu-id="342c0-135">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="342c0-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="342c0-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="342c0-136">Validation File</span></span>  <br/> |<span data-ttu-id="342c0-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="342c0-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="342c0-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="342c0-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="342c0-139">False</span><span class="sxs-lookup"><span data-stu-id="342c0-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="342c0-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="342c0-140">See also</span></span>

- [<span data-ttu-id="342c0-141">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="342c0-141">FindFolder operation</span></span>](findfolder-operation.md)  
- [<span data-ttu-id="342c0-142">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="342c0-142">FindItem operation</span></span>](finditem-operation.md) 
- [<span data-ttu-id="342c0-143">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="342c0-143">ResolveNames operation</span></span>](resolvenames-operation.md)

