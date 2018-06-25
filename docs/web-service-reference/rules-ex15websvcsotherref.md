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
ms.openlocfilehash: 5d511f977f3eb3273dc43f56356a059985b2a929
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829269"
---
# <a name="rules"></a><span data-ttu-id="4007b-103">Règles</span><span class="sxs-lookup"><span data-stu-id="4007b-103">Rules</span></span>

<span data-ttu-id="4007b-104">L’élément **Rules** contient un tableau de règles de protection.</span><span class="sxs-lookup"><span data-stu-id="4007b-104">The **Rules** element contains an array of protection rules.</span></span> 
  
```xml
<Rules>   <Rule/></Rules>
```

 <span data-ttu-id="4007b-105">**ArrayOfProtectionRulesType**</span><span class="sxs-lookup"><span data-stu-id="4007b-105">**ArrayOfProtectionRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4007b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4007b-106">Attributes and elements</span></span>

<span data-ttu-id="4007b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4007b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4007b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4007b-108">Attributes</span></span>

<span data-ttu-id="4007b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4007b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4007b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4007b-110">Child elements</span></span>

|<span data-ttu-id="4007b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4007b-111">**Element**</span></span>|<span data-ttu-id="4007b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4007b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4007b-113">Règle</span><span class="sxs-lookup"><span data-stu-id="4007b-113">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="4007b-114">Contient une règle de protection unique.</span><span class="sxs-lookup"><span data-stu-id="4007b-114">Contains a single protection rule.</span></span> <span data-ttu-id="4007b-115">Cet élément peut se produire plusieurs fois.</span><span class="sxs-lookup"><span data-stu-id="4007b-115">This element can occur zero or more times.</span></span> <span data-ttu-id="4007b-116">Cet élément produit zéro lorsque aucune règle de protection n’est définies par l’organisation.</span><span class="sxs-lookup"><span data-stu-id="4007b-116">This element occurs zero times when no protection rules are defined by the organization.</span></span> <span data-ttu-id="4007b-117">Il se produit une ou plusieurs fois si au moins une règle est définie par l’organisation.</span><span class="sxs-lookup"><span data-stu-id="4007b-117">It occurs one or more times if at least one rule is defined by the organization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4007b-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4007b-118">Parent elements</span></span>

|<span data-ttu-id="4007b-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4007b-119">**Element**</span></span>|<span data-ttu-id="4007b-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="4007b-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4007b-121">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="4007b-121">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="4007b-122">Contient la configuration de service pour le service de règles de protection.</span><span class="sxs-lookup"><span data-stu-id="4007b-122">Contains service configuration for the protection rules service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4007b-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="4007b-123">Remarks</span></span>

<span data-ttu-id="4007b-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="4007b-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4007b-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4007b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4007b-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4007b-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4007b-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4007b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4007b-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4007b-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="4007b-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4007b-129">Validation File</span></span>  <br/> |<span data-ttu-id="4007b-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4007b-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4007b-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4007b-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="4007b-132">False</span><span class="sxs-lookup"><span data-stu-id="4007b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4007b-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4007b-133">See also</span></span>



- [<span data-ttu-id="4007b-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4007b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

