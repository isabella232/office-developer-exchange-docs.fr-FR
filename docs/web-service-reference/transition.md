---
title: Bascul
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
description: L’élément transition représente une transition de fuseau horaire.
ms.openlocfilehash: 05495eb4a493feedc88532cc4bc8b949493481f5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467493"
---
# <a name="transition"></a><span data-ttu-id="7ebff-103">Bascul</span><span class="sxs-lookup"><span data-stu-id="7ebff-103">Transition</span></span>

<span data-ttu-id="7ebff-104">L’élément **transition** représente une transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7ebff-104">The **Transition** element represents a time zone transition.</span></span> 
  
```xml
<Transition>
   <To/>
</Transition>
```

 <span data-ttu-id="7ebff-105">**TransitionType**</span><span class="sxs-lookup"><span data-stu-id="7ebff-105">**TransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ebff-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7ebff-106">Attributes and elements</span></span>

<span data-ttu-id="7ebff-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7ebff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ebff-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7ebff-108">Attributes</span></span>

<span data-ttu-id="7ebff-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7ebff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ebff-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7ebff-110">Child elements</span></span>

|<span data-ttu-id="7ebff-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7ebff-111">**Element**</span></span>|<span data-ttu-id="7ebff-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7ebff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ebff-113">To</span><span class="sxs-lookup"><span data-stu-id="7ebff-113">To</span></span>](to.md) <br/> |<span data-ttu-id="7ebff-114">Spécifie le [point](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7ebff-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7ebff-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7ebff-115">Parent elements</span></span>

|<span data-ttu-id="7ebff-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7ebff-116">**Element**</span></span>|<span data-ttu-id="7ebff-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7ebff-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ebff-118">Transitions</span><span class="sxs-lookup"><span data-stu-id="7ebff-118">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="7ebff-119">Représente une collection de transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7ebff-119">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ebff-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="7ebff-120">Remarks</span></span>

<span data-ttu-id="7ebff-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7ebff-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ebff-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7ebff-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ebff-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7ebff-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ebff-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7ebff-124">Schema Name</span></span>  <br/> |<span data-ttu-id="7ebff-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7ebff-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ebff-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7ebff-126">Validation File</span></span>  <br/> |<span data-ttu-id="7ebff-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7ebff-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ebff-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7ebff-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="7ebff-129">False</span><span class="sxs-lookup"><span data-stu-id="7ebff-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ebff-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7ebff-130">See also</span></span>



- [<span data-ttu-id="7ebff-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7ebff-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

