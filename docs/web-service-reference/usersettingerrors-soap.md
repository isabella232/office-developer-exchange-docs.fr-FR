---
title: UserSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a9b94bae-cab9-412d-a811-801e849ed6c5
description: L’élément UserSettingErrors représente une collection d’informations sur les paramètres qui ne peut pas être retourné.
ms.openlocfilehash: 4477c30145d2cb187a4309d018512537af974ee8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838984"
---
# <a name="usersettingerrors-soap"></a><span data-ttu-id="8816d-103">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8816d-103">UserSettingErrors (SOAP)</span></span>

<span data-ttu-id="8816d-104">L’élément **UserSettingErrors** représente une collection d’informations sur les paramètres qui ne peut pas être retourné.</span><span class="sxs-lookup"><span data-stu-id="8816d-104">The **UserSettingErrors** element represents a collection of information about settings that could not be returned.</span></span> 
  
```XML
<UserSettingErrors>
    <UserSettingError/>
</UserSettingErrors>
```

 <span data-ttu-id="8816d-105">**UserSettingErrors**</span><span class="sxs-lookup"><span data-stu-id="8816d-105">**UserSettingErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8816d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8816d-106">Attributes and elements</span></span>

<span data-ttu-id="8816d-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8816d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8816d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8816d-108">Attributes</span></span>

<span data-ttu-id="8816d-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8816d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8816d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8816d-110">Child elements</span></span>

|<span data-ttu-id="8816d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8816d-111">**Element**</span></span>|<span data-ttu-id="8816d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8816d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8816d-113">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8816d-113">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="8816d-114">Représente une erreur est renvoyée lors de la récupération d’un paramètre de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8816d-114">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8816d-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8816d-115">Parent elements</span></span>

|<span data-ttu-id="8816d-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8816d-116">**Element**</span></span>|<span data-ttu-id="8816d-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="8816d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8816d-118">Réponse de l’utilisateur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8816d-118">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="8816d-119">Représente une réponse à une demande de GetUserSettings pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="8816d-119">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8816d-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8816d-120">Text value</span></span>

<span data-ttu-id="8816d-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8816d-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8816d-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8816d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8816d-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8816d-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="8816d-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8816d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8816d-125">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="8816d-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="8816d-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8816d-126">Validation File</span></span>  <br/> |<span data-ttu-id="8816d-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8816d-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8816d-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8816d-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8816d-129">True</span><span class="sxs-lookup"><span data-stu-id="8816d-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8816d-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8816d-130">See also</span></span>



[<span data-ttu-id="8816d-131">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8816d-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

