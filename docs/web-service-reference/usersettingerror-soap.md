---
title: UserSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: abb175c5-4f38-4dcc-81e3-b511686862eb
description: L’élément UserSettingError représente une erreur qui est renvoyée à la suite d’une tentative d’obtention d’un paramètre de l’utilisateur.
ms.openlocfilehash: 886e0be0aa900ce3a00902c21cc115e866d0cd99
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838978"
---
# <a name="usersettingerror-soap"></a><span data-ttu-id="54c7c-103">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="54c7c-103">UserSettingError (SOAP)</span></span>

<span data-ttu-id="54c7c-104">L’élément **UserSettingError** représente une erreur qui est renvoyée à la suite d’une tentative d’obtention d’un paramètre de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="54c7c-104">The **UserSettingError** element represents an error that is returned as a result of an attempt to get a user setting.</span></span> 
  
```XML
<UserSettingError>
    <ErrorCode/>
    <ErrorMessage/>
    <SettingName/>
</UserSettingError>
```

 <span data-ttu-id="54c7c-105">**UserSettingError**</span><span class="sxs-lookup"><span data-stu-id="54c7c-105">**UserSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54c7c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="54c7c-106">Attributes and elements</span></span>

<span data-ttu-id="54c7c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="54c7c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54c7c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="54c7c-108">Attributes</span></span>

<span data-ttu-id="54c7c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="54c7c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54c7c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="54c7c-110">Child elements</span></span>

|<span data-ttu-id="54c7c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="54c7c-111">**Element**</span></span>|<span data-ttu-id="54c7c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="54c7c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54c7c-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="54c7c-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="54c7c-114">Représente un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="54c7c-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="54c7c-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="54c7c-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="54c7c-116">Représente un message associé à un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="54c7c-116">Respresents a message associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="54c7c-117">Nom du paramètre (SOAP)</span><span class="sxs-lookup"><span data-stu-id="54c7c-117">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="54c7c-118">Représente le nom d’un paramètre de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="54c7c-118">Represents the name of a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54c7c-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="54c7c-119">Parent elements</span></span>

|<span data-ttu-id="54c7c-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="54c7c-120">**Element**</span></span>|<span data-ttu-id="54c7c-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="54c7c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54c7c-122">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="54c7c-122">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="54c7c-123">Représente une collection d’informations sur les paramètres qui ne peut pas être retourné.</span><span class="sxs-lookup"><span data-stu-id="54c7c-123">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="54c7c-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="54c7c-124">Text value</span></span>

<span data-ttu-id="54c7c-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="54c7c-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54c7c-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="54c7c-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54c7c-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="54c7c-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="54c7c-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="54c7c-128">Schema Name</span></span>  <br/> |<span data-ttu-id="54c7c-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="54c7c-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="54c7c-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="54c7c-130">Validation File</span></span>  <br/> |<span data-ttu-id="54c7c-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="54c7c-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54c7c-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="54c7c-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="54c7c-133">True</span><span class="sxs-lookup"><span data-stu-id="54c7c-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54c7c-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="54c7c-134">See also</span></span>



[<span data-ttu-id="54c7c-135">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="54c7c-135">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

