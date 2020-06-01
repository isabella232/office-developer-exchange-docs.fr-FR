---
title: NumberOfOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfOccurrences
api_type:
- schema
ms.assetid: 9ec86ceb-b271-4718-97ca-b6a532ea7223
description: L’élément NumberOfOccurrences contient le nombre d’occurrences d’un élément périodique.
ms.openlocfilehash: f9b72611e87c5f2b98deb14c25988e574a324491
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462541"
---
# <a name="numberofoccurrences"></a><span data-ttu-id="310ab-103">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="310ab-103">NumberOfOccurrences</span></span>

<span data-ttu-id="310ab-104">L’élément **NumberOfOccurrences** contient le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="310ab-104">The **NumberOfOccurrences** element contains the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberOfOccurrences/>
```

 <span data-ttu-id="310ab-105">**int**</span><span class="sxs-lookup"><span data-stu-id="310ab-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="310ab-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="310ab-106">Attributes and elements</span></span>

<span data-ttu-id="310ab-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="310ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="310ab-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="310ab-108">Attributes</span></span>

<span data-ttu-id="310ab-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="310ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="310ab-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="310ab-110">Child elements</span></span>

<span data-ttu-id="310ab-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="310ab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="310ab-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="310ab-112">Parent elements</span></span>

|<span data-ttu-id="310ab-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="310ab-113">**Element**</span></span>|<span data-ttu-id="310ab-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="310ab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="310ab-115">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="310ab-115">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="310ab-116">Décrit la date de début et le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="310ab-116">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="310ab-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="310ab-117">Text value</span></span>

<span data-ttu-id="310ab-118">La valeur de texte est un entier qui représente le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="310ab-118">The text value is an integer that represents the number of occurrences of a recurring item.</span></span> <span data-ttu-id="310ab-119">La valeur doit être un entier compris entre 1 et 999.</span><span class="sxs-lookup"><span data-stu-id="310ab-119">The value must be an integer in the range of 1 to 999.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="310ab-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="310ab-120">Remarks</span></span>

<span data-ttu-id="310ab-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="310ab-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="310ab-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="310ab-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="310ab-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="310ab-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="310ab-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="310ab-124">Schema name</span></span>  <br/> |<span data-ttu-id="310ab-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="310ab-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="310ab-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="310ab-126">Validation file</span></span>  <br/> |<span data-ttu-id="310ab-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="310ab-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="310ab-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="310ab-128">Can be empty</span></span>  <br/> |<span data-ttu-id="310ab-129">False</span><span class="sxs-lookup"><span data-stu-id="310ab-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="310ab-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="310ab-130">See also</span></span>



- [<span data-ttu-id="310ab-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="310ab-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

