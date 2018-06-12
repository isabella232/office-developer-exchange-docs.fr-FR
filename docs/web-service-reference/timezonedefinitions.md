---
title: TimeZoneDefinitions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinitions
api_type:
- schema
ms.assetid: 9ca1584e-65b8-49ba-a408-e3e8597e6607
description: L’élément TimeZoneDefinitions représente un tableau des définitions de fuseau horaire.
ms.openlocfilehash: 0bc1b69ef564bb4e239d9845a4b1a0133292ff12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838726"
---
# <a name="timezonedefinitions"></a><span data-ttu-id="ad814-103">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="ad814-103">TimeZoneDefinitions</span></span>

<span data-ttu-id="ad814-104">L’élément **TimeZoneDefinitions** représente un tableau des définitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="ad814-104">The **TimeZoneDefinitions** element represents an array of time zone definitions.</span></span> 
  
```XML
<TimeZoneDefinitions>
   <TimeZoneDefinition/>
</TimeZoneDefinitions>
```

 <span data-ttu-id="ad814-105">**ArrayOfTimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="ad814-105">**ArrayOfTimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad814-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad814-106">Attributes and elements</span></span>

<span data-ttu-id="ad814-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad814-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad814-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad814-108">Attributes</span></span>

<span data-ttu-id="ad814-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad814-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad814-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad814-110">Child elements</span></span>

|<span data-ttu-id="ad814-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad814-111">**Element**</span></span>|<span data-ttu-id="ad814-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad814-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad814-113">Définition de fuseau horaire</span><span class="sxs-lookup"><span data-stu-id="ad814-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="ad814-114">Spécifie les périodes et les transitions qui définissent un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="ad814-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad814-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad814-115">Parent elements</span></span>

|<span data-ttu-id="ad814-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad814-116">**Element**</span></span>|<span data-ttu-id="ad814-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad814-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad814-118">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ad814-118">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="ad814-119">Contient l’état et les résultats d’une demande [d’opération GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ad814-119">Contains the status and result of a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ad814-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="ad814-120">Remarks</span></span>

<span data-ttu-id="ad814-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad814-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad814-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad814-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad814-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad814-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ad814-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad814-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ad814-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ad814-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ad814-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ad814-126">Validation File</span></span>  <br/> |<span data-ttu-id="ad814-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ad814-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ad814-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad814-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad814-129">False</span><span class="sxs-lookup"><span data-stu-id="ad814-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad814-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad814-130">See also</span></span>



- [<span data-ttu-id="ad814-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ad814-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

