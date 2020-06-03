---
title: DictionaryEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryEntry
api_type:
- schema
ms.assetid: 531ea96a-d411-43e6-9fec-11fa2c959a30
description: L’élément DictionaryEntry spécifie le contenu d’une propriété d’entrée de dictionnaire unique.
ms.openlocfilehash: 4c5d4c037f0c97b26d518d2f1386f71b31fa2d1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455659"
---
# <a name="dictionaryentry"></a><span data-ttu-id="09ff8-103">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="09ff8-103">DictionaryEntry</span></span>

<span data-ttu-id="09ff8-104">L’élément **DictionaryEntry** spécifie le contenu d’une propriété d’entrée de dictionnaire unique.</span><span class="sxs-lookup"><span data-stu-id="09ff8-104">The **DictionaryEntry** element specifies the contents of a single dictionary entry property.</span></span> 
  
```xml
<DictionaryEntry>
   <DictionaryKey/>
   <DictionaryValue/>
</DictionaryEntry>
```

 <span data-ttu-id="09ff8-105">**UserConfigurationDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="09ff8-105">**UserConfigurationDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09ff8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="09ff8-106">Attributes and elements</span></span>

<span data-ttu-id="09ff8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="09ff8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09ff8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="09ff8-108">Attributes</span></span>

<span data-ttu-id="09ff8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="09ff8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09ff8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="09ff8-110">Child elements</span></span>

|<span data-ttu-id="09ff8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="09ff8-111">**Element**</span></span>|<span data-ttu-id="09ff8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="09ff8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09ff8-113">DictionaryKey</span><span class="sxs-lookup"><span data-stu-id="09ff8-113">DictionaryKey</span></span>](dictionarykey.md) <br/> |<span data-ttu-id="09ff8-114">Spécifie la clé de dictionnaire pour une propriété de dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="09ff8-114">Specifies the dictionary key for a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="09ff8-115">DictionaryValue</span><span class="sxs-lookup"><span data-stu-id="09ff8-115">DictionaryValue</span></span>](dictionaryvalue.md) <br/> |<span data-ttu-id="09ff8-116">Spécifie la valeur de dictionnaire pour une propriété de dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="09ff8-116">Specifies the dictionary value for a dictionary property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="09ff8-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="09ff8-117">Parent elements</span></span>

|<span data-ttu-id="09ff8-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="09ff8-118">**Element**</span></span>|<span data-ttu-id="09ff8-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="09ff8-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09ff8-120">Dictionnaire</span><span class="sxs-lookup"><span data-stu-id="09ff8-120">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="09ff8-121">Définit un ensemble d’entrées de propriété de dictionnaire pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="09ff8-121">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09ff8-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="09ff8-122">Text value</span></span>

<span data-ttu-id="09ff8-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="09ff8-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09ff8-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="09ff8-124">Remarks</span></span>

<span data-ttu-id="09ff8-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="09ff8-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09ff8-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="09ff8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09ff8-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="09ff8-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="09ff8-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="09ff8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="09ff8-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="09ff8-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="09ff8-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="09ff8-130">Validation File</span></span>  <br/> |<span data-ttu-id="09ff8-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="09ff8-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="09ff8-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="09ff8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="09ff8-133">False</span><span class="sxs-lookup"><span data-stu-id="09ff8-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09ff8-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="09ff8-134">See also</span></span>

- [<span data-ttu-id="09ff8-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="09ff8-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

