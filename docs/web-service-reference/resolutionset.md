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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829160"
---
# <a name="resolutionset"></a><span data-ttu-id="61a61-103">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="61a61-103">ResolutionSet</span></span>

<span data-ttu-id="61a61-104">L’élément **ResolutionSet** contient un tableau des résolutions pour un nom ambigu.</span><span class="sxs-lookup"><span data-stu-id="61a61-104">The **ResolutionSet** element contains an array of resolutions for an ambiguous name.</span></span> 
  
[<span data-ttu-id="61a61-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="61a61-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="61a61-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="61a61-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="61a61-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="61a61-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="61a61-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="61a61-108">ResolutionSet</span></span>](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 <span data-ttu-id="61a61-109">**ArrayOfResolutionType**</span><span class="sxs-lookup"><span data-stu-id="61a61-109">**ArrayOfResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61a61-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="61a61-110">Attributes and elements</span></span>

<span data-ttu-id="61a61-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="61a61-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61a61-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="61a61-112">Attributes</span></span>

|<span data-ttu-id="61a61-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="61a61-113">**Attribute**</span></span>|<span data-ttu-id="61a61-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="61a61-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="61a61-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="61a61-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="61a61-116">Représente l’index suivant doit être utilisé pour la requête suivante lorsque vous utilisez un affichage de page indexés.</span><span class="sxs-lookup"><span data-stu-id="61a61-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="61a61-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="61a61-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="61a61-118">Représente la nouvelle valeur numérateur à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fraction.</span><span class="sxs-lookup"><span data-stu-id="61a61-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="61a61-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="61a61-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="61a61-120">Représente le dénominateur suivant à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fraction.</span><span class="sxs-lookup"><span data-stu-id="61a61-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="61a61-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="61a61-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="61a61-122">Cet attribut sera la valeur true si le résultat actuel contient le dernier élément dans la requête, afin que le fichier d’échange supplémentaire n’est pas nécessaire.</span><span class="sxs-lookup"><span data-stu-id="61a61-122">This attribute will be true if the current results contain the last item in the query, so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="61a61-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="61a61-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="61a61-124">Représente le nombre total d’éléments dans l’affichage.</span><span class="sxs-lookup"><span data-stu-id="61a61-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="61a61-125">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="61a61-125">Child elements</span></span>

|<span data-ttu-id="61a61-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="61a61-126">**Element**</span></span>|<span data-ttu-id="61a61-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="61a61-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61a61-128">Solution</span><span class="sxs-lookup"><span data-stu-id="61a61-128">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="61a61-129">Contient une seule entité résolue.</span><span class="sxs-lookup"><span data-stu-id="61a61-129">Contains a single resolved entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="61a61-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="61a61-130">Parent elements</span></span>

|<span data-ttu-id="61a61-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="61a61-131">**Element**</span></span>|<span data-ttu-id="61a61-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="61a61-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61a61-133">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="61a61-133">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md) <br/> |<span data-ttu-id="61a61-134">Contient l’état et les résultats d’une demande ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="61a61-134">Contains the status and result of a ResolveNames request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="61a61-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="61a61-135">Remarks</span></span>

<span data-ttu-id="61a61-136">Un élément **ResolutionSet** peut contenir un maximum de 100 entités résolus.</span><span class="sxs-lookup"><span data-stu-id="61a61-136">A **ResolutionSet** element can contain a maximum of 100 resolved entities.</span></span> 
  
<span data-ttu-id="61a61-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="61a61-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61a61-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="61a61-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61a61-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="61a61-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="61a61-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="61a61-140">Schema Name</span></span>  <br/> |<span data-ttu-id="61a61-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="61a61-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="61a61-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="61a61-142">Validation File</span></span>  <br/> |<span data-ttu-id="61a61-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="61a61-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="61a61-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="61a61-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="61a61-145">False</span><span class="sxs-lookup"><span data-stu-id="61a61-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61a61-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="61a61-146">See also</span></span>



[<span data-ttu-id="61a61-147">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="61a61-147">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="61a61-148">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="61a61-148">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="61a61-149">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="61a61-149">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="61a61-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="61a61-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

