---
title: Mois (transition de fuseau horaire)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: 5e6aac75-366d-43d0-8ccb-956285474662
description: L’élément month représente le mois au cours duquel la transition de fuseau horaire a lieu.
ms.openlocfilehash: 1fa32ea355cc3fe826f9c34b2fd147a0d8201673
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467738"
---
# <a name="month-time-zone-transition"></a><span data-ttu-id="ca167-103">Mois (transition de fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="ca167-103">Month (Time Zone Transition)</span></span>

<span data-ttu-id="ca167-104">L’élément **Month** représente le mois au cours duquel la transition de fuseau horaire a lieu.</span><span class="sxs-lookup"><span data-stu-id="ca167-104">The **Month** element represents the month in which the time zone transition occurs.</span></span> 
  
```xml
<Month/>
```

 <span data-ttu-id="ca167-105">**int**</span><span class="sxs-lookup"><span data-stu-id="ca167-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca167-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ca167-106">Attributes and elements</span></span>

<span data-ttu-id="ca167-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ca167-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca167-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ca167-108">Attributes</span></span>

<span data-ttu-id="ca167-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ca167-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca167-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ca167-110">Child elements</span></span>

<span data-ttu-id="ca167-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ca167-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ca167-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ca167-112">Parent elements</span></span>

|<span data-ttu-id="ca167-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ca167-113">**Element**</span></span>|<span data-ttu-id="ca167-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ca167-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca167-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="ca167-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="ca167-116">Représente une transition de fuseau horaire qui se produit à une date spécifique chaque année.</span><span class="sxs-lookup"><span data-stu-id="ca167-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="ca167-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="ca167-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="ca167-118">Représente une transition de fuseau horaire qui se produit chaque année.</span><span class="sxs-lookup"><span data-stu-id="ca167-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ca167-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ca167-119">Text value</span></span>

<span data-ttu-id="ca167-120">La valeur de texte est un entier qui représente le mois au cours duquel la transition de fuseau horaire a lieu.</span><span class="sxs-lookup"><span data-stu-id="ca167-120">The text value is an integer that represents the month in which the time zone transition occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ca167-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="ca167-121">Remarks</span></span>

<span data-ttu-id="ca167-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ca167-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca167-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ca167-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca167-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ca167-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ca167-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ca167-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ca167-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ca167-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="ca167-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ca167-127">Validation File</span></span>  <br/> |<span data-ttu-id="ca167-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ca167-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ca167-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ca167-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca167-130">False</span><span class="sxs-lookup"><span data-stu-id="ca167-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca167-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ca167-131">See also</span></span>



- [<span data-ttu-id="ca167-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ca167-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

