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
description: L’élément UserSettingErrors représente une collection d’informations sur les paramètres qui n’ont pas pu être renvoyés.
ms.openlocfilehash: a6cc0fe114bd511dc4136532986b552c28b0d5c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467122"
---
# <a name="usersettingerrors-soap"></a><span data-ttu-id="e8632-103">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e8632-103">UserSettingErrors (SOAP)</span></span>

<span data-ttu-id="e8632-104">L’élément **UserSettingErrors** représente une collection d’informations sur les paramètres qui n’ont pas pu être renvoyés.</span><span class="sxs-lookup"><span data-stu-id="e8632-104">The **UserSettingErrors** element represents a collection of information about settings that could not be returned.</span></span> 
  
```XML
<UserSettingErrors>
    <UserSettingError/>
</UserSettingErrors>
```

 <span data-ttu-id="e8632-105">**UserSettingErrors**</span><span class="sxs-lookup"><span data-stu-id="e8632-105">**UserSettingErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8632-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e8632-106">Attributes and elements</span></span>

<span data-ttu-id="e8632-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e8632-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8632-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e8632-108">Attributes</span></span>

<span data-ttu-id="e8632-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e8632-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8632-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e8632-110">Child elements</span></span>

|<span data-ttu-id="e8632-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e8632-111">**Element**</span></span>|<span data-ttu-id="e8632-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e8632-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8632-113">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e8632-113">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="e8632-114">Représente une erreur renvoyée lors de la récupération d’un paramètre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e8632-114">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8632-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e8632-115">Parent elements</span></span>

|<span data-ttu-id="e8632-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e8632-116">**Element**</span></span>|<span data-ttu-id="e8632-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="e8632-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8632-118">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e8632-118">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="e8632-119">Représente une réponse à une demande GetUserSettings pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="e8632-119">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e8632-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e8632-120">Text value</span></span>

<span data-ttu-id="e8632-121">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e8632-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8632-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e8632-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8632-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e8632-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e8632-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e8632-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e8632-125">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="e8632-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e8632-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e8632-126">Validation File</span></span>  <br/> |<span data-ttu-id="e8632-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e8632-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8632-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e8632-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8632-129">True</span><span class="sxs-lookup"><span data-stu-id="e8632-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8632-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e8632-130">See also</span></span>



[<span data-ttu-id="e8632-131">Éléments XML de découverte automatique SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e8632-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

