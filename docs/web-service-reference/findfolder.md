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
ms.openlocfilehash: d41283547c443e38e2e87379a7224df9c89f901d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756385"
---
# <a name="findfolder"></a><span data-ttu-id="e683b-103">FindFolder</span><span class="sxs-lookup"><span data-stu-id="e683b-103">FindFolder</span></span>

<span data-ttu-id="e683b-104">L’élément **FindFolder** définit une requête pour rechercher les dossiers dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e683b-104">The **FindFolder** element defines a request to find folders in a mailbox.</span></span> 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

 <span data-ttu-id="e683b-105">**FindFolderType**</span><span class="sxs-lookup"><span data-stu-id="e683b-105">**FindFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e683b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e683b-106">Attributes and elements</span></span>

<span data-ttu-id="e683b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e683b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e683b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e683b-108">Attributes</span></span>

|<span data-ttu-id="e683b-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="e683b-109">**Attribute**</span></span>|<span data-ttu-id="e683b-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="e683b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e683b-111">Traversée du contenu</span><span class="sxs-lookup"><span data-stu-id="e683b-111">Traversal</span></span>  <br/> |<span data-ttu-id="e683b-112">Définit la façon dont une recherche est effectuée.</span><span class="sxs-lookup"><span data-stu-id="e683b-112">Defines how a search is performed.</span></span> <span data-ttu-id="e683b-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="e683b-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="e683b-114">Valeurs d’attribut Traversal</span><span class="sxs-lookup"><span data-stu-id="e683b-114">Traversal attribute values</span></span>

|<span data-ttu-id="e683b-115">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="e683b-115">**Value**</span></span>|<span data-ttu-id="e683b-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="e683b-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e683b-117">Peu profond</span><span class="sxs-lookup"><span data-stu-id="e683b-117">Shallow</span></span>  <br/> |<span data-ttu-id="e683b-118">Indique à l’opération FindFolder recherche uniquement le dossier identifié et renvoyer uniquement l’ID de dossier pour les éléments qui n’ont pas été supprimés.</span><span class="sxs-lookup"><span data-stu-id="e683b-118">Instructs the FindFolder operation to search only the identified folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="e683b-119">Il s’agit d’un parcours en surface.</span><span class="sxs-lookup"><span data-stu-id="e683b-119">This is called a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="e683b-120">Profond</span><span class="sxs-lookup"><span data-stu-id="e683b-120">Deep</span></span>  <br/> |<span data-ttu-id="e683b-121">Indique à l’opération FindFolder pour la recherche dans tous les dossiers enfants du dossier parent identifié et renvoyer uniquement l’ID de dossier pour les éléments qui n’ont pas été supprimés.</span><span class="sxs-lookup"><span data-stu-id="e683b-121">Instructs the FindFolder operation to search in all child folders of the identified parent folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="e683b-122">Il s’agit d’une longue traversée.</span><span class="sxs-lookup"><span data-stu-id="e683b-122">This is called a deep traversal.</span></span>  <br/> |
|<span data-ttu-id="e683b-123">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="e683b-123">SoftDeleted</span></span>  <br/> |<span data-ttu-id="e683b-124">Indique à l’opération FindFolder pour effectuer une recherche parcours en surface des éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="e683b-124">Instructs the FindFolder operation to perform a shallow traversal search for deleted items.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e683b-125">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e683b-125">Child elements</span></span>

|<span data-ttu-id="e683b-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e683b-126">**Element**</span></span>|<span data-ttu-id="e683b-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="e683b-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e683b-128">FolderShape</span><span class="sxs-lookup"><span data-stu-id="e683b-128">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="e683b-129">Identifie les propriétés du dossier à inclure dans une réponse FindFolder.</span><span class="sxs-lookup"><span data-stu-id="e683b-129">Identifies the folder properties to include in a FindFolder response.</span></span>  <br/> |
|[<span data-ttu-id="e683b-130">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="e683b-130">IndexedPageFolderView</span></span>](indexedpagefolderview.md) <br/> |<span data-ttu-id="e683b-131">Décrit comment paginé informations sont retournées dans une réponse FindFolder.</span><span class="sxs-lookup"><span data-stu-id="e683b-131">Describes how paged item information is returned in a FindFolder response.</span></span> <span data-ttu-id="e683b-132">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e683b-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e683b-133">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="e683b-133">FractionalPageFolderView</span></span>](fractionalpagefolderview.md) <br/> |<span data-ttu-id="e683b-134">Décrit où l’affichage paginé démarre et le nombre maximal de dossiers renvoyées dans une requête FindFolder.</span><span class="sxs-lookup"><span data-stu-id="e683b-134">Describes where the paged view starts and the maximum number of folders returned in a FindFolder request.</span></span> <span data-ttu-id="e683b-135">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e683b-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e683b-136">Restriction</span><span class="sxs-lookup"><span data-stu-id="e683b-136">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="e683b-137">Définit une restriction ou une requête qui est utilisé pour filtrer les dossiers dans une opération FindFolder.</span><span class="sxs-lookup"><span data-stu-id="e683b-137">Defines a restriction or query that is used to filter folders in a FindFolder operation.</span></span> <span data-ttu-id="e683b-138">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e683b-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e683b-139">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="e683b-139">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="e683b-140">Identifie les dossiers pour l’opération FindFolder à rechercher.</span><span class="sxs-lookup"><span data-stu-id="e683b-140">Identifies folders for the FindFolder operation to search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e683b-141">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e683b-141">Parent elements</span></span>

<span data-ttu-id="e683b-142">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e683b-142">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e683b-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="e683b-143">Remarks</span></span>

<span data-ttu-id="e683b-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e683b-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="e683b-145">Exemple</span><span class="sxs-lookup"><span data-stu-id="e683b-145">Example</span></span>

<span data-ttu-id="e683b-146">L’exemple suivant d’une demande FindFolder indique comment former une requête pour rechercher tous les dossiers situés dans une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="e683b-146">The following example of a FindFolder request shows how to form a request to find all the folders located in an Inbox.</span></span>
  
```
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

## <a name="element-information"></a><span data-ttu-id="e683b-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e683b-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e683b-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e683b-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e683b-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e683b-149">Schema Name</span></span>  <br/> |<span data-ttu-id="e683b-150">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e683b-150">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e683b-151">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e683b-151">Validation File</span></span>  <br/> |<span data-ttu-id="e683b-152">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e683b-152">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e683b-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e683b-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="e683b-154">False</span><span class="sxs-lookup"><span data-stu-id="e683b-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e683b-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e683b-155">See also</span></span>



[<span data-ttu-id="e683b-156">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="e683b-156">FindFolder operation</span></span>](findfolder-operation.md)

