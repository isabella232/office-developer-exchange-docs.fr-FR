---
title: FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: b8a59740-d978-454c-9629-a10792385ba0
description: L’élément FindFolder définit une requête pour rechercher les dossiers dans une boîte aux lettres.
ms.openlocfilehash: 69fbaebc5615ac7d19512770658cde83e4d352df
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353531"
---
# <a name="findfolder"></a><span data-ttu-id="293d4-103">FindFolder</span><span class="sxs-lookup"><span data-stu-id="293d4-103">FindFolder</span></span>

<span data-ttu-id="293d4-104">L’élément **FindFolder** définit une requête pour rechercher les dossiers dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="293d4-104">The **FindFolder** element defines a request to find folders in a mailbox.</span></span> 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <FractionalPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

<span data-ttu-id="293d4-105">**FindFolderType**</span><span class="sxs-lookup"><span data-stu-id="293d4-105">**FindFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="293d4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="293d4-106">Attributes and elements</span></span>

<span data-ttu-id="293d4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="293d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="293d4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="293d4-108">Attributes</span></span>

|<span data-ttu-id="293d4-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="293d4-109">**Attribute**</span></span>|<span data-ttu-id="293d4-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="293d4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="293d4-111">Traversée du contenu</span><span class="sxs-lookup"><span data-stu-id="293d4-111">Traversal</span></span>  <br/> |<span data-ttu-id="293d4-112">Définit la façon dont une recherche est effectuée.</span><span class="sxs-lookup"><span data-stu-id="293d4-112">Defines how a search is performed.</span></span> <span data-ttu-id="293d4-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="293d4-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="293d4-114">Valeurs d’attribut Traversal</span><span class="sxs-lookup"><span data-stu-id="293d4-114">Traversal attribute values</span></span>

|<span data-ttu-id="293d4-115">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="293d4-115">**Value**</span></span>|<span data-ttu-id="293d4-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="293d4-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="293d4-117">Peu profond</span><span class="sxs-lookup"><span data-stu-id="293d4-117">Shallow</span></span>  <br/> |<span data-ttu-id="293d4-118">Indique à l’opération FindFolder recherche uniquement le dossier identifié et renvoyer uniquement l’ID de dossier pour les éléments qui n’ont pas été supprimés.</span><span class="sxs-lookup"><span data-stu-id="293d4-118">Instructs the FindFolder operation to search only the identified folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="293d4-119">Il s’agit d’un parcours en surface.</span><span class="sxs-lookup"><span data-stu-id="293d4-119">This is called a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="293d4-120">Profond</span><span class="sxs-lookup"><span data-stu-id="293d4-120">Deep</span></span>  <br/> |<span data-ttu-id="293d4-121">Indique à l’opération FindFolder pour la recherche dans tous les dossiers enfants du dossier parent identifié et renvoyer uniquement l’ID de dossier pour les éléments qui n’ont pas été supprimés.</span><span class="sxs-lookup"><span data-stu-id="293d4-121">Instructs the FindFolder operation to search in all child folders of the identified parent folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="293d4-122">Il s’agit d’une longue traversée.</span><span class="sxs-lookup"><span data-stu-id="293d4-122">This is called a deep traversal.</span></span>  <br/> |
|<span data-ttu-id="293d4-123">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="293d4-123">SoftDeleted</span></span>  <br/> |<span data-ttu-id="293d4-124">Indique à l’opération FindFolder pour effectuer une recherche parcours en surface des éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="293d4-124">Instructs the FindFolder operation to perform a shallow traversal search for deleted items.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="293d4-125">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="293d4-125">Child elements</span></span>

|<span data-ttu-id="293d4-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="293d4-126">**Element**</span></span>|<span data-ttu-id="293d4-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="293d4-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="293d4-128">FolderShape</span><span class="sxs-lookup"><span data-stu-id="293d4-128">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="293d4-129">Identifie les propriétés du dossier à inclure dans une réponse FindFolder.</span><span class="sxs-lookup"><span data-stu-id="293d4-129">Identifies the folder properties to include in a FindFolder response.</span></span>  <br/> |
|[<span data-ttu-id="293d4-130">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="293d4-130">IndexedPageFolderView</span></span>](indexedpagefolderview.md) <br/> |<span data-ttu-id="293d4-131">Décrit comment paginé informations sont retournées dans une réponse FindFolder.</span><span class="sxs-lookup"><span data-stu-id="293d4-131">Describes how paged item information is returned in a FindFolder response.</span></span> <span data-ttu-id="293d4-132">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="293d4-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="293d4-133">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="293d4-133">FractionalPageFolderView</span></span>](fractionalpagefolderview.md) <br/> |<span data-ttu-id="293d4-134">Décrit où l’affichage paginé démarre et le nombre maximal de dossiers renvoyées dans une requête FindFolder.</span><span class="sxs-lookup"><span data-stu-id="293d4-134">Describes where the paged view starts and the maximum number of folders returned in a FindFolder request.</span></span> <span data-ttu-id="293d4-135">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="293d4-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="293d4-136">Restriction</span><span class="sxs-lookup"><span data-stu-id="293d4-136">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="293d4-137">Définit une restriction ou une requête qui est utilisé pour filtrer les dossiers dans une opération FindFolder.</span><span class="sxs-lookup"><span data-stu-id="293d4-137">Defines a restriction or query that is used to filter folders in a FindFolder operation.</span></span> <span data-ttu-id="293d4-138">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="293d4-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="293d4-139">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="293d4-139">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="293d4-140">Identifie les dossiers pour l’opération FindFolder à rechercher.</span><span class="sxs-lookup"><span data-stu-id="293d4-140">Identifies folders for the FindFolder operation to search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="293d4-141">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="293d4-141">Parent elements</span></span>

<span data-ttu-id="293d4-142">Aucun.</span><span class="sxs-lookup"><span data-stu-id="293d4-142">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="293d4-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="293d4-143">Remarks</span></span>

<span data-ttu-id="293d4-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="293d4-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="293d4-145">Exemple</span><span class="sxs-lookup"><span data-stu-id="293d4-145">Example</span></span>

<span data-ttu-id="293d4-146">L’exemple suivant d’une demande FindFolder indique comment former une requête pour rechercher tous les dossiers situés dans une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="293d4-146">The following example of a FindFolder request shows how to form a request to find all the folders located in an Inbox.</span></span>
  
```xml
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

## <a name="element-information"></a><span data-ttu-id="293d4-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="293d4-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="293d4-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="293d4-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="293d4-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="293d4-149">Schema Name</span></span>  <br/> |<span data-ttu-id="293d4-150">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="293d4-150">Messages schema</span></span>  <br/> |
|<span data-ttu-id="293d4-151">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="293d4-151">Validation File</span></span>  <br/> |<span data-ttu-id="293d4-152">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="293d4-152">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="293d4-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="293d4-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="293d4-154">False</span><span class="sxs-lookup"><span data-stu-id="293d4-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="293d4-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="293d4-155">See also</span></span>

- [<span data-ttu-id="293d4-156">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="293d4-156">FindFolder operation</span></span>](findfolder-operation.md)

