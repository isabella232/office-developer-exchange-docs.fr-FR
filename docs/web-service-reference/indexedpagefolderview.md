---
title: IndexedPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageFolderView
api_type:
- schema
ms.assetid: c6dac232-244b-4db0-9a15-5e01b8aa7a7d
description: L’élément IndexedPageFolderView décrit comment paginé informations sont retournées dans une réponse FindFolder.
ms.openlocfilehash: f32f778daa6fa3fea93ab2bc1951f2407dcf7f80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827910"
---
# <a name="indexedpagefolderview"></a><span data-ttu-id="bc751-103">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="bc751-103">IndexedPageFolderView</span></span>

<span data-ttu-id="bc751-104">L’élément **IndexedPageFolderView** décrit comment paginé informations sont retournées dans une réponse [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="bc751-104">The **IndexedPageFolderView** element describes how paged item information is returned in a [FindFolder](findfolder.md) response.</span></span> 
  
[<span data-ttu-id="bc751-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="bc751-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="bc751-106">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="bc751-106">IndexedPageFolderView</span></span>](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 <span data-ttu-id="bc751-107">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="bc751-107">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc751-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bc751-108">Attributes and elements</span></span>

<span data-ttu-id="bc751-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bc751-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc751-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="bc751-110">Attributes</span></span>

|<span data-ttu-id="bc751-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bc751-111">**Attribute**</span></span>|<span data-ttu-id="bc751-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="bc751-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bc751-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="bc751-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="bc751-114">Indique le nombre maximal de dossiers à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="bc751-114">Describes the maximum number of folders to return in the response.</span></span> <span data-ttu-id="bc751-115">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="bc751-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="bc751-116">**Offset**</span><span class="sxs-lookup"><span data-stu-id="bc751-116">**Offset**</span></span> <br/> |<span data-ttu-id="bc751-117">Indique le décalage à partir du **point de base**.</span><span class="sxs-lookup"><span data-stu-id="bc751-117">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="bc751-118">Offset doit être supérieure ou égale à zéro.</span><span class="sxs-lookup"><span data-stu-id="bc751-118">Offset must be greater than or equal to zero.</span></span> <span data-ttu-id="bc751-119">Si le **point de base** est égal au début, le décalage est positif.</span><span class="sxs-lookup"><span data-stu-id="bc751-119">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="bc751-120">Si le **point de base** est égal à End, le décalage est géré comme s’il s’agissait négatif.</span><span class="sxs-lookup"><span data-stu-id="bc751-120">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span>  <br/> <span data-ttu-id="bc751-121">Identifie le dossier qui sera le premier dossier fourni dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="bc751-121">This identifies which folder will be the first folder delivered in the response.</span></span> <span data-ttu-id="bc751-122">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="bc751-122">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="bc751-123">**Point de base**</span><span class="sxs-lookup"><span data-stu-id="bc751-123">**BasePoint**</span></span> <br/> |<span data-ttu-id="bc751-124">Indique si la page des dossiers démarre au début ou à la fin de l’ensemble des dossiers se trouvant avec les critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="bc751-124">Describes whether the page of folders will start from the start or the end of the set of folders that are found with the search criteria.</span></span> <span data-ttu-id="bc751-125">Recherche toujours à partir de la fin de recherche vers l’arrière.</span><span class="sxs-lookup"><span data-stu-id="bc751-125">Seeking from the end always searches backward.</span></span> <span data-ttu-id="bc751-126">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="bc751-126">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="bc751-127">Attribut de point de base</span><span class="sxs-lookup"><span data-stu-id="bc751-127">BasePoint Attribute</span></span>

|<span data-ttu-id="bc751-128">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="bc751-128">**Value**</span></span>|<span data-ttu-id="bc751-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="bc751-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bc751-130">Début</span><span class="sxs-lookup"><span data-stu-id="bc751-130">Beginning</span></span>  <br/> |<span data-ttu-id="bc751-131">L’affichage paginé commence au début de l’ensemble du dossier trouvé.</span><span class="sxs-lookup"><span data-stu-id="bc751-131">The paged view starts at the beginning of the found folder set.</span></span>  <br/> |
|<span data-ttu-id="bc751-132">End</span><span class="sxs-lookup"><span data-stu-id="bc751-132">End</span></span>  <br/> |<span data-ttu-id="bc751-133">L’affichage paginé commence à la fin de l’ensemble du dossier trouvé.</span><span class="sxs-lookup"><span data-stu-id="bc751-133">The paged view starts at the end of the found folder set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bc751-134">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bc751-134">Child elements</span></span>

<span data-ttu-id="bc751-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bc751-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bc751-136">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bc751-136">Parent elements</span></span>

|<span data-ttu-id="bc751-137">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bc751-137">**Element**</span></span>|<span data-ttu-id="bc751-138">**Description**</span><span class="sxs-lookup"><span data-stu-id="bc751-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc751-139">FindFolder</span><span class="sxs-lookup"><span data-stu-id="bc751-139">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="bc751-140">Définit une requête pour rechercher les dossiers dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="bc751-140">Defines a request to find folders in a mailbox.</span></span>  <br/> <span data-ttu-id="bc751-141">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="bc751-141">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bc751-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="bc751-142">Remarks</span></span>

<span data-ttu-id="bc751-143">Recherche à partir de fin consiste à déplacer à l’origine identifié par le décalage.</span><span class="sxs-lookup"><span data-stu-id="bc751-143">Seeking from end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="bc751-144">En outre, le pointeur est ramené par le nombre d’enregistrements demandés.</span><span class="sxs-lookup"><span data-stu-id="bc751-144">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="bc751-145">Par exemple, si 100 enregistrements et le décalage est de 25 à partir de la fin, la recherche démarre 75.</span><span class="sxs-lookup"><span data-stu-id="bc751-145">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="bc751-146">Si 10 enregistrements sont renvoyés, le pointeur est déplacé vers l’arrière 10 supplémentaires à 65 des enregistrements et retourne les enregistrements de 65 à 75.</span><span class="sxs-lookup"><span data-stu-id="bc751-146">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="bc751-147">L’index suivant est de 64.</span><span class="sxs-lookup"><span data-stu-id="bc751-147">The next index is 64.</span></span> <span data-ttu-id="bc751-148">Le prochain offset à partir de la fin d’une page est de 100 moins 64 qui est égale à 36.</span><span class="sxs-lookup"><span data-stu-id="bc751-148">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="bc751-149">La valeur de décalage suivant à partir de la fin pour récupérer la page suivante indexée est 36.</span><span class="sxs-lookup"><span data-stu-id="bc751-149">The value for the next offset from the end to get the next indexed page is 36.</span></span>
  
<span data-ttu-id="bc751-150">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="bc751-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc751-151">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bc751-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc751-152">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bc751-152">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bc751-153">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bc751-153">Schema Name</span></span>  <br/> |<span data-ttu-id="bc751-154">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="bc751-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bc751-155">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bc751-155">Validation File</span></span>  <br/> |<span data-ttu-id="bc751-156">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bc751-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc751-157">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bc751-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc751-158">False</span><span class="sxs-lookup"><span data-stu-id="bc751-158">False</span></span>  <br/> |
   

