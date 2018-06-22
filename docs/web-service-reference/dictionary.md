---
title: Dictionary
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Dictionary
api_type:
- schema
ms.assetid: 8309e468-115b-4d6e-b33c-c4719dcecc4c
description: L’élément Dictionary définit un ensemble d’entrées de dictionnaire de propriétés pour un objet de configuration utilisateur.
ms.openlocfilehash: 151abfe7a9a9ae05b8b61af87c33675e025920ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755919"
---
# <a name="dictionary"></a><span data-ttu-id="f7e88-103">Dictionary</span><span class="sxs-lookup"><span data-stu-id="f7e88-103">Dictionary</span></span>

<span data-ttu-id="f7e88-104">L’élément **Dictionary** définit un ensemble d’entrées de dictionnaire de propriétés pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f7e88-104">The **Dictionary** element defines a set of dictionary property entries for a user configuration object.</span></span> 
  
```xml
<Dictionary>
   <DictionaryEntry/>
</Dictionary>
```

 <span data-ttu-id="f7e88-105">**UserConfigurationDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="f7e88-105">**UserConfigurationDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7e88-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f7e88-106">Attributes and elements</span></span>

<span data-ttu-id="f7e88-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f7e88-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7e88-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f7e88-108">Attributes</span></span>

<span data-ttu-id="f7e88-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f7e88-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7e88-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f7e88-110">Child elements</span></span>

|<span data-ttu-id="f7e88-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7e88-111">**Element**</span></span>|<span data-ttu-id="f7e88-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7e88-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7e88-113">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="f7e88-113">DictionaryEntry</span></span>](dictionaryentry.md) <br/> |<span data-ttu-id="f7e88-114">Spécifie le contenu d’une propriété de l’entrée de dictionnaire unique.</span><span class="sxs-lookup"><span data-stu-id="f7e88-114">Specifies the contents of a single dictionary entry property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7e88-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f7e88-115">Parent elements</span></span>

|<span data-ttu-id="f7e88-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7e88-116">**Element**</span></span>|<span data-ttu-id="f7e88-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7e88-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7e88-118">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7e88-118">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="f7e88-119">Définit un objet de configuration utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="f7e88-119">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f7e88-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f7e88-120">Text value</span></span>

<span data-ttu-id="f7e88-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f7e88-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f7e88-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="f7e88-122">Remarks</span></span>

<span data-ttu-id="f7e88-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7e88-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7e88-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f7e88-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7e88-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f7e88-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7e88-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f7e88-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f7e88-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f7e88-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7e88-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f7e88-128">Validation File</span></span>  <br/> |<span data-ttu-id="f7e88-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f7e88-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7e88-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f7e88-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7e88-131">False</span><span class="sxs-lookup"><span data-stu-id="f7e88-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7e88-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f7e88-132">See also</span></span>

- [<span data-ttu-id="f7e88-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f7e88-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

