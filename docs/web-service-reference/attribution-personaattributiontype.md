---
title: Attribution (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: L’élément Attribution spécifie une instance d’un tableau d’attributs pour un élément PersonaType.
ms.openlocfilehash: 0e800c92c75bf0c475d4bffd33d6ab49f9ad9a9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755349"
---
# <a name="attribution-personaattributiontype"></a><span data-ttu-id="2a4b4-103">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="2a4b4-103">Attribution (PersonaAttributionType)</span></span>

<span data-ttu-id="2a4b4-104">L’élément **Attribution** spécifie une instance d’un tableau d’attributs pour un élément **PersonaType** .</span><span class="sxs-lookup"><span data-stu-id="2a4b4-104">The **Attribution** element specifies an instance in an array of attributes for a **PersonaType** element.</span></span> 
  
```XML
<Attribution>
    <Id></Id>
    <SourceId></SourceId>
    <DisplayName></DisplayName>
    <IsWritable></IsWritable>
    <IsQuickContact></IsQuickContact>
    <IsHidden></IsHidden>
    <FolderId></FolderId>
</Attribution>
```

 <span data-ttu-id="2a4b4-105">**PersonaAttributionType**</span><span class="sxs-lookup"><span data-stu-id="2a4b4-105">**PersonaAttributionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a4b4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2a4b4-106">Attributes and elements</span></span>

<span data-ttu-id="2a4b4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a4b4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2a4b4-108">Attributes</span></span>

<span data-ttu-id="2a4b4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a4b4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2a4b4-110">Child elements</span></span>

|<span data-ttu-id="2a4b4-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2a4b4-111">**Element**</span></span>|<span data-ttu-id="2a4b4-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2a4b4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a4b4-113">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="2a4b4-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="2a4b4-114">Spécifie une chaîne qui identifie de manière unique une application ou une attribution dans un personnage.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-114">Specifies a string that uniquely identifies an app or an attribution in a persona.</span></span>  <br/> |
|[<span data-ttu-id="2a4b4-115">ID source</span><span class="sxs-lookup"><span data-stu-id="2a4b4-115">SourceId</span></span>](sourceid.md) <br/> |<span data-ttu-id="2a4b4-116">Spécifie l’identificateur du contact ou du destinataire d’Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-116">Specifies the identifier of the contact or Active Directory recipient.</span></span>  <br/> |
|[<span data-ttu-id="2a4b4-117">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="2a4b4-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="2a4b4-118">Définit le nom complet d’un dossier, contact, liste de distribution, délégué utilisateur ou de règle.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-118">Defines the display name of a folder, contact, distribution list, delegate user, or rule.</span></span>  <br/> |
|[<span data-ttu-id="2a4b4-119">IsWritable</span><span class="sxs-lookup"><span data-stu-id="2a4b4-119">IsWritable</span></span>](iswritable.md) <br/> |<span data-ttu-id="2a4b4-120">Spécifie si l’ou les destinataires d’Active Directory sous-jacent peut être écrite.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-120">Specifies whether the underlying contact or Active Directory recipient can be written to.</span></span>  <br/> |
|[<span data-ttu-id="2a4b4-121">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="2a4b4-121">IsQuickContact</span></span>](isquickcontact.md) <br/> |<span data-ttu-id="2a4b4-122">Spécifie une valeur de type Boolean qui indique si l’ou les destinataires d’Active Directory sous-jacent est un contact rapide.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-122">Specifies a Boolean value that indicates whether the underlying contact or Active Directory recipient is a quick contact.</span></span>  <br/> |
|[<span data-ttu-id="2a4b4-123">IsHidden</span><span class="sxs-lookup"><span data-stu-id="2a4b4-123">IsHidden</span></span>](ishidden.md) <br/> |<span data-ttu-id="2a4b4-124">Contient une valeur de type Boolean qui indique si l’ou les destinataires d’Active Directory sous-jacent doit être masqué ou affiché dans le cadre du personnage.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-124">Contains a Boolean value that indicates whether the underlying contact or Active Directory recipient should be hidden or displayed as part of the persona.</span></span>  <br/> |
|[<span data-ttu-id="2a4b4-125">FolderId</span><span class="sxs-lookup"><span data-stu-id="2a4b4-125">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="2a4b4-126">Contient la clé d’identificateur et de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-126">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2a4b4-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2a4b4-127">Parent elements</span></span>

|<span data-ttu-id="2a4b4-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2a4b4-128">**Element**</span></span>|<span data-ttu-id="2a4b4-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="2a4b4-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a4b4-130">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="2a4b4-130">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="2a4b4-131">Spécifie un tableau des informations d’attribution d’un ou plusieurs contacts ou des destinataires d’active directory (AD) regroupées dans les personnages associés.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-131">Specifies an array of attribution information for one or more of the contacts or active directory (AD) recipients aggregated into the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2a4b4-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="2a4b4-132">Remarks</span></span>

<span data-ttu-id="2a4b4-133">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2a4b4-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2a4b4-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a4b4-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2a4b4-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a4b4-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2a4b4-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2a4b4-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2a4b4-137">Schema Name</span></span>  <br/> |<span data-ttu-id="2a4b4-138">Schéma type</span><span class="sxs-lookup"><span data-stu-id="2a4b4-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="2a4b4-139">Validation File</span><span class="sxs-lookup"><span data-stu-id="2a4b4-139">Validation File</span></span>  <br/> |<span data-ttu-id="2a4b4-140">types.xsd</span><span class="sxs-lookup"><span data-stu-id="2a4b4-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2a4b4-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2a4b4-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2a4b4-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2a4b4-142">See also</span></span>

- [<span data-ttu-id="2a4b4-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2a4b4-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

