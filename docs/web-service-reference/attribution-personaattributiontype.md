---
title: Attribution (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: L’élément spécifie une instance dans un tableau d’attributs pour un élément PersonaType.
ms.openlocfilehash: 05b0d41c116f2ed7b8dbb3ac44108bb879256b5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464174"
---
# <a name="attribution-personaattributiontype"></a><span data-ttu-id="04a11-103">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="04a11-103">Attribution (PersonaAttributionType)</span></span>

<span data-ttu-id="04a11-104">L' **élément** spécifie une instance dans un tableau d’attributs pour un élément **PersonaType** .</span><span class="sxs-lookup"><span data-stu-id="04a11-104">The **Attribution** element specifies an instance in an array of attributes for a **PersonaType** element.</span></span> 
  
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

 <span data-ttu-id="04a11-105">**PersonaAttributionType**</span><span class="sxs-lookup"><span data-stu-id="04a11-105">**PersonaAttributionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04a11-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="04a11-106">Attributes and elements</span></span>

<span data-ttu-id="04a11-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="04a11-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04a11-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="04a11-108">Attributes</span></span>

<span data-ttu-id="04a11-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="04a11-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04a11-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="04a11-110">Child elements</span></span>

|<span data-ttu-id="04a11-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04a11-111">**Element**</span></span>|<span data-ttu-id="04a11-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="04a11-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04a11-113">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="04a11-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="04a11-114">Spécifie une chaîne qui identifie de manière unique une application ou une attribution dans un personnage.</span><span class="sxs-lookup"><span data-stu-id="04a11-114">Specifies a string that uniquely identifies an app or an attribution in a persona.</span></span>  <br/> |
|[<span data-ttu-id="04a11-115">SourceId</span><span class="sxs-lookup"><span data-stu-id="04a11-115">SourceId</span></span>](sourceid.md) <br/> |<span data-ttu-id="04a11-116">Spécifie l’identificateur du destinataire du contact ou Active Directory.</span><span class="sxs-lookup"><span data-stu-id="04a11-116">Specifies the identifier of the contact or Active Directory recipient.</span></span>  <br/> |
|[<span data-ttu-id="04a11-117">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="04a11-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="04a11-118">Définit le nom d’affichage d’un dossier, d’un contact, d’une liste de distribution, d’un utilisateur délégué ou d’une règle.</span><span class="sxs-lookup"><span data-stu-id="04a11-118">Defines the display name of a folder, contact, distribution list, delegate user, or rule.</span></span>  <br/> |
|[<span data-ttu-id="04a11-119">IsWritable</span><span class="sxs-lookup"><span data-stu-id="04a11-119">IsWritable</span></span>](iswritable.md) <br/> |<span data-ttu-id="04a11-120">Indique si le contact sous-jacent ou le destinataire Active Directory peut être accessible en écriture.</span><span class="sxs-lookup"><span data-stu-id="04a11-120">Specifies whether the underlying contact or Active Directory recipient can be written to.</span></span>  <br/> |
|[<span data-ttu-id="04a11-121">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="04a11-121">IsQuickContact</span></span>](isquickcontact.md) <br/> |<span data-ttu-id="04a11-122">Spécifie une valeur de type Boolean qui indique si le contact sous-jacent ou le destinataire Active Directory est un contact rapide.</span><span class="sxs-lookup"><span data-stu-id="04a11-122">Specifies a Boolean value that indicates whether the underlying contact or Active Directory recipient is a quick contact.</span></span>  <br/> |
|[<span data-ttu-id="04a11-123">IsHidden</span><span class="sxs-lookup"><span data-stu-id="04a11-123">IsHidden</span></span>](ishidden.md) <br/> |<span data-ttu-id="04a11-124">Contient une valeur de type Boolean qui indique si le destinataire sous-jacent ou Active Directory doit être masqué ou affiché en tant que partie du personnage.</span><span class="sxs-lookup"><span data-stu-id="04a11-124">Contains a Boolean value that indicates whether the underlying contact or Active Directory recipient should be hidden or displayed as part of the persona.</span></span>  <br/> |
|[<span data-ttu-id="04a11-125">FolderId</span><span class="sxs-lookup"><span data-stu-id="04a11-125">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="04a11-126">Contient l’identificateur et la clé de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="04a11-126">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04a11-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="04a11-127">Parent elements</span></span>

|<span data-ttu-id="04a11-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04a11-128">**Element**</span></span>|<span data-ttu-id="04a11-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="04a11-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04a11-130">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="04a11-130">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="04a11-131">Spécifie un tableau d’informations d’attribution pour un ou plusieurs contacts ou destinataires Active Directory (AD) rassemblés dans le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="04a11-131">Specifies an array of attribution information for one or more of the contacts or active directory (AD) recipients aggregated into the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="04a11-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="04a11-132">Remarks</span></span>

<span data-ttu-id="04a11-133">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="04a11-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="04a11-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="04a11-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04a11-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="04a11-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04a11-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="04a11-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04a11-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="04a11-137">Schema Name</span></span>  <br/> |<span data-ttu-id="04a11-138">Schéma type</span><span class="sxs-lookup"><span data-stu-id="04a11-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="04a11-139">Validation File</span><span class="sxs-lookup"><span data-stu-id="04a11-139">Validation File</span></span>  <br/> |<span data-ttu-id="04a11-140">types. xsd</span><span class="sxs-lookup"><span data-stu-id="04a11-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="04a11-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="04a11-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="04a11-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="04a11-142">See also</span></span>

- [<span data-ttu-id="04a11-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="04a11-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

