---
title: UserParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: L’élément UserParameters contient une liste des extensions de client activé et désactivé.
ms.openlocfilehash: e0a72fe13255380ee56b32c863fb3bffb2e1ac5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838970"
---
# <a name="userparameters"></a><span data-ttu-id="56aa4-103">UserParameters</span><span class="sxs-lookup"><span data-stu-id="56aa4-103">UserParameters</span></span>

<span data-ttu-id="56aa4-104">L’élément **UserParameters** contient une liste des extensions de client activé et désactivé.</span><span class="sxs-lookup"><span data-stu-id="56aa4-104">The **UserParameters** element contains a list of enabled and disabled client extensions.</span></span> 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 <span data-ttu-id="56aa4-105">**GetClientExtensionUserParametersType**</span><span class="sxs-lookup"><span data-stu-id="56aa4-105">**GetClientExtensionUserParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56aa4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="56aa4-106">Attributes and elements</span></span>

<span data-ttu-id="56aa4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="56aa4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56aa4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="56aa4-108">Attributes</span></span>

|<span data-ttu-id="56aa4-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="56aa4-109">**Attribute**</span></span>|<span data-ttu-id="56aa4-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="56aa4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="56aa4-111">UserId</span><span class="sxs-lookup"><span data-stu-id="56aa4-111">UserId</span></span>  <br/> |<span data-ttu-id="56aa4-112">La valeur de texte de l’attribut **UserId** est l’identificateur de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="56aa4-112">The text value of the **UserId** attribute is the identifier of the user.</span></span>  <br/> |
|<span data-ttu-id="56aa4-113">EnabledOnly</span><span class="sxs-lookup"><span data-stu-id="56aa4-113">EnabledOnly</span></span>  <br/> |<span data-ttu-id="56aa4-114">La valeur de texte de **EnabledOnly** indique si la réponse contient uniquement les extensions activées.</span><span class="sxs-lookup"><span data-stu-id="56aa4-114">The text value of the **EnabledOnly** indicates whether the response only contains the enabled extensions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="56aa4-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="56aa4-115">Child elements</span></span>

<span data-ttu-id="56aa4-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span><span class="sxs-lookup"><span data-stu-id="56aa4-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="56aa4-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="56aa4-117">Parent elements</span></span>

[<span data-ttu-id="56aa4-118">GetClientExtension</span><span class="sxs-lookup"><span data-stu-id="56aa4-118">GetClientExtension</span></span>](getclientextension.md)
  
## <a name="remarks"></a><span data-ttu-id="56aa4-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="56aa4-119">Remarks</span></span>

<span data-ttu-id="56aa4-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="56aa4-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="56aa4-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="56aa4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56aa4-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="56aa4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56aa4-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="56aa4-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56aa4-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="56aa4-124">Schema name</span></span>  <br/> |<span data-ttu-id="56aa4-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="56aa4-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="56aa4-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="56aa4-126">Validation file</span></span>  <br/> |<span data-ttu-id="56aa4-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="56aa4-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="56aa4-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="56aa4-128">Can be empty</span></span>  <br/> ||
   

