---
title: TimeZoneContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneContext
api_type:
- schema
ms.assetid: 573c462b-aa1d-4ba0-8852-e3f48b26873b
description: L’élément TimeZoneContext est utilisé dans l’en-tête SOAP Simple Object Access Protocol () pour spécifier la définition de fuseau horaire à utiliser par défaut lors de l’affectation le fuseau horaire pour les propriétés DateTime des objets qui sont créés, mis à jour et récupérés par à l’aide d’Exchange Web Services (EWS).
ms.openlocfilehash: 38b7ab4c587adac45fc3bcf351f417ea72313a97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838727"
---
# <a name="timezonecontext"></a><span data-ttu-id="7da73-103">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="7da73-103">TimeZoneContext</span></span>

<span data-ttu-id="7da73-104">L’élément **TimeZoneContext** est utilisé dans l’en-tête SOAP Simple Object Access Protocol () pour spécifier la définition de fuseau horaire à utiliser par défaut lors de l’affectation le fuseau horaire pour les propriétés DateTime d’objets qui sont créés, mis à jour, et récupéré à l’aide d’Exchange Web Services (EWS).</span><span class="sxs-lookup"><span data-stu-id="7da73-104">The **TimeZoneContext** element is used in the Simple Object Access Protocol (SOAP) header to specify the time zone definition that is to be used as the default when assigning the time zone for the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span> 
  
```xml
<TimeZoneContext>
   <TimeZoneDefinition/>
</TimeZoneContext>
```

 <span data-ttu-id="7da73-105">**TimeZoneContextType**</span><span class="sxs-lookup"><span data-stu-id="7da73-105">**TimeZoneContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7da73-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7da73-106">Attributes and elements</span></span>

<span data-ttu-id="7da73-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7da73-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7da73-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7da73-108">Attributes</span></span>

<span data-ttu-id="7da73-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7da73-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7da73-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7da73-110">Child elements</span></span>

|<span data-ttu-id="7da73-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7da73-111">**Element**</span></span>|<span data-ttu-id="7da73-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7da73-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7da73-113">Définition de fuseau horaire</span><span class="sxs-lookup"><span data-stu-id="7da73-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="7da73-114">Spécifie les périodes et les transitions qui définissent un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7da73-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7da73-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7da73-115">Parent elements</span></span>

<span data-ttu-id="7da73-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7da73-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7da73-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="7da73-117">Remarks</span></span>

<span data-ttu-id="7da73-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="7da73-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7da73-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7da73-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7da73-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7da73-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7da73-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7da73-121">Schema Name</span></span>  <br/> |<span data-ttu-id="7da73-122">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7da73-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="7da73-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7da73-123">Validation File</span></span>  <br/> |<span data-ttu-id="7da73-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7da73-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7da73-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7da73-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="7da73-126">False</span><span class="sxs-lookup"><span data-stu-id="7da73-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7da73-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7da73-127">See also</span></span>



- [<span data-ttu-id="7da73-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7da73-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

