---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: L’élément PolicyTag Spécifie l’identificateur de rétention sur un élément ou un dossier.
ms.openlocfilehash: d6cd5aab1145f6006912541c8f8c1d0a91d1e17e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828835"
---
# <a name="policytag"></a><span data-ttu-id="89f44-103">PolicyTag</span><span class="sxs-lookup"><span data-stu-id="89f44-103">PolicyTag</span></span>

<span data-ttu-id="89f44-104">L’élément **PolicyTag** Spécifie l’identificateur de rétention sur un élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="89f44-104">The **PolicyTag** element specifies the retention identifier on an item or folder.</span></span> 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 <span data-ttu-id="89f44-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="89f44-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89f44-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="89f44-106">Attributes and elements</span></span>

<span data-ttu-id="89f44-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="89f44-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89f44-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="89f44-108">Attributes</span></span>

|<span data-ttu-id="89f44-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="89f44-109">**Attribute**</span></span>|<span data-ttu-id="89f44-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="89f44-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="89f44-111">IsExplicit</span><span class="sxs-lookup"><span data-stu-id="89f44-111">IsExplicit</span></span>  <br/> |<span data-ttu-id="89f44-112">Indique si une balise de stratégie a été explicitement définie sur un élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="89f44-112">Indicates whether a policy tag was explicitly set on an item or folder.</span></span>  <br/> <span data-ttu-id="89f44-113">Une valeur de texte de **la valeur true** pour l’attribut **IsExplicit** indique que la balise de stratégie a été explicitement définie sur l’élément ou d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="89f44-113">A text value of **true** for the **IsExplicit** attribute indicates that the policy tag was explicitly set on the item or folder.</span></span> <span data-ttu-id="89f44-114">Texte la valeur **false** indique que la balise de stratégie a été implicitement définie sur l’élément ou un dossier en fonction de la balise de stratégie de dossier parent.</span><span class="sxs-lookup"><span data-stu-id="89f44-114">A text value of **false** indicates that the policy tag was implicitly set on the item or folder based on the parent folder policy tag.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="89f44-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="89f44-115">Child elements</span></span>

<span data-ttu-id="89f44-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="89f44-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="89f44-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="89f44-117">Parent elements</span></span>

<span data-ttu-id="89f44-118">[SearchPreviewItem](searchpreviewitem.md) | [élément](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [tâche](task.md)</span><span class="sxs-lookup"><span data-stu-id="89f44-118">[SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="89f44-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="89f44-119">Text value</span></span>

<span data-ttu-id="89f44-120">La valeur de texte de l’élément **PolicyTag** est l’identificateur de balise de stratégie.</span><span class="sxs-lookup"><span data-stu-id="89f44-120">The text value of the **PolicyTag** element is the policy tag identifier.</span></span> <span data-ttu-id="89f44-121">L’identificateur de balise de stratégie est un GUID.</span><span class="sxs-lookup"><span data-stu-id="89f44-121">The policy tag identifier is a GUID.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="89f44-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="89f44-122">Remarks</span></span>

<span data-ttu-id="89f44-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="89f44-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="89f44-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="89f44-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89f44-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="89f44-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89f44-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="89f44-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89f44-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="89f44-127">Schema name</span></span>  <br/> |<span data-ttu-id="89f44-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="89f44-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="89f44-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="89f44-129">Validation file</span></span>  <br/> |<span data-ttu-id="89f44-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="89f44-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="89f44-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="89f44-131">Can be empty</span></span>  <br/> ||
   

