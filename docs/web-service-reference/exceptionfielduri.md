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
description: L’élément ExceptionFieldURI identifie les erreurs particulières dans une demande. Cet élément est utilisé uniquement dans le cadre d’une réponse d’erreur dans le nœud MessageXml.
ms.openlocfilehash: a47d44098f85d8bacb1e7a2c48a33e478e56c7ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454343"
---
# <a name="exceptionfielduri"></a><span data-ttu-id="9e388-104">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="9e388-104">ExceptionFieldURI</span></span>

<span data-ttu-id="9e388-105">L’élément **ExceptionFieldURI** identifie les erreurs particulières dans une demande.</span><span class="sxs-lookup"><span data-stu-id="9e388-105">The **ExceptionFieldURI** element identifies particular errors in a request.</span></span> <span data-ttu-id="9e388-106">Cet élément est utilisé uniquement dans le cadre d’une réponse d’erreur dans le nœud [messagexml](messagexml.md) .</span><span class="sxs-lookup"><span data-stu-id="9e388-106">This element is only used as part of an error response in the [MessageXml](messagexml.md) node.</span></span> 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 <span data-ttu-id="9e388-107">**ExceptionPropertyURIType**</span><span class="sxs-lookup"><span data-stu-id="9e388-107">**ExceptionPropertyURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e388-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9e388-108">Attributes and elements</span></span>

<span data-ttu-id="9e388-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9e388-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e388-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="9e388-110">Attributes</span></span>

|<span data-ttu-id="9e388-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="9e388-111">**Attribute**</span></span>|<span data-ttu-id="9e388-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9e388-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9e388-113">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="9e388-113">**FieldURI**</span></span> <br/> |<span data-ttu-id="9e388-114">Identifie une propriété d’une occurrence d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="9e388-114">Identifies a property of an occurrence of a recurring item.</span></span> <span data-ttu-id="9e388-115">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="9e388-115">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="9e388-116">Attribut FieldURI</span><span class="sxs-lookup"><span data-stu-id="9e388-116">FieldURI Attribute</span></span>

|<span data-ttu-id="9e388-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="9e388-117">**Value**</span></span>|<span data-ttu-id="9e388-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="9e388-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9e388-119">pièce jointe : nom</span><span class="sxs-lookup"><span data-stu-id="9e388-119">attachment:Name</span></span>  <br/> |<span data-ttu-id="9e388-120">Identifie le nom de la pièce jointe comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="9e388-120">Identifies the attachment name as containing an error.</span></span>  <br/> |
|<span data-ttu-id="9e388-121">pièce jointe : ContentType</span><span class="sxs-lookup"><span data-stu-id="9e388-121">attachment:ContentType</span></span>  <br/> |<span data-ttu-id="9e388-122">Identifie le type de contenu comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="9e388-122">Identifies the content type as containing an error.</span></span>  <br/> |
|<span data-ttu-id="9e388-123">pièce jointe : contenu</span><span class="sxs-lookup"><span data-stu-id="9e388-123">attachment:Content</span></span>  <br/> |<span data-ttu-id="9e388-124">Identifie le contenu comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="9e388-124">Identifies the content as containing an error.</span></span>  <br/> |
|<span data-ttu-id="9e388-125">Périodicité : mois</span><span class="sxs-lookup"><span data-stu-id="9e388-125">recurrence:Month</span></span>  <br/> |<span data-ttu-id="9e388-126">Identifie le champ de mois comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="9e388-126">Identifies the month field as containing an error.</span></span>  <br/> |
|<span data-ttu-id="9e388-127">Périodicité : DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="9e388-127">recurrence:DayOfWeekIndex</span></span>  <br/> |<span data-ttu-id="9e388-128">Identifie l’index du jour de la semaine comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="9e388-128">Identifies the day of week index as containing an error.</span></span>  <br/> |
|<span data-ttu-id="9e388-129">Périodicité : DaysOfWeek</span><span class="sxs-lookup"><span data-stu-id="9e388-129">recurrence:DaysOfWeek</span></span>  <br/> |<span data-ttu-id="9e388-130">Identifie la propriété DaysOfWeek comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="9e388-130">Identifies the DaysOfWeek property as containing an error.</span></span>  <br/> |
|<span data-ttu-id="9e388-131">Périodicité : DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="9e388-131">recurrence:DayOfMonth</span></span>  <br/> |<span data-ttu-id="9e388-132">Identifie le DayOfMonth comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="9e388-132">Identifies the DayOfMonth as containing an error.</span></span>  <br/> |
|<span data-ttu-id="9e388-133">Périodicité : intervalle</span><span class="sxs-lookup"><span data-stu-id="9e388-133">recurrence:Interval</span></span>  <br/> |<span data-ttu-id="9e388-134">Identifie l’intervalle comme contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="9e388-134">Identifies the interval as containing an error.</span></span>  <br/> |
|<span data-ttu-id="9e388-135">Périodicité : NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="9e388-135">recurrence:NumberOfOccurrences</span></span>  <br/> |<span data-ttu-id="9e388-136">Identifie le nombre d’occurrences contenant une erreur.</span><span class="sxs-lookup"><span data-stu-id="9e388-136">Identifies the number of occurrences as containing an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9e388-137">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9e388-137">Child elements</span></span>

<span data-ttu-id="9e388-138">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9e388-138">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9e388-139">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9e388-139">Parent elements</span></span>

|<span data-ttu-id="9e388-140">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9e388-140">**Element**</span></span>|<span data-ttu-id="9e388-141">**Description**</span><span class="sxs-lookup"><span data-stu-id="9e388-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e388-142">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9e388-142">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9e388-143">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="9e388-143">Provides additional error response information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9e388-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="9e388-144">Remarks</span></span>

<span data-ttu-id="9e388-145">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9e388-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e388-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9e388-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e388-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9e388-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e388-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9e388-148">Schema Name</span></span>  <br/> |<span data-ttu-id="9e388-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9e388-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="9e388-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9e388-150">Validation File</span></span>  <br/> |<span data-ttu-id="9e388-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9e388-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9e388-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9e388-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e388-153">False</span><span class="sxs-lookup"><span data-stu-id="9e388-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e388-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9e388-154">See also</span></span>



- [<span data-ttu-id="9e388-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9e388-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

