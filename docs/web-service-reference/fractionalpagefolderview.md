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
description: L’élément FractionalPageFolderView décrit où l’affichage paginé démarre et le nombre maximal de dossiers renvoyées dans une requête FindFolder.
ms.openlocfilehash: 3cb5f8333634a0c484ae3ce6a6256631cff57cc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756473"
---
# <a name="fractionalpagefolderview"></a><span data-ttu-id="d05ac-103">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="d05ac-103">FractionalPageFolderView</span></span>

<span data-ttu-id="d05ac-104">L’élément **FractionalPageFolderView** décrit où l’affichage paginé démarre et le nombre maximal de dossiers renvoyées dans une requête [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="d05ac-104">The **FractionalPageFolderView** element describes where the paged view starts and the maximum number of folders returned in a [FindFolder](findfolder.md) request.</span></span> 
  
[<span data-ttu-id="d05ac-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="d05ac-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="d05ac-106">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="d05ac-106">FractionalPageFolderView</span></span>](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="d05ac-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="d05ac-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d05ac-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d05ac-108">Attributes and elements</span></span>

<span data-ttu-id="d05ac-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d05ac-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d05ac-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d05ac-110">Attributes</span></span>

|<span data-ttu-id="d05ac-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d05ac-111">**Attribute**</span></span>|<span data-ttu-id="d05ac-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d05ac-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d05ac-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="d05ac-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="d05ac-114">Identifie le nombre maximal de résultats à retourner dans la réponse [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="d05ac-114">Identifies the maximum number of results to return in the [FindFolder](findfolder.md) response.</span></span> <span data-ttu-id="d05ac-115">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d05ac-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="d05ac-116">**Numérateur**</span><span class="sxs-lookup"><span data-stu-id="d05ac-116">**Numerator**</span></span> <br/> |<span data-ttu-id="d05ac-117">Représente le numérateur du décalage en fraction à partir du début du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="d05ac-117">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="d05ac-118">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="d05ac-118">This attribute is required.</span></span> <span data-ttu-id="d05ac-119">Le numérateur doit être le dénominateur inférieur ou égal à.</span><span class="sxs-lookup"><span data-stu-id="d05ac-119">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="d05ac-120">Cet attribut doit représenter une valeur intégrale est égale ou supérieure à zéro.</span><span class="sxs-lookup"><span data-stu-id="d05ac-120">This attribute must represent an integral value that is equal to or greater than zero.</span></span> <span data-ttu-id="d05ac-121">Pour plus d’informations, voir les remarques plus loin dans cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="d05ac-121">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="d05ac-122">**Dénominateur**</span><span class="sxs-lookup"><span data-stu-id="d05ac-122">**Denominator**</span></span> <br/> |<span data-ttu-id="d05ac-123">Représente le dénominateur de décalage fractionnaire à partir du début du nombre total de dossiers dans le jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="d05ac-123">Represents the denominator of the fractional offset from the start of the total number of folders in the result set.</span></span> <span data-ttu-id="d05ac-124">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="d05ac-124">This attribute is required.</span></span> <span data-ttu-id="d05ac-125">Cet attribut doit représenter une valeur intégrale qui est supérieure à 1.</span><span class="sxs-lookup"><span data-stu-id="d05ac-125">This attribute must represent an integral value that is greater than one.</span></span> <span data-ttu-id="d05ac-126">Pour plus d’informations, voir les remarques plus loin dans cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="d05ac-126">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d05ac-127">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d05ac-127">Child elements</span></span>

<span data-ttu-id="d05ac-128">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d05ac-128">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d05ac-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d05ac-129">Parent elements</span></span>

|<span data-ttu-id="d05ac-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d05ac-130">**Element**</span></span>|<span data-ttu-id="d05ac-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="d05ac-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d05ac-132">FindFolder</span><span class="sxs-lookup"><span data-stu-id="d05ac-132">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="d05ac-133">Définit une demande pour identifier les dossiers dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d05ac-133">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="d05ac-134">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="d05ac-134">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d05ac-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="d05ac-135">Remarks</span></span>

<span data-ttu-id="d05ac-136">Le décalage d’affichage paginé à partir du début de l’ensemble des dossiers trouvés est décrit par une fraction.</span><span class="sxs-lookup"><span data-stu-id="d05ac-136">The paged view offset from the start of the set of found folders is described by a fraction.</span></span> <span data-ttu-id="d05ac-137">La fraction, qui est définie par les attributs **numérateur** et **dénominateur** , décrit où démarre la page d’informations.</span><span class="sxs-lookup"><span data-stu-id="d05ac-137">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="d05ac-138">Par exemple, si **numérateur** est égale à quatre et **dénominateur** est égal à 5, la page d’informations renvoyées commence une entrée trouve quatre cinquièmes de la manière dans le jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="d05ac-138">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="d05ac-139">Si la fraction correspond à zéro, qui indique le début du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="d05ac-139">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="d05ac-140">Si la fraction a la valeur 1, qui indique la fin du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="d05ac-140">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="d05ac-141">La fraction représente le point de départ de la page, pas le nombre de résultats dans le jeu de résultats s’afficheront.</span><span class="sxs-lookup"><span data-stu-id="d05ac-141">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="d05ac-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d05ac-142">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d05ac-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d05ac-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d05ac-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d05ac-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d05ac-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d05ac-145">Schema Name</span></span>  <br/> |<span data-ttu-id="d05ac-146">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d05ac-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d05ac-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d05ac-147">Validation File</span></span>  <br/> |<span data-ttu-id="d05ac-148">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d05ac-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d05ac-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d05ac-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="d05ac-150">False</span><span class="sxs-lookup"><span data-stu-id="d05ac-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d05ac-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d05ac-151">See also</span></span>



[<span data-ttu-id="d05ac-152">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="d05ac-152">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="d05ac-153">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="d05ac-153">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

