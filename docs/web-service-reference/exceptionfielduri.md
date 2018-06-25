---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: L’élément ExceptionFieldURI identifie les erreurs spécifiques dans une requête. Cet élément est utilisé uniquement dans le cadre d’une réponse d’erreur dans le nœud MessageXml.
ms.openlocfilehash: 79909405179cec0d0b86ad12bf52031e1daeb790
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756234"
---
# <a name="exceptionfielduri"></a><span data-ttu-id="aba4f-104">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="aba4f-104">ExceptionFieldURI</span></span>

<span data-ttu-id="aba4f-105">L’élément **ExceptionFieldURI** identifie les erreurs spécifiques dans une requête.</span><span class="sxs-lookup"><span data-stu-id="aba4f-105">The **ExceptionFieldURI** element identifies particular errors in a request.</span></span> <span data-ttu-id="aba4f-106">Cet élément est utilisé uniquement dans le cadre d’une réponse d’erreur dans le nœud [MessageXml](messagexml.md) .</span><span class="sxs-lookup"><span data-stu-id="aba4f-106">This element is only used as part of an error response in the [MessageXml](messagexml.md) node.</span></span> 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 <span data-ttu-id="aba4f-107">**ExceptionPropertyURIType**</span><span class="sxs-lookup"><span data-stu-id="aba4f-107">**ExceptionPropertyURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aba4f-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aba4f-108">Attributes and elements</span></span>

<span data-ttu-id="aba4f-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aba4f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aba4f-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="aba4f-110">Attributes</span></span>

|<span data-ttu-id="aba4f-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="aba4f-111">**Attribute**</span></span>|<span data-ttu-id="aba4f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="aba4f-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aba4f-113">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="aba4f-113">**FieldURI**</span></span> <br/> |<span data-ttu-id="aba4f-114">Identifie une propriété d’une occurrence d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="aba4f-114">Identifies a property of an occurrence of a recurring item.</span></span> <span data-ttu-id="aba4f-115">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="aba4f-115">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="aba4f-116">Attribut FieldURI</span><span class="sxs-lookup"><span data-stu-id="aba4f-116">FieldURI Attribute</span></span>

|<span data-ttu-id="aba4f-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="aba4f-117">**Value**</span></span>|<span data-ttu-id="aba4f-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="aba4f-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aba4f-119">Nom de la pièce jointe :</span><span class="sxs-lookup"><span data-stu-id="aba4f-119">attachment:Name</span></span>  <br/> |<span data-ttu-id="aba4f-120">Identifie le nom de la pièce jointe comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="aba4f-120">Identifies the attachment name as containing an error.</span></span>  <br/> |
|<span data-ttu-id="aba4f-121">pièce jointe : ContentType</span><span class="sxs-lookup"><span data-stu-id="aba4f-121">attachment:ContentType</span></span>  <br/> |<span data-ttu-id="aba4f-122">Identifie le type de contenu comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="aba4f-122">Identifies the content type as containing an error.</span></span>  <br/> |
|<span data-ttu-id="aba4f-123">Contenu des pièces jointes :</span><span class="sxs-lookup"><span data-stu-id="aba4f-123">attachment:Content</span></span>  <br/> |<span data-ttu-id="aba4f-124">Identifie le contenu comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="aba4f-124">Identifies the content as containing an error.</span></span>  <br/> |
|<span data-ttu-id="aba4f-125">Mois de périodicité :</span><span class="sxs-lookup"><span data-stu-id="aba4f-125">recurrence:Month</span></span>  <br/> |<span data-ttu-id="aba4f-126">Identifie le champ mois comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="aba4f-126">Identifies the month field as containing an error.</span></span>  <br/> |
|<span data-ttu-id="aba4f-127">Périodicité : DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="aba4f-127">recurrence:DayOfWeekIndex</span></span>  <br/> |<span data-ttu-id="aba4f-128">Identifie le jour de l’index de semaine comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="aba4f-128">Identifies the day of week index as containing an error.</span></span>  <br/> |
|<span data-ttu-id="aba4f-129">Périodicité : DaysOfWeek</span><span class="sxs-lookup"><span data-stu-id="aba4f-129">recurrence:DaysOfWeek</span></span>  <br/> |<span data-ttu-id="aba4f-130">Identifie la propriété DaysOfWeek comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="aba4f-130">Identifies the DaysOfWeek property as containing an error.</span></span>  <br/> |
|<span data-ttu-id="aba4f-131">Périodicité : DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="aba4f-131">recurrence:DayOfMonth</span></span>  <br/> |<span data-ttu-id="aba4f-132">Identifie le DayOfMonth comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="aba4f-132">Identifies the DayOfMonth as containing an error.</span></span>  <br/> |
|<span data-ttu-id="aba4f-133">Intervalle de périodicité :</span><span class="sxs-lookup"><span data-stu-id="aba4f-133">recurrence:Interval</span></span>  <br/> |<span data-ttu-id="aba4f-134">Identifie l’intervalle comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="aba4f-134">Identifies the interval as containing an error.</span></span>  <br/> |
|<span data-ttu-id="aba4f-135">Périodicité : NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="aba4f-135">recurrence:NumberOfOccurrences</span></span>  <br/> |<span data-ttu-id="aba4f-136">Identifie le nombre d’occurrences comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="aba4f-136">Identifies the number of occurrences as containing an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="aba4f-137">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aba4f-137">Child elements</span></span>

<span data-ttu-id="aba4f-138">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aba4f-138">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aba4f-139">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aba4f-139">Parent elements</span></span>

|<span data-ttu-id="aba4f-140">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aba4f-140">**Element**</span></span>|<span data-ttu-id="aba4f-141">**Description**</span><span class="sxs-lookup"><span data-stu-id="aba4f-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aba4f-142">MessageXml</span><span class="sxs-lookup"><span data-stu-id="aba4f-142">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="aba4f-143">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="aba4f-143">Provides additional error response information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aba4f-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="aba4f-144">Remarks</span></span>

<span data-ttu-id="aba4f-145">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="aba4f-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aba4f-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aba4f-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aba4f-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aba4f-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aba4f-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aba4f-148">Schema Name</span></span>  <br/> |<span data-ttu-id="aba4f-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="aba4f-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="aba4f-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="aba4f-150">Validation File</span></span>  <br/> |<span data-ttu-id="aba4f-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aba4f-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aba4f-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aba4f-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="aba4f-153">False</span><span class="sxs-lookup"><span data-stu-id="aba4f-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aba4f-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aba4f-154">See also</span></span>



- [<span data-ttu-id="aba4f-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="aba4f-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

