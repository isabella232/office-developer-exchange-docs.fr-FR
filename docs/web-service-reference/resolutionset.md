---
title: ResolutionSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolutionSet
api_type:
- schema
ms.assetid: 43d5b876-0e87-4414-9b1d-bff1c1ec825c
description: L’élément ResolutionSet contient un tableau de résolutions pour un nom ambigu.
ms.openlocfilehash: 483a096a7fcedbabe25758ebcaa31c83405a0ad4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467171"
---
# <a name="resolutionset"></a><span data-ttu-id="76288-103">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="76288-103">ResolutionSet</span></span>

<span data-ttu-id="76288-104">L’élément **ResolutionSet** contient un tableau de résolutions pour un nom ambigu.</span><span class="sxs-lookup"><span data-stu-id="76288-104">The **ResolutionSet** element contains an array of resolutions for an ambiguous name.</span></span> 
  
[<span data-ttu-id="76288-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="76288-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="76288-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="76288-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="76288-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76288-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="76288-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="76288-108">ResolutionSet</span></span>](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 <span data-ttu-id="76288-109">**ArrayOfResolutionType**</span><span class="sxs-lookup"><span data-stu-id="76288-109">**ArrayOfResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76288-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="76288-110">Attributes and elements</span></span>

<span data-ttu-id="76288-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="76288-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76288-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="76288-112">Attributes</span></span>

|<span data-ttu-id="76288-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="76288-113">**Attribute**</span></span>|<span data-ttu-id="76288-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="76288-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="76288-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="76288-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="76288-116">Représente l’index suivant qui doit être utilisé pour la requête suivante lorsque vous utilisez une vue de page indexée.</span><span class="sxs-lookup"><span data-stu-id="76288-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="76288-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="76288-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="76288-118">Représente la nouvelle valeur de numérateur à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fractions.</span><span class="sxs-lookup"><span data-stu-id="76288-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="76288-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="76288-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="76288-120">Représente le dénominateur suivant à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fractions.</span><span class="sxs-lookup"><span data-stu-id="76288-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="76288-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="76288-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="76288-122">Cet attribut est true si les résultats actuels contiennent le dernier élément de la requête, afin que la pagination supplémentaire ne soit pas nécessaire.</span><span class="sxs-lookup"><span data-stu-id="76288-122">This attribute will be true if the current results contain the last item in the query, so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="76288-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="76288-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="76288-124">Représente le nombre total d’éléments dans l’affichage.</span><span class="sxs-lookup"><span data-stu-id="76288-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="76288-125">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="76288-125">Child elements</span></span>

|<span data-ttu-id="76288-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="76288-126">**Element**</span></span>|<span data-ttu-id="76288-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="76288-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76288-128">Solution</span><span class="sxs-lookup"><span data-stu-id="76288-128">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="76288-129">Contient une seule entité résolue.</span><span class="sxs-lookup"><span data-stu-id="76288-129">Contains a single resolved entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76288-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="76288-130">Parent elements</span></span>

|<span data-ttu-id="76288-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="76288-131">**Element**</span></span>|<span data-ttu-id="76288-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="76288-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76288-133">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76288-133">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md) <br/> |<span data-ttu-id="76288-134">Contient l’État et le résultat d’une demande ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="76288-134">Contains the status and result of a ResolveNames request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="76288-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="76288-135">Remarks</span></span>

<span data-ttu-id="76288-136">Un élément **ResolutionSet** peut contenir un maximum de 100 entités résolues.</span><span class="sxs-lookup"><span data-stu-id="76288-136">A **ResolutionSet** element can contain a maximum of 100 resolved entities.</span></span> 
  
<span data-ttu-id="76288-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="76288-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76288-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="76288-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76288-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="76288-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="76288-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="76288-140">Schema Name</span></span>  <br/> |<span data-ttu-id="76288-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="76288-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="76288-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="76288-142">Validation File</span></span>  <br/> |<span data-ttu-id="76288-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="76288-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="76288-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="76288-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="76288-145">False</span><span class="sxs-lookup"><span data-stu-id="76288-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76288-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="76288-146">See also</span></span>



[<span data-ttu-id="76288-147">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="76288-147">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="76288-148">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="76288-148">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="76288-149">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="76288-149">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="76288-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="76288-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

