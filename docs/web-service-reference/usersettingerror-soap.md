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
description: L’élément UserSettingError représente une erreur qui est renvoyée suite à une tentative d’obtention d’un paramètre utilisateur.
ms.openlocfilehash: 61603038ce93780f690d72226b1356b239d2002d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468606"
---
# <a name="usersettingerror-soap"></a><span data-ttu-id="04571-103">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="04571-103">UserSettingError (SOAP)</span></span>

<span data-ttu-id="04571-104">L’élément **UserSettingError** représente une erreur qui est renvoyée suite à une tentative d’obtention d’un paramètre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="04571-104">The **UserSettingError** element represents an error that is returned as a result of an attempt to get a user setting.</span></span> 
  
```XML
<UserSettingError>
    <ErrorCode/>
    <ErrorMessage/>
    <SettingName/>
</UserSettingError>
```

 <span data-ttu-id="04571-105">**UserSettingError**</span><span class="sxs-lookup"><span data-stu-id="04571-105">**UserSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04571-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="04571-106">Attributes and elements</span></span>

<span data-ttu-id="04571-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="04571-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04571-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="04571-108">Attributes</span></span>

<span data-ttu-id="04571-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="04571-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04571-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="04571-110">Child elements</span></span>

|<span data-ttu-id="04571-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04571-111">**Element**</span></span>|<span data-ttu-id="04571-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="04571-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04571-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="04571-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="04571-114">Représente un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="04571-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="04571-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="04571-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="04571-116">Représenté par un message associé à un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="04571-116">Respresents a message associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="04571-117">Propriétés SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="04571-117">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="04571-118">Représente le nom d’un paramètre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="04571-118">Represents the name of a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04571-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="04571-119">Parent elements</span></span>

|<span data-ttu-id="04571-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04571-120">**Element**</span></span>|<span data-ttu-id="04571-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="04571-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04571-122">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="04571-122">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="04571-123">Représente une collection d’informations sur les paramètres qui n’ont pas pu être renvoyés.</span><span class="sxs-lookup"><span data-stu-id="04571-123">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04571-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="04571-124">Text value</span></span>

<span data-ttu-id="04571-125">Aucune.</span><span class="sxs-lookup"><span data-stu-id="04571-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04571-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="04571-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04571-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="04571-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="04571-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="04571-128">Schema Name</span></span>  <br/> |<span data-ttu-id="04571-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="04571-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="04571-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="04571-130">Validation File</span></span>  <br/> |<span data-ttu-id="04571-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="04571-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="04571-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="04571-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="04571-133">True</span><span class="sxs-lookup"><span data-stu-id="04571-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04571-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="04571-134">See also</span></span>



[<span data-ttu-id="04571-135">Éléments XML de découverte automatique SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="04571-135">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

