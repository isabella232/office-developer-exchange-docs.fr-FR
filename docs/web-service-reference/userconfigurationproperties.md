---
title: UserConfigurationProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationProperties
api_type:
- schema
ms.assetid: c143a6ec-62ad-4d48-b844-b1ad88054bc1
description: L’élément UserConfigurationProperties spécifie les types de propriétés à obtenir dans une opération GetUserConfiguration.
ms.openlocfilehash: 4f993765bb7c36f28a41a3f2fa7e28698a3f709e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838952"
---
# <a name="userconfigurationproperties"></a><span data-ttu-id="9cafb-103">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="9cafb-103">UserConfigurationProperties</span></span>

<span data-ttu-id="9cafb-104">L’élément **UserConfigurationProperties** spécifie les types de propriétés à obtenir dans une opération GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9cafb-104">The **UserConfigurationProperties** element specifies the property types to get in a GetUserConfiguration operation.</span></span> 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 <span data-ttu-id="9cafb-105">**UserConfigurationPropertyType**</span><span class="sxs-lookup"><span data-stu-id="9cafb-105">**UserConfigurationPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9cafb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9cafb-106">Attributes and elements</span></span>

<span data-ttu-id="9cafb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9cafb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9cafb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9cafb-108">Attributes</span></span>

<span data-ttu-id="9cafb-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9cafb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9cafb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9cafb-110">Child elements</span></span>

<span data-ttu-id="9cafb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9cafb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9cafb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9cafb-112">Parent elements</span></span>

|<span data-ttu-id="9cafb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9cafb-113">**Element**</span></span>|<span data-ttu-id="9cafb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9cafb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9cafb-115">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="9cafb-115">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="9cafb-116">Spécifie une requête pour obtenir un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9cafb-116">Specifies a request to get a user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9cafb-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9cafb-117">Text value</span></span>

<span data-ttu-id="9cafb-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **UserConfigurationProperties** .</span><span class="sxs-lookup"><span data-stu-id="9cafb-118">The following table lists the possible values for the **UserConfigurationProperties** element.</span></span> 
  
|<span data-ttu-id="9cafb-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="9cafb-119">**Value**</span></span>|<span data-ttu-id="9cafb-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="9cafb-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9cafb-121">ID</span><span class="sxs-lookup"><span data-stu-id="9cafb-121">Id</span></span>  <br/> |<span data-ttu-id="9cafb-122">Spécifie la propriété identificateur.</span><span class="sxs-lookup"><span data-stu-id="9cafb-122">Specifies the identifier property.</span></span>  <br/> |
|<span data-ttu-id="9cafb-123">Dictionary</span><span class="sxs-lookup"><span data-stu-id="9cafb-123">Dictionary</span></span>  <br/> |<span data-ttu-id="9cafb-124">Spécifie les types de propriétés de dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="9cafb-124">Specifies dictionary property types.</span></span>  <br/> |
|<span data-ttu-id="9cafb-125">XmlData</span><span class="sxs-lookup"><span data-stu-id="9cafb-125">XmlData</span></span>  <br/> |<span data-ttu-id="9cafb-126">Spécifie les types de propriété de données XML.</span><span class="sxs-lookup"><span data-stu-id="9cafb-126">Specifies XML data property types.</span></span>  <br/> |
|<span data-ttu-id="9cafb-127">BinaryData</span><span class="sxs-lookup"><span data-stu-id="9cafb-127">BinaryData</span></span>  <br/> |<span data-ttu-id="9cafb-128">Spécifie les types de propriétés des données binaires.</span><span class="sxs-lookup"><span data-stu-id="9cafb-128">Specifies binary data property types.</span></span>  <br/> |
|<span data-ttu-id="9cafb-129">Tous</span><span class="sxs-lookup"><span data-stu-id="9cafb-129">All</span></span>  <br/> |<span data-ttu-id="9cafb-130">Spécifie l’identificateur, dictionnaire, données XML et les types de propriétés des données binaires.</span><span class="sxs-lookup"><span data-stu-id="9cafb-130">Specifies the identifier, dictionary, XML data, and binary data property types.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9cafb-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="9cafb-131">Remarks</span></span>

<span data-ttu-id="9cafb-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9cafb-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9cafb-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9cafb-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9cafb-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9cafb-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9cafb-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9cafb-135">Schema Name</span></span>  <br/> |<span data-ttu-id="9cafb-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9cafb-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9cafb-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9cafb-137">Validation File</span></span>  <br/> |<span data-ttu-id="9cafb-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9cafb-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9cafb-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9cafb-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="9cafb-140">False</span><span class="sxs-lookup"><span data-stu-id="9cafb-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9cafb-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9cafb-141">See also</span></span>



- [<span data-ttu-id="9cafb-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9cafb-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
