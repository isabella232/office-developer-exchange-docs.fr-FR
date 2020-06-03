---
title: HasLocationChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5fd465b4-6070-4cd0-9ac3-ed9d2bfd5951
description: L’élément HasLocationChanged spécifie si la propriété Location d’une réunion a été modifiée.
ms.openlocfilehash: 4f774adcf4a7666f40524931504f1172e15ba24d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462443"
---
# <a name="haslocationchanged"></a><span data-ttu-id="15fd3-103">HasLocationChanged</span><span class="sxs-lookup"><span data-stu-id="15fd3-103">HasLocationChanged</span></span>

<span data-ttu-id="15fd3-104">L’élément **HasLocationChanged** spécifie si la propriété Location d’une réunion a été modifiée.</span><span class="sxs-lookup"><span data-stu-id="15fd3-104">The **HasLocationChanged** element specifies whether the location property of a meeting has changed.</span></span> 
  
```XML
<HasLocationChanged> true | false </HasLocationChanged>
```

 <span data-ttu-id="15fd3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="15fd3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15fd3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="15fd3-106">Attributes and elements</span></span>

<span data-ttu-id="15fd3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="15fd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15fd3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="15fd3-108">Attributes</span></span>

<span data-ttu-id="15fd3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="15fd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15fd3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="15fd3-110">Child elements</span></span>

<span data-ttu-id="15fd3-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="15fd3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15fd3-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="15fd3-112">Parent elements</span></span>

|<span data-ttu-id="15fd3-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="15fd3-113">**Element**</span></span>|<span data-ttu-id="15fd3-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="15fd3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15fd3-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="15fd3-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="15fd3-116">Spécifie les modifications apportées entre deux versions d’un message de demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="15fd3-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="15fd3-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="15fd3-117">Text value</span></span>

<span data-ttu-id="15fd3-118">Une valeur de texte de **true** pour l’élément **HasLocationChanged** indique que la propriété Location d’une réunion a changé.</span><span class="sxs-lookup"><span data-stu-id="15fd3-118">A text value of **true** for the **HasLocationChanged** element indicates that the location property of a meeting has changed.</span></span> <span data-ttu-id="15fd3-119">La valeur **false** indique que la propriété Location d’une réunion n’a pas été modifiée.</span><span class="sxs-lookup"><span data-stu-id="15fd3-119">A value **false** indicates that the location property of a meeting has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="15fd3-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="15fd3-120">Remarks</span></span>

<span data-ttu-id="15fd3-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="15fd3-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="15fd3-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="15fd3-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15fd3-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="15fd3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15fd3-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="15fd3-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15fd3-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="15fd3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="15fd3-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="15fd3-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="15fd3-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="15fd3-127">Validation File</span></span>  <br/> |<span data-ttu-id="15fd3-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="15fd3-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="15fd3-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="15fd3-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="15fd3-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="15fd3-130">See also</span></span>



- [<span data-ttu-id="15fd3-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15fd3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

