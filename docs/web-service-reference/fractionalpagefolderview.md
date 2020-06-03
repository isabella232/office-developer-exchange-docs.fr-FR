---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: L’élément FractionalPageFolderView décrit l’emplacement où l’affichage paginé démarre et le nombre maximal de dossiers renvoyés dans une demande FindFolder.
ms.openlocfilehash: a8627c6277b49655d3933679128b844118633cda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463068"
---
# <a name="fractionalpagefolderview"></a><span data-ttu-id="a142c-103">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="a142c-103">FractionalPageFolderView</span></span>

<span data-ttu-id="a142c-104">L’élément **FractionalPageFolderView** décrit l’emplacement où l’affichage paginé démarre et le nombre maximal de dossiers renvoyés dans une demande [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="a142c-104">The **FractionalPageFolderView** element describes where the paged view starts and the maximum number of folders returned in a [FindFolder](findfolder.md) request.</span></span> 
  
[<span data-ttu-id="a142c-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="a142c-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="a142c-106">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="a142c-106">FractionalPageFolderView</span></span>](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="a142c-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="a142c-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a142c-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a142c-108">Attributes and elements</span></span>

<span data-ttu-id="a142c-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a142c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a142c-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="a142c-110">Attributes</span></span>

|<span data-ttu-id="a142c-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a142c-111">**Attribute**</span></span>|<span data-ttu-id="a142c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a142c-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a142c-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="a142c-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="a142c-114">Identifie le nombre maximal de résultats à renvoyer dans la réponse [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="a142c-114">Identifies the maximum number of results to return in the [FindFolder](findfolder.md) response.</span></span> <span data-ttu-id="a142c-115">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="a142c-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a142c-116">**Monnaie**</span><span class="sxs-lookup"><span data-stu-id="a142c-116">**Numerator**</span></span> <br/> |<span data-ttu-id="a142c-117">Représente le numérateur du décalage fractionnaire à partir du début du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="a142c-117">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="a142c-118">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="a142c-118">This attribute is required.</span></span> <span data-ttu-id="a142c-119">Le numérateur doit être inférieur ou égal au dénominateur.</span><span class="sxs-lookup"><span data-stu-id="a142c-119">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="a142c-120">Cet attribut doit représenter une valeur intégrale égale ou supérieure à zéro.</span><span class="sxs-lookup"><span data-stu-id="a142c-120">This attribute must represent an integral value that is equal to or greater than zero.</span></span> <span data-ttu-id="a142c-121">Pour plus d’informations, consultez la section Remarques plus loin dans cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="a142c-121">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="a142c-122">**Petit**</span><span class="sxs-lookup"><span data-stu-id="a142c-122">**Denominator**</span></span> <br/> |<span data-ttu-id="a142c-123">Représente le dénominateur du décalage fractionnaire à partir du début du nombre total de dossiers dans le jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="a142c-123">Represents the denominator of the fractional offset from the start of the total number of folders in the result set.</span></span> <span data-ttu-id="a142c-124">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="a142c-124">This attribute is required.</span></span> <span data-ttu-id="a142c-125">Cet attribut doit représenter une valeur intégrale supérieure à 1.</span><span class="sxs-lookup"><span data-stu-id="a142c-125">This attribute must represent an integral value that is greater than one.</span></span> <span data-ttu-id="a142c-126">Pour plus d’informations, consultez la section Remarques plus loin dans cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="a142c-126">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a142c-127">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a142c-127">Child elements</span></span>

<span data-ttu-id="a142c-128">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a142c-128">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a142c-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a142c-129">Parent elements</span></span>

|<span data-ttu-id="a142c-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a142c-130">**Element**</span></span>|<span data-ttu-id="a142c-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="a142c-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a142c-132">FindFolder</span><span class="sxs-lookup"><span data-stu-id="a142c-132">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="a142c-133">Définit une demande pour identifier les dossiers d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a142c-133">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="a142c-134">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="a142c-134">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a142c-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="a142c-135">Remarks</span></span>

<span data-ttu-id="a142c-136">Le décalage de l’affichage paginé à partir du début de l’ensemble des dossiers trouvés est décrit par une fraction.</span><span class="sxs-lookup"><span data-stu-id="a142c-136">The paged view offset from the start of the set of found folders is described by a fraction.</span></span> <span data-ttu-id="a142c-137">La fraction, définie par les attributs **numérateur** et **dénominateur** , décrit l’emplacement de début de la page d’informations.</span><span class="sxs-lookup"><span data-stu-id="a142c-137">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="a142c-138">Par exemple, si le **numérateur** est égal à quatre et que le **dénominateur** est égal à cinq, la page des informations retournées commence à une entrée située quatre cinquièmes du contenu du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="a142c-138">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="a142c-139">Si la fraction est égale à zéro, cela indique le début du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="a142c-139">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="a142c-140">Si la fraction est égale à 1, cela indique la fin du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="a142c-140">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="a142c-141">La fraction représente le point de départ de la page, pas le nombre de résultats dans le jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="a142c-141">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="a142c-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a142c-142">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a142c-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a142c-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a142c-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a142c-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a142c-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a142c-145">Schema Name</span></span>  <br/> |<span data-ttu-id="a142c-146">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a142c-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a142c-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a142c-147">Validation File</span></span>  <br/> |<span data-ttu-id="a142c-148">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a142c-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a142c-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a142c-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="a142c-150">False</span><span class="sxs-lookup"><span data-stu-id="a142c-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a142c-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a142c-151">See also</span></span>



[<span data-ttu-id="a142c-152">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="a142c-152">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="a142c-153">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="a142c-153">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

