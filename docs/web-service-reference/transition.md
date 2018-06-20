---
title: Transition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Transition
api_type:
- schema
ms.assetid: 23ce171a-a9c9-47ed-a366-822777048eea
description: L’élément de Transition représente une transition de fuseau horaire.
ms.openlocfilehash: 5dcd2f0dae7c3df2dcf660d6fe1a41b216c67b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838775"
---
# <a name="transition"></a><span data-ttu-id="c514c-103">Transition</span><span class="sxs-lookup"><span data-stu-id="c514c-103">Transition</span></span>

<span data-ttu-id="c514c-104">L’élément de **Transition** représente une transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="c514c-104">The **Transition** element represents a time zone transition.</span></span> 
  
```xml
<Transition>
   <To/>
</Transition>
```

 <span data-ttu-id="c514c-105">**TransitionType**</span><span class="sxs-lookup"><span data-stu-id="c514c-105">**TransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c514c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c514c-106">Attributes and elements</span></span>

<span data-ttu-id="c514c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c514c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c514c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c514c-108">Attributes</span></span>

<span data-ttu-id="c514c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c514c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c514c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c514c-110">Child elements</span></span>

|<span data-ttu-id="c514c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c514c-111">**Element**</span></span>|<span data-ttu-id="c514c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c514c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c514c-113">Pour</span><span class="sxs-lookup"><span data-stu-id="c514c-113">To</span></span>](to.md) <br/> |<span data-ttu-id="c514c-114">Spécifie la [période](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="c514c-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c514c-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c514c-115">Parent elements</span></span>

|<span data-ttu-id="c514c-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c514c-116">**Element**</span></span>|<span data-ttu-id="c514c-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c514c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c514c-118">Transitions</span><span class="sxs-lookup"><span data-stu-id="c514c-118">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="c514c-119">Représente une collection des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="c514c-119">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c514c-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="c514c-120">Remarks</span></span>

<span data-ttu-id="c514c-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="c514c-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c514c-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c514c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c514c-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c514c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c514c-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c514c-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c514c-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c514c-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c514c-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c514c-126">Validation File</span></span>  <br/> |<span data-ttu-id="c514c-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c514c-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c514c-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c514c-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c514c-129">False</span><span class="sxs-lookup"><span data-stu-id="c514c-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c514c-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c514c-130">See also</span></span>



- [<span data-ttu-id="c514c-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c514c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

