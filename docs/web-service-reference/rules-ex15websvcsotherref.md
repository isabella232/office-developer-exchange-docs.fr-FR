---
title: Règles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rules
api_type:
- schema
ms.assetid: 53f59054-8f68-4eaa-be9c-ccfc9383bcf2
description: L’élément Rules contient un tableau de règles de protection.
ms.openlocfilehash: d848abfe0c97d07836f28bc75806f506c5433d44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464937"
---
# <a name="rules"></a><span data-ttu-id="e871d-103">Règles</span><span class="sxs-lookup"><span data-stu-id="e871d-103">Rules</span></span>

<span data-ttu-id="e871d-104">L’élément **Rules** contient un tableau de règles de protection.</span><span class="sxs-lookup"><span data-stu-id="e871d-104">The **Rules** element contains an array of protection rules.</span></span> 
  
```xml
<Rules>   <Rule/></Rules>
```

 <span data-ttu-id="e871d-105">**ArrayOfProtectionRulesType**</span><span class="sxs-lookup"><span data-stu-id="e871d-105">**ArrayOfProtectionRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e871d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e871d-106">Attributes and elements</span></span>

<span data-ttu-id="e871d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e871d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e871d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e871d-108">Attributes</span></span>

<span data-ttu-id="e871d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e871d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e871d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e871d-110">Child elements</span></span>

|<span data-ttu-id="e871d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e871d-111">**Element**</span></span>|<span data-ttu-id="e871d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e871d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e871d-113">Règle</span><span class="sxs-lookup"><span data-stu-id="e871d-113">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="e871d-114">Contient une règle de protection unique.</span><span class="sxs-lookup"><span data-stu-id="e871d-114">Contains a single protection rule.</span></span> <span data-ttu-id="e871d-115">Cet élément peut se produire zéro ou plusieurs fois.</span><span class="sxs-lookup"><span data-stu-id="e871d-115">This element can occur zero or more times.</span></span> <span data-ttu-id="e871d-116">Cet élément se produit zéro fois lorsqu’aucune règle de protection n’est définie par l’organisation.</span><span class="sxs-lookup"><span data-stu-id="e871d-116">This element occurs zero times when no protection rules are defined by the organization.</span></span> <span data-ttu-id="e871d-117">Elle se produit une ou plusieurs fois si au moins une règle est définie par l’organisation.</span><span class="sxs-lookup"><span data-stu-id="e871d-117">It occurs one or more times if at least one rule is defined by the organization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e871d-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e871d-118">Parent elements</span></span>

|<span data-ttu-id="e871d-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e871d-119">**Element**</span></span>|<span data-ttu-id="e871d-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="e871d-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e871d-121">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="e871d-121">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="e871d-122">Contient la configuration du service des règles de protection.</span><span class="sxs-lookup"><span data-stu-id="e871d-122">Contains service configuration for the protection rules service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e871d-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="e871d-123">Remarks</span></span>

<span data-ttu-id="e871d-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e871d-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e871d-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e871d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e871d-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e871d-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e871d-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e871d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e871d-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e871d-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="e871d-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e871d-129">Validation File</span></span>  <br/> |<span data-ttu-id="e871d-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e871d-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e871d-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e871d-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e871d-132">False</span><span class="sxs-lookup"><span data-stu-id="e871d-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e871d-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e871d-133">See also</span></span>



- [<span data-ttu-id="e871d-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e871d-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

