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
description: L’élément TimeZoneContext est utilisé dans l’en-tête SOAP (Simple Object Access Protocol) pour spécifier la définition du fuseau horaire à utiliser par défaut lors de l’affectation du fuseau horaire pour les propriétés DateTime des objets créés, mis à jour et récupérés à l’aide des services Web Exchange (EWS).
ms.openlocfilehash: 26727317ccf34338e8d62ec92bd7a44d43a6cfdb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460252"
---
# <a name="timezonecontext"></a><span data-ttu-id="bd9a2-103">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="bd9a2-103">TimeZoneContext</span></span>

<span data-ttu-id="bd9a2-104">L’élément **TimeZoneContext** est utilisé dans l’en-tête SOAP (Simple Object Access Protocol) pour spécifier la définition du fuseau horaire à utiliser par défaut lors de l’affectation du fuseau horaire pour les propriétés DateTime des objets créés, mis à jour et récupérés à l’aide des services Web Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="bd9a2-104">The **TimeZoneContext** element is used in the Simple Object Access Protocol (SOAP) header to specify the time zone definition that is to be used as the default when assigning the time zone for the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span> 
  
```xml
<TimeZoneContext>
   <TimeZoneDefinition/>
</TimeZoneContext>
```

 <span data-ttu-id="bd9a2-105">**TimeZoneContextType**</span><span class="sxs-lookup"><span data-stu-id="bd9a2-105">**TimeZoneContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd9a2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bd9a2-106">Attributes and elements</span></span>

<span data-ttu-id="bd9a2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bd9a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd9a2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bd9a2-108">Attributes</span></span>

<span data-ttu-id="bd9a2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bd9a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd9a2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bd9a2-110">Child elements</span></span>

|<span data-ttu-id="bd9a2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bd9a2-111">**Element**</span></span>|<span data-ttu-id="bd9a2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="bd9a2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd9a2-113">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="bd9a2-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="bd9a2-114">Spécifie les périodes et les transitions qui définissent un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bd9a2-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd9a2-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bd9a2-115">Parent elements</span></span>

<span data-ttu-id="bd9a2-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bd9a2-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bd9a2-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="bd9a2-117">Remarks</span></span>

<span data-ttu-id="bd9a2-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="bd9a2-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd9a2-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bd9a2-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd9a2-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bd9a2-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd9a2-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bd9a2-121">Schema Name</span></span>  <br/> |<span data-ttu-id="bd9a2-122">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bd9a2-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd9a2-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bd9a2-123">Validation File</span></span>  <br/> |<span data-ttu-id="bd9a2-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bd9a2-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd9a2-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bd9a2-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd9a2-126">False</span><span class="sxs-lookup"><span data-stu-id="bd9a2-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd9a2-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bd9a2-127">See also</span></span>



- [<span data-ttu-id="bd9a2-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bd9a2-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

