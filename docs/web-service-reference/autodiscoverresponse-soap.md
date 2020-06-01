---
title: AutodiscoverResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 203a5ac3-ebd0-4514-acbe-bc1c74638127
description: L’élément AutodiscoverResponse (SOAP) représente l’élément de base pour toutes les réponses renvoyées par le service de découverte automatique.
ms.openlocfilehash: 81fd557578bde9552d07e24386c93903e44a9afa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463964"
---
# <a name="autodiscoverresponse-soap"></a><span data-ttu-id="05398-103">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05398-103">AutodiscoverResponse (SOAP)</span></span>

<span data-ttu-id="05398-104">L’élément **AutodiscoverResponse (SOAP)** représente l’élément de base pour toutes les réponses renvoyées par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="05398-104">The **AutodiscoverResponse (SOAP)** element represents the base element for all responses that are returned by the Autodiscover service.</span></span> 
  
- [<span data-ttu-id="05398-105">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05398-105">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md)
  
```XML
<AutodiscoverResponse>
    <UserResponses/>
    <UserSettingErrors/>
    <UserSettings/>
</AutodiscoverResponse>

```

 <span data-ttu-id="05398-106">**AutodiscoverResponse**</span><span class="sxs-lookup"><span data-stu-id="05398-106">**AutodiscoverResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05398-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="05398-107">Attributes and elements</span></span>

<span data-ttu-id="05398-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="05398-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05398-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="05398-109">Attributes</span></span>

<span data-ttu-id="05398-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="05398-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05398-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="05398-111">Child elements</span></span>

|<span data-ttu-id="05398-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="05398-112">**Element**</span></span>|<span data-ttu-id="05398-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="05398-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05398-114">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05398-114">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="05398-115">Représente une collection d’éléments [UserResponse (SOAP)](userresponse-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="05398-115">Represents a collection of [UserResponse (SOAP)](userresponse-soap.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="05398-116">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05398-116">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="05398-117">Représente une collection d’éléments [UserSettingError (SOAP)](usersettingerror-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="05398-117">Represents a collection of [UserSettingError (SOAP)](usersettingerror-soap.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="05398-118">UserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05398-118">UserSettings (SOAP)</span></span>](usersettings-soap.md) <br/> |<span data-ttu-id="05398-119">Représente une collection d’éléments [UserSetting (SOAP)](usersetting-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="05398-119">Represents a collection of [UserSetting (SOAP)](usersetting-soap.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="05398-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="05398-120">Parent elements</span></span>

<span data-ttu-id="05398-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05398-121">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="05398-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="05398-122">Text value</span></span>

<span data-ttu-id="05398-123">Aucune.</span><span class="sxs-lookup"><span data-stu-id="05398-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05398-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="05398-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05398-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="05398-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="05398-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="05398-126">Schema Name</span></span>  <br/> |<span data-ttu-id="05398-127">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="05398-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="05398-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="05398-128">Validation File</span></span>  <br/> |<span data-ttu-id="05398-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="05398-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="05398-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="05398-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="05398-131">True</span><span class="sxs-lookup"><span data-stu-id="05398-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05398-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05398-132">See also</span></span>

- [<span data-ttu-id="05398-133">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05398-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="05398-134">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05398-134">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)
- [<span data-ttu-id="05398-135">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05398-135">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

