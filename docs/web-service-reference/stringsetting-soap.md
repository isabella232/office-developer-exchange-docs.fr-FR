---
title: StringSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bf7096d8-42d4-4bf5-bbdd-851af2754000
description: L’élément StringSetting représente un paramètre de l’utilisateur dont la valeur est de type chaîne.
ms.openlocfilehash: af2c8ed243182e3491723be172ae162554250951
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829606"
---
# <a name="stringsetting-soap"></a><span data-ttu-id="386fb-103">StringSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="386fb-103">StringSetting (SOAP)</span></span>

<span data-ttu-id="386fb-104">L’élément **StringSetting** représente un paramètre de l’utilisateur dont la valeur est de type chaîne.</span><span class="sxs-lookup"><span data-stu-id="386fb-104">The **StringSetting** element represents a user setting the value of which is of type string.</span></span> 
  
```XML
<StringSetting>
   <Name/>
   <Value/>
</StringSetting>
```

 <span data-ttu-id="386fb-105">**StringSetting**</span><span class="sxs-lookup"><span data-stu-id="386fb-105">**StringSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="386fb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="386fb-106">Attributes and elements</span></span>

<span data-ttu-id="386fb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="386fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="386fb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="386fb-108">Attributes</span></span>

<span data-ttu-id="386fb-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="386fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="386fb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="386fb-110">Child elements</span></span>

|<span data-ttu-id="386fb-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="386fb-111">**Element**</span></span>|<span data-ttu-id="386fb-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="386fb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="386fb-113">Nom (SOAP)</span><span class="sxs-lookup"><span data-stu-id="386fb-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="386fb-114">Représente un nom de paramètre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="386fb-114">Represents a user setting name.</span></span>  <br/> |
|[<span data-ttu-id="386fb-115">Valeur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="386fb-115">Value (SOAP)</span></span>](value-soap.md) <br/> |<span data-ttu-id="386fb-116">Représente une valeur de paramètre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="386fb-116">Represents a user setting value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="386fb-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="386fb-117">Parent elements</span></span>

<span data-ttu-id="386fb-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="386fb-118">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="386fb-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="386fb-119">Text value</span></span>

<span data-ttu-id="386fb-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="386fb-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="386fb-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="386fb-121">Remarks</span></span>

<span data-ttu-id="386fb-122">Le type **StringSetting** étend le type **UserSetting** .</span><span class="sxs-lookup"><span data-stu-id="386fb-122">The **StringSetting** type extends the **UserSetting** type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="386fb-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="386fb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="386fb-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="386fb-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="386fb-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="386fb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="386fb-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="386fb-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="386fb-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="386fb-127">Validation File</span></span>  <br/> |<span data-ttu-id="386fb-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="386fb-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="386fb-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="386fb-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="386fb-130">True</span><span class="sxs-lookup"><span data-stu-id="386fb-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="386fb-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="386fb-131">See also</span></span>



[<span data-ttu-id="386fb-132">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="386fb-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="386fb-133">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="386fb-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="386fb-134">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="386fb-134">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

