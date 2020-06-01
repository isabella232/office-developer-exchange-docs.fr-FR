---
title: FileAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAs
api_type:
- schema
ms.assetid: df50524e-471c-49d2-89fe-b2d0f61a1365
description: L’élément FileAs représente la manière dont un contact ou une liste de distribution est classé dans le dossier contacts.
ms.openlocfilehash: be756d86d7608fcb758dd54f2ada9f03a04343e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461197"
---
# <a name="fileas"></a><span data-ttu-id="b5af1-103">FileAs</span><span class="sxs-lookup"><span data-stu-id="b5af1-103">FileAs</span></span>

<span data-ttu-id="b5af1-104">L’élément **FileAs** représente la manière dont un contact ou une liste de distribution est classé dans le dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="b5af1-104">The **FileAs** element represents how a contact or distribution list is filed in the Contacts folder.</span></span> 
  
```xml
<FileAs/>
```

 <span data-ttu-id="b5af1-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="b5af1-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5af1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b5af1-106">Attributes and elements</span></span>

<span data-ttu-id="b5af1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b5af1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5af1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b5af1-108">Attributes</span></span>

<span data-ttu-id="b5af1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b5af1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5af1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b5af1-110">Child elements</span></span>

<span data-ttu-id="b5af1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b5af1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5af1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b5af1-112">Parent elements</span></span>

|<span data-ttu-id="b5af1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b5af1-113">**Element**</span></span>|<span data-ttu-id="b5af1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b5af1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5af1-115">DistributionList</span><span class="sxs-lookup"><span data-stu-id="b5af1-115">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="b5af1-116">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="b5af1-116">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="b5af1-117">Contact</span><span class="sxs-lookup"><span data-stu-id="b5af1-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b5af1-118">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5af1-118">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b5af1-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="b5af1-119">Text value</span></span>

<span data-ttu-id="b5af1-120">Une valeur de texte qui représente une chaîne est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="b5af1-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b5af1-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="b5af1-121">Remarks</span></span>

<span data-ttu-id="b5af1-122">L’élément **FileAs** sert à trier les contacts et les listes de distribution par un nom autre qu’un nom complet ou un nom de société.</span><span class="sxs-lookup"><span data-stu-id="b5af1-122">The **FileAs** element is used to sort contacts and distribution lists by a name other than a full name or company name.</span></span> 
  
<span data-ttu-id="b5af1-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b5af1-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5af1-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b5af1-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5af1-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b5af1-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5af1-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b5af1-126">Schema name</span></span>  <br/> |<span data-ttu-id="b5af1-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b5af1-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="b5af1-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b5af1-128">Validation file</span></span>  <br/> |<span data-ttu-id="b5af1-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b5af1-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5af1-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b5af1-130">Can be empty</span></span>  <br/> |<span data-ttu-id="b5af1-131">False</span><span class="sxs-lookup"><span data-stu-id="b5af1-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b5af1-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b5af1-132">See also</span></span>



- [<span data-ttu-id="b5af1-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b5af1-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

