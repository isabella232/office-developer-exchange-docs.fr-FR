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
description: L’élément TimeZoneDefinitions représente un tableau de définitions de fuseau horaire.
ms.openlocfilehash: 16a25eb4fdcad2554ebd19626d0a0bc7f6391ac5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468760"
---
# <a name="timezonedefinitions"></a><span data-ttu-id="995c7-103">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="995c7-103">TimeZoneDefinitions</span></span>

<span data-ttu-id="995c7-104">L’élément **TimeZoneDefinitions** représente un tableau de définitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="995c7-104">The **TimeZoneDefinitions** element represents an array of time zone definitions.</span></span> 
  
```XML
<TimeZoneDefinitions>
   <TimeZoneDefinition/>
</TimeZoneDefinitions>
```

 <span data-ttu-id="995c7-105">**ArrayOfTimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="995c7-105">**ArrayOfTimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="995c7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="995c7-106">Attributes and elements</span></span>

<span data-ttu-id="995c7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="995c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="995c7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="995c7-108">Attributes</span></span>

<span data-ttu-id="995c7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="995c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="995c7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="995c7-110">Child elements</span></span>

|<span data-ttu-id="995c7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="995c7-111">**Element**</span></span>|<span data-ttu-id="995c7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="995c7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="995c7-113">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="995c7-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="995c7-114">Spécifie les périodes et les transitions qui définissent un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="995c7-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="995c7-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="995c7-115">Parent elements</span></span>

|<span data-ttu-id="995c7-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="995c7-116">**Element**</span></span>|<span data-ttu-id="995c7-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="995c7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="995c7-118">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="995c7-118">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="995c7-119">Contient l’État et le résultat d’une demande d' [opération GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="995c7-119">Contains the status and result of a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="995c7-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="995c7-120">Remarks</span></span>

<span data-ttu-id="995c7-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="995c7-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="995c7-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="995c7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="995c7-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="995c7-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="995c7-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="995c7-124">Schema Name</span></span>  <br/> |<span data-ttu-id="995c7-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="995c7-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="995c7-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="995c7-126">Validation File</span></span>  <br/> |<span data-ttu-id="995c7-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="995c7-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="995c7-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="995c7-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="995c7-129">False</span><span class="sxs-lookup"><span data-stu-id="995c7-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="995c7-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="995c7-130">See also</span></span>



- [<span data-ttu-id="995c7-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="995c7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

