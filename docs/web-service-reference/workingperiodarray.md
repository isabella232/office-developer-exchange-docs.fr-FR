---
title: WorkingPeriodArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriodArray
api_type:
- schema
ms.assetid: 3a3f6393-eacc-4734-b6c9-b67023fe2830
description: L’élément WorkingPeriodArray contient des informations de période de travail pour l’utilisateur de boîte aux lettres.
ms.openlocfilehash: a9ca55866a574c5208d8561fca6daf417867fef6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465197"
---
# <a name="workingperiodarray"></a><span data-ttu-id="68269-103">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="68269-103">WorkingPeriodArray</span></span>

<span data-ttu-id="68269-104">L’élément **WorkingPeriodArray** contient des informations de période de travail pour l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="68269-104">The **WorkingPeriodArray** element contains working period information for the mailbox user.</span></span> 
  
[<span data-ttu-id="68269-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="68269-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="68269-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="68269-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="68269-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="68269-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="68269-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="68269-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="68269-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="68269-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="68269-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="68269-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
```xml
<WorkingPeriodArray>
   <WorkingPeriod>...</WorkingPeriod>
</WorkingPeriodArray>
```

 <span data-ttu-id="68269-111">**ArrayOfWorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="68269-111">**ArrayOfWorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68269-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="68269-112">Attributes and elements</span></span>

<span data-ttu-id="68269-113">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="68269-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68269-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="68269-114">Attributes</span></span>

<span data-ttu-id="68269-115">Aucune.</span><span class="sxs-lookup"><span data-stu-id="68269-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68269-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="68269-116">Child elements</span></span>

|<span data-ttu-id="68269-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="68269-117">**Element**</span></span>|<span data-ttu-id="68269-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="68269-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68269-119">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="68269-119">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="68269-120">Contient les jours et les heures de travail de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="68269-120">Contains the work week days and hours of the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68269-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="68269-121">Parent elements</span></span>

|<span data-ttu-id="68269-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="68269-122">**Element**</span></span>|<span data-ttu-id="68269-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="68269-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68269-124">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="68269-124">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="68269-125">Représente les paramètres de fuseau horaire et les heures de travail de l’utilisateur de boîte aux lettres demandé.</span><span class="sxs-lookup"><span data-stu-id="68269-125">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="68269-126">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="68269-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="68269-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="68269-127">Remarks</span></span>

<span data-ttu-id="68269-128">Cet élément est requis si l’élément [WorkingHours](workinghours-ex15websvcsotherref.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="68269-128">This element is required if the [WorkingHours](workinghours-ex15websvcsotherref.md) element is used.</span></span> <span data-ttu-id="68269-129">Tous les éléments enfants sont répertoriés dans l’ordre dans lequel ils se produisent.</span><span class="sxs-lookup"><span data-stu-id="68269-129">All the child elements are listed in the sequence in which they occur.</span></span> 
  
<span data-ttu-id="68269-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="68269-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68269-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="68269-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68269-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="68269-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="68269-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="68269-133">Schema Name</span></span>  <br/> |<span data-ttu-id="68269-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="68269-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="68269-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="68269-135">Validation File</span></span>  <br/> |<span data-ttu-id="68269-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="68269-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="68269-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="68269-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="68269-138">False</span><span class="sxs-lookup"><span data-stu-id="68269-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68269-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="68269-139">See also</span></span>



[<span data-ttu-id="68269-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="68269-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="68269-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="68269-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="68269-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="68269-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

