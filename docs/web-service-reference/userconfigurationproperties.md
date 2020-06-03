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
ms.openlocfilehash: af6bee64516a7410d96ecc7581e8e819f550ddc1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466492"
---
# <a name="userconfigurationproperties"></a><span data-ttu-id="85268-103">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="85268-103">UserConfigurationProperties</span></span>

<span data-ttu-id="85268-104">L’élément **UserConfigurationProperties** spécifie les types de propriétés à obtenir dans une opération GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="85268-104">The **UserConfigurationProperties** element specifies the property types to get in a GetUserConfiguration operation.</span></span> 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 <span data-ttu-id="85268-105">**UserConfigurationPropertyType**</span><span class="sxs-lookup"><span data-stu-id="85268-105">**UserConfigurationPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85268-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="85268-106">Attributes and elements</span></span>

<span data-ttu-id="85268-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="85268-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85268-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="85268-108">Attributes</span></span>

<span data-ttu-id="85268-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="85268-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85268-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="85268-110">Child elements</span></span>

<span data-ttu-id="85268-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="85268-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="85268-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="85268-112">Parent elements</span></span>

|<span data-ttu-id="85268-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="85268-113">**Element**</span></span>|<span data-ttu-id="85268-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="85268-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85268-115">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="85268-115">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="85268-116">Spécifie une demande d’obtention d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="85268-116">Specifies a request to get a user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="85268-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="85268-117">Text value</span></span>

<span data-ttu-id="85268-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **UserConfigurationProperties** .</span><span class="sxs-lookup"><span data-stu-id="85268-118">The following table lists the possible values for the **UserConfigurationProperties** element.</span></span> 
  
|<span data-ttu-id="85268-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="85268-119">**Value**</span></span>|<span data-ttu-id="85268-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="85268-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="85268-121">ID</span><span class="sxs-lookup"><span data-stu-id="85268-121">Id</span></span>  <br/> |<span data-ttu-id="85268-122">Spécifie la propriété identifier.</span><span class="sxs-lookup"><span data-stu-id="85268-122">Specifies the identifier property.</span></span>  <br/> |
|<span data-ttu-id="85268-123">Dictionary</span><span class="sxs-lookup"><span data-stu-id="85268-123">Dictionary</span></span>  <br/> |<span data-ttu-id="85268-124">Spécifie les types de propriété de dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="85268-124">Specifies dictionary property types.</span></span>  <br/> |
|<span data-ttu-id="85268-125">XmlData</span><span class="sxs-lookup"><span data-stu-id="85268-125">XmlData</span></span>  <br/> |<span data-ttu-id="85268-126">Spécifie les types de propriétés de données XML.</span><span class="sxs-lookup"><span data-stu-id="85268-126">Specifies XML data property types.</span></span>  <br/> |
|<span data-ttu-id="85268-127">BinaryData</span><span class="sxs-lookup"><span data-stu-id="85268-127">BinaryData</span></span>  <br/> |<span data-ttu-id="85268-128">Spécifie les types de propriétés de données binaires.</span><span class="sxs-lookup"><span data-stu-id="85268-128">Specifies binary data property types.</span></span>  <br/> |
|<span data-ttu-id="85268-129">Tous</span><span class="sxs-lookup"><span data-stu-id="85268-129">All</span></span>  <br/> |<span data-ttu-id="85268-130">Spécifie l’identificateur, le dictionnaire, les données XML et les types de propriétés de données binaires.</span><span class="sxs-lookup"><span data-stu-id="85268-130">Specifies the identifier, dictionary, XML data, and binary data property types.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="85268-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="85268-131">Remarks</span></span>

<span data-ttu-id="85268-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="85268-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85268-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="85268-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85268-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="85268-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="85268-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="85268-135">Schema Name</span></span>  <br/> |<span data-ttu-id="85268-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="85268-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="85268-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="85268-137">Validation File</span></span>  <br/> |<span data-ttu-id="85268-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="85268-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="85268-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="85268-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="85268-140">False</span><span class="sxs-lookup"><span data-stu-id="85268-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85268-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="85268-141">See also</span></span>



- [<span data-ttu-id="85268-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="85268-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

