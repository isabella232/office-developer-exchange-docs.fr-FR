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
description: L’élément IndexedPageFolderView décrit comment les informations d’élément paginé sont renvoyées dans une réponse FindFolder.
ms.openlocfilehash: 6e9e2796c0bdcd9a15487f0e1bc7cbdf09d0a492
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457199"
---
# <a name="indexedpagefolderview"></a><span data-ttu-id="16660-103">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="16660-103">IndexedPageFolderView</span></span>

<span data-ttu-id="16660-104">L’élément **IndexedPageFolderView** décrit comment les informations d’élément paginé sont renvoyées dans une réponse [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="16660-104">The **IndexedPageFolderView** element describes how paged item information is returned in a [FindFolder](findfolder.md) response.</span></span> 
  
[<span data-ttu-id="16660-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="16660-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="16660-106">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="16660-106">IndexedPageFolderView</span></span>](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 <span data-ttu-id="16660-107">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="16660-107">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16660-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="16660-108">Attributes and elements</span></span>

<span data-ttu-id="16660-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="16660-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16660-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="16660-110">Attributes</span></span>

|<span data-ttu-id="16660-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="16660-111">**Attribute**</span></span>|<span data-ttu-id="16660-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="16660-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16660-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="16660-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="16660-114">Décrit le nombre maximal de dossiers à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="16660-114">Describes the maximum number of folders to return in the response.</span></span> <span data-ttu-id="16660-115">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="16660-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="16660-116">**Offset**</span><span class="sxs-lookup"><span data-stu-id="16660-116">**Offset**</span></span> <br/> |<span data-ttu-id="16660-117">Décrit le décalage par rapport à l' **BasePoint**.</span><span class="sxs-lookup"><span data-stu-id="16660-117">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="16660-118">Offset doit être supérieur ou égal à zéro.</span><span class="sxs-lookup"><span data-stu-id="16660-118">Offset must be greater than or equal to zero.</span></span> <span data-ttu-id="16660-119">Si **BasePoint** est égal à début, le décalage est positif.</span><span class="sxs-lookup"><span data-stu-id="16660-119">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="16660-120">Si **BasePoint** est égal à fin, le décalage est géré comme s’il était négatif.</span><span class="sxs-lookup"><span data-stu-id="16660-120">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span>  <br/> <span data-ttu-id="16660-121">Cela identifie le dossier qui sera le premier dossier remis dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="16660-121">This identifies which folder will be the first folder delivered in the response.</span></span> <span data-ttu-id="16660-122">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="16660-122">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="16660-123">**BasePoint**</span><span class="sxs-lookup"><span data-stu-id="16660-123">**BasePoint**</span></span> <br/> |<span data-ttu-id="16660-124">Indique si la page de dossiers commence à partir du début ou de la fin de l’ensemble des dossiers trouvés avec les critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="16660-124">Describes whether the page of folders will start from the start or the end of the set of folders that are found with the search criteria.</span></span> <span data-ttu-id="16660-125">La recherche à partir de la fin effectue toujours des recherches vers l’arrière.</span><span class="sxs-lookup"><span data-stu-id="16660-125">Seeking from the end always searches backward.</span></span> <span data-ttu-id="16660-126">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="16660-126">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="16660-127">Attribut BasePoint</span><span class="sxs-lookup"><span data-stu-id="16660-127">BasePoint Attribute</span></span>

|<span data-ttu-id="16660-128">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="16660-128">**Value**</span></span>|<span data-ttu-id="16660-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="16660-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16660-130">Entam</span><span class="sxs-lookup"><span data-stu-id="16660-130">Beginning</span></span>  <br/> |<span data-ttu-id="16660-131">L’affichage paginé commence au début de l’ensemble de dossiers trouvé.</span><span class="sxs-lookup"><span data-stu-id="16660-131">The paged view starts at the beginning of the found folder set.</span></span>  <br/> |
|<span data-ttu-id="16660-132">End</span><span class="sxs-lookup"><span data-stu-id="16660-132">End</span></span>  <br/> |<span data-ttu-id="16660-133">La vue paginée commence à la fin de l’ensemble de dossiers trouvé.</span><span class="sxs-lookup"><span data-stu-id="16660-133">The paged view starts at the end of the found folder set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="16660-134">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="16660-134">Child elements</span></span>

<span data-ttu-id="16660-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="16660-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16660-136">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="16660-136">Parent elements</span></span>

|<span data-ttu-id="16660-137">**Élément**</span><span class="sxs-lookup"><span data-stu-id="16660-137">**Element**</span></span>|<span data-ttu-id="16660-138">**Description**</span><span class="sxs-lookup"><span data-stu-id="16660-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16660-139">FindFolder</span><span class="sxs-lookup"><span data-stu-id="16660-139">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="16660-140">Définit une demande de recherche de dossiers dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="16660-140">Defines a request to find folders in a mailbox.</span></span>  <br/> <span data-ttu-id="16660-141">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="16660-141">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="16660-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="16660-142">Remarks</span></span>

<span data-ttu-id="16660-143">La recherche de end implique le passage à l’origine identifiée par le décalage.</span><span class="sxs-lookup"><span data-stu-id="16660-143">Seeking from end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="16660-144">De plus, le pointeur est ramené par le nombre d’enregistrements demandés.</span><span class="sxs-lookup"><span data-stu-id="16660-144">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="16660-145">Par exemple, s’il y a 100 enregistrements et que le décalage est de 25 à partir de la fin, la recherche commence à partir de 75.</span><span class="sxs-lookup"><span data-stu-id="16660-145">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="16660-146">Si 10 enregistrements sont renvoyés, le pointeur de la souris recule de 10 enregistrements supplémentaires sur 65 et renvoie les enregistrements 65 à 75.</span><span class="sxs-lookup"><span data-stu-id="16660-146">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="16660-147">L’index suivant est 64.</span><span class="sxs-lookup"><span data-stu-id="16660-147">The next index is 64.</span></span> <span data-ttu-id="16660-148">Le prochain décalage par rapport à la fin d’une page est de 100 moins 64, ce qui équivaut à 36.</span><span class="sxs-lookup"><span data-stu-id="16660-148">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="16660-149">La valeur du décalage suivant à partir de la fin pour obtenir la page indexée suivante est 36.</span><span class="sxs-lookup"><span data-stu-id="16660-149">The value for the next offset from the end to get the next indexed page is 36.</span></span>
  
<span data-ttu-id="16660-150">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="16660-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16660-151">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="16660-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16660-152">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="16660-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="16660-153">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="16660-153">Schema Name</span></span>  <br/> |<span data-ttu-id="16660-154">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="16660-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="16660-155">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="16660-155">Validation File</span></span>  <br/> |<span data-ttu-id="16660-156">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="16660-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="16660-157">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="16660-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="16660-158">False</span><span class="sxs-lookup"><span data-stu-id="16660-158">False</span></span>  <br/> |
   

