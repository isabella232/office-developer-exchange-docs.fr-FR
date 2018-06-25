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
description: L’élément ResolutionSet contient un tableau des résolutions pour un nom ambigu.
ms.openlocfilehash: ad7bd31c85051e8c80aea25aa9e6f2914cf0ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829160"
---
# <a name="resolutionset"></a><span data-ttu-id="60247-103">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="60247-103">ResolutionSet</span></span>

<span data-ttu-id="60247-104">L’élément **ResolutionSet** contient un tableau des résolutions pour un nom ambigu.</span><span class="sxs-lookup"><span data-stu-id="60247-104">The **ResolutionSet** element contains an array of resolutions for an ambiguous name.</span></span> 
  
[<span data-ttu-id="60247-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="60247-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="60247-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="60247-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="60247-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="60247-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="60247-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="60247-108">ResolutionSet</span></span>](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 <span data-ttu-id="60247-109">**ArrayOfResolutionType**</span><span class="sxs-lookup"><span data-stu-id="60247-109">**ArrayOfResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60247-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="60247-110">Attributes and elements</span></span>

<span data-ttu-id="60247-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="60247-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60247-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="60247-112">Attributes</span></span>

|<span data-ttu-id="60247-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="60247-113">**Attribute**</span></span>|<span data-ttu-id="60247-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="60247-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="60247-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="60247-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="60247-116">Représente l’index suivant doit être utilisé pour la requête suivante lorsque vous utilisez un affichage de page indexés.</span><span class="sxs-lookup"><span data-stu-id="60247-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="60247-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="60247-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="60247-118">Représente la nouvelle valeur numérateur à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fraction.</span><span class="sxs-lookup"><span data-stu-id="60247-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="60247-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="60247-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="60247-120">Représente le dénominateur suivant à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fraction.</span><span class="sxs-lookup"><span data-stu-id="60247-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="60247-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="60247-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="60247-122">Cet attribut sera la valeur true si le résultat actuel contient le dernier élément dans la requête, afin que le fichier d’échange supplémentaire n’est pas nécessaire.</span><span class="sxs-lookup"><span data-stu-id="60247-122">This attribute will be true if the current results contain the last item in the query, so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="60247-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="60247-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="60247-124">Représente le nombre total d’éléments dans l’affichage.</span><span class="sxs-lookup"><span data-stu-id="60247-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="60247-125">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="60247-125">Child elements</span></span>

|<span data-ttu-id="60247-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="60247-126">**Element**</span></span>|<span data-ttu-id="60247-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="60247-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60247-128">Solution</span><span class="sxs-lookup"><span data-stu-id="60247-128">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="60247-129">Contient une seule entité résolue.</span><span class="sxs-lookup"><span data-stu-id="60247-129">Contains a single resolved entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60247-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="60247-130">Parent elements</span></span>

|<span data-ttu-id="60247-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="60247-131">**Element**</span></span>|<span data-ttu-id="60247-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="60247-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60247-133">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="60247-133">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md) <br/> |<span data-ttu-id="60247-134">Contient l’état et les résultats d’une demande ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="60247-134">Contains the status and result of a ResolveNames request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="60247-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="60247-135">Remarks</span></span>

<span data-ttu-id="60247-136">Un élément **ResolutionSet** peut contenir un maximum de 100 entités résolus.</span><span class="sxs-lookup"><span data-stu-id="60247-136">A **ResolutionSet** element can contain a maximum of 100 resolved entities.</span></span> 
  
<span data-ttu-id="60247-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="60247-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60247-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="60247-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60247-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="60247-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="60247-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="60247-140">Schema Name</span></span>  <br/> |<span data-ttu-id="60247-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="60247-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="60247-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="60247-142">Validation File</span></span>  <br/> |<span data-ttu-id="60247-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="60247-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="60247-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="60247-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="60247-145">False</span><span class="sxs-lookup"><span data-stu-id="60247-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60247-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="60247-146">See also</span></span>



[<span data-ttu-id="60247-147">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="60247-147">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="60247-148">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="60247-148">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="60247-149">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="60247-149">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="60247-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="60247-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

