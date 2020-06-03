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
description: L’élément FindFolder définit une demande de recherche de dossiers dans une boîte aux lettres.
ms.openlocfilehash: 248047206a661afe723543e52c51b57847148423
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462576"
---
# <a name="findfolder"></a><span data-ttu-id="18f84-103">FindFolder</span><span class="sxs-lookup"><span data-stu-id="18f84-103">FindFolder</span></span>

<span data-ttu-id="18f84-104">L’élément **FindFolder** définit une demande de recherche de dossiers dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="18f84-104">The **FindFolder** element defines a request to find folders in a mailbox.</span></span> 
  
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

<span data-ttu-id="18f84-105">**FindFolderType**</span><span class="sxs-lookup"><span data-stu-id="18f84-105">**FindFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="18f84-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="18f84-106">Attributes and elements</span></span>

<span data-ttu-id="18f84-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="18f84-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18f84-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="18f84-108">Attributes</span></span>

|<span data-ttu-id="18f84-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="18f84-109">**Attribute**</span></span>|<span data-ttu-id="18f84-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="18f84-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="18f84-111">Traversée</span><span class="sxs-lookup"><span data-stu-id="18f84-111">Traversal</span></span>  <br/> |<span data-ttu-id="18f84-112">Définit le mode d’exécution d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="18f84-112">Defines how a search is performed.</span></span> <span data-ttu-id="18f84-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="18f84-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="18f84-114">Valeurs d’attribut transversal</span><span class="sxs-lookup"><span data-stu-id="18f84-114">Traversal attribute values</span></span>

|<span data-ttu-id="18f84-115">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="18f84-115">**Value**</span></span>|<span data-ttu-id="18f84-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="18f84-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="18f84-117">Partielle</span><span class="sxs-lookup"><span data-stu-id="18f84-117">Shallow</span></span>  <br/> |<span data-ttu-id="18f84-118">Indique à l’opération FindFolder de rechercher uniquement le dossier identifié et de renvoyer uniquement les ID de dossier pour les éléments qui n’ont pas été supprimés.</span><span class="sxs-lookup"><span data-stu-id="18f84-118">Instructs the FindFolder operation to search only the identified folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="18f84-119">Il s’agit d’un parcours superficiel.</span><span class="sxs-lookup"><span data-stu-id="18f84-119">This is called a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="18f84-120">Développée</span><span class="sxs-lookup"><span data-stu-id="18f84-120">Deep</span></span>  <br/> |<span data-ttu-id="18f84-121">Indique à l’opération FindFolder d’effectuer une recherche dans tous les dossiers enfants du dossier parent identifié et de renvoyer uniquement les ID de dossier pour les éléments qui n’ont pas été supprimés.</span><span class="sxs-lookup"><span data-stu-id="18f84-121">Instructs the FindFolder operation to search in all child folders of the identified parent folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="18f84-122">Il s’agit d’un parcours approfondi.</span><span class="sxs-lookup"><span data-stu-id="18f84-122">This is called a deep traversal.</span></span>  <br/> |
|<span data-ttu-id="18f84-123">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="18f84-123">SoftDeleted</span></span>  <br/> |<span data-ttu-id="18f84-124">Indique à l’opération FindFolder d’effectuer une recherche de parcours superficiel pour les éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="18f84-124">Instructs the FindFolder operation to perform a shallow traversal search for deleted items.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="18f84-125">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="18f84-125">Child elements</span></span>

|<span data-ttu-id="18f84-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="18f84-126">**Element**</span></span>|<span data-ttu-id="18f84-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="18f84-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18f84-128">FolderShape</span><span class="sxs-lookup"><span data-stu-id="18f84-128">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="18f84-129">Identifie les propriétés de dossier à inclure dans une réponse FindFolder.</span><span class="sxs-lookup"><span data-stu-id="18f84-129">Identifies the folder properties to include in a FindFolder response.</span></span>  <br/> |
|[<span data-ttu-id="18f84-130">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="18f84-130">IndexedPageFolderView</span></span>](indexedpagefolderview.md) <br/> |<span data-ttu-id="18f84-131">Décrit comment les informations d’élément paginé sont renvoyées dans une réponse FindFolder.</span><span class="sxs-lookup"><span data-stu-id="18f84-131">Describes how paged item information is returned in a FindFolder response.</span></span> <span data-ttu-id="18f84-132">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="18f84-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="18f84-133">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="18f84-133">FractionalPageFolderView</span></span>](fractionalpagefolderview.md) <br/> |<span data-ttu-id="18f84-134">Décrit l’emplacement où l’affichage paginé démarre et le nombre maximal de dossiers renvoyés dans une demande FindFolder.</span><span class="sxs-lookup"><span data-stu-id="18f84-134">Describes where the paged view starts and the maximum number of folders returned in a FindFolder request.</span></span> <span data-ttu-id="18f84-135">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="18f84-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="18f84-136">Restriction</span><span class="sxs-lookup"><span data-stu-id="18f84-136">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="18f84-137">Définit une restriction ou une requête utilisée pour filtrer les dossiers dans une opération FindFolder.</span><span class="sxs-lookup"><span data-stu-id="18f84-137">Defines a restriction or query that is used to filter folders in a FindFolder operation.</span></span> <span data-ttu-id="18f84-138">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="18f84-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="18f84-139">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="18f84-139">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="18f84-140">Identifie les dossiers pour l’opération FindFolder à rechercher.</span><span class="sxs-lookup"><span data-stu-id="18f84-140">Identifies folders for the FindFolder operation to search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18f84-141">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="18f84-141">Parent elements</span></span>

<span data-ttu-id="18f84-142">Aucun.</span><span class="sxs-lookup"><span data-stu-id="18f84-142">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="18f84-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="18f84-143">Remarks</span></span>

<span data-ttu-id="18f84-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="18f84-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="18f84-145">Exemple</span><span class="sxs-lookup"><span data-stu-id="18f84-145">Example</span></span>

<span data-ttu-id="18f84-146">L’exemple de requête FindFolder suivant montre comment créer une requête pour rechercher tous les dossiers situés dans une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="18f84-146">The following example of a FindFolder request shows how to form a request to find all the folders located in an Inbox.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="18f84-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="18f84-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18f84-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="18f84-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="18f84-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="18f84-149">Schema Name</span></span>  <br/> |<span data-ttu-id="18f84-150">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="18f84-150">Messages schema</span></span>  <br/> |
|<span data-ttu-id="18f84-151">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="18f84-151">Validation File</span></span>  <br/> |<span data-ttu-id="18f84-152">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="18f84-152">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="18f84-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="18f84-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="18f84-154">False</span><span class="sxs-lookup"><span data-stu-id="18f84-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18f84-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="18f84-155">See also</span></span>

- [<span data-ttu-id="18f84-156">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="18f84-156">FindFolder operation</span></span>](findfolder-operation.md)

