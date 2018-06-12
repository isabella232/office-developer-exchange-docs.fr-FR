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
description: L’élément DictionaryEntry Spécifie le contenu d’une propriété de l’entrée de dictionnaire unique.
ms.openlocfilehash: 75d7dd1aa82a4cc6c363b9c787cfb15b4d15b656
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755921"
---
# <a name="dictionaryentry"></a><span data-ttu-id="53dc5-103">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="53dc5-103">DictionaryEntry</span></span>

<span data-ttu-id="53dc5-104">L’élément **DictionaryEntry** Spécifie le contenu d’une propriété de l’entrée de dictionnaire unique.</span><span class="sxs-lookup"><span data-stu-id="53dc5-104">The **DictionaryEntry** element specifies the contents of a single dictionary entry property.</span></span> 
  
```xml
<DictionaryEntry>
   <DictionaryKey/>
   <DictionaryValue/>
</DictionaryEntry>
```

 <span data-ttu-id="53dc5-105">**UserConfigurationDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="53dc5-105">**UserConfigurationDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53dc5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="53dc5-106">Attributes and elements</span></span>

<span data-ttu-id="53dc5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="53dc5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53dc5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="53dc5-108">Attributes</span></span>

<span data-ttu-id="53dc5-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="53dc5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="53dc5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="53dc5-110">Child elements</span></span>

|<span data-ttu-id="53dc5-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="53dc5-111">**Element**</span></span>|<span data-ttu-id="53dc5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="53dc5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53dc5-113">DictionaryKey</span><span class="sxs-lookup"><span data-stu-id="53dc5-113">DictionaryKey</span></span>](dictionarykey.md) <br/> |<span data-ttu-id="53dc5-114">Spécifie la clé de dictionnaire pour une propriété de dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="53dc5-114">Specifies the dictionary key for a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="53dc5-115">DictionaryValue</span><span class="sxs-lookup"><span data-stu-id="53dc5-115">DictionaryValue</span></span>](dictionaryvalue.md) <br/> |<span data-ttu-id="53dc5-116">Spécifie la valeur de dictionnaire pour une propriété de dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="53dc5-116">Specifies the dictionary value for a dictionary property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="53dc5-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="53dc5-117">Parent elements</span></span>

|<span data-ttu-id="53dc5-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="53dc5-118">**Element**</span></span>|<span data-ttu-id="53dc5-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="53dc5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53dc5-120">Dictionnaire</span><span class="sxs-lookup"><span data-stu-id="53dc5-120">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="53dc5-121">Définit un ensemble d’entrées de dictionnaire de propriétés pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="53dc5-121">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="53dc5-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="53dc5-122">Text value</span></span>

<span data-ttu-id="53dc5-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="53dc5-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="53dc5-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="53dc5-124">Remarks</span></span>

<span data-ttu-id="53dc5-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="53dc5-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="53dc5-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="53dc5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53dc5-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="53dc5-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="53dc5-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="53dc5-128">Schema Name</span></span>  <br/> |<span data-ttu-id="53dc5-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="53dc5-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="53dc5-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="53dc5-130">Validation File</span></span>  <br/> |<span data-ttu-id="53dc5-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="53dc5-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="53dc5-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="53dc5-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="53dc5-133">False</span><span class="sxs-lookup"><span data-stu-id="53dc5-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="53dc5-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="53dc5-134">See also</span></span>

- [<span data-ttu-id="53dc5-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="53dc5-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

