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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838970"
---
# <a name="userparameters"></a><span data-ttu-id="12da1-103">UserParameters</span><span class="sxs-lookup"><span data-stu-id="12da1-103">UserParameters</span></span>

<span data-ttu-id="12da1-104">L’élément **UserParameters** contient une liste des extensions de client activé et désactivé.</span><span class="sxs-lookup"><span data-stu-id="12da1-104">The **UserParameters** element contains a list of enabled and disabled client extensions.</span></span> 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 <span data-ttu-id="12da1-105">**GetClientExtensionUserParametersType**</span><span class="sxs-lookup"><span data-stu-id="12da1-105">**GetClientExtensionUserParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12da1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="12da1-106">Attributes and elements</span></span>

<span data-ttu-id="12da1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="12da1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12da1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="12da1-108">Attributes</span></span>

|<span data-ttu-id="12da1-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="12da1-109">**Attribute**</span></span>|<span data-ttu-id="12da1-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="12da1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="12da1-111">UserId</span><span class="sxs-lookup"><span data-stu-id="12da1-111">UserId</span></span>  <br/> |<span data-ttu-id="12da1-112">La valeur de texte de l’attribut **UserId** est l’identificateur de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="12da1-112">The text value of the **UserId** attribute is the identifier of the user.</span></span>  <br/> |
|<span data-ttu-id="12da1-113">EnabledOnly</span><span class="sxs-lookup"><span data-stu-id="12da1-113">EnabledOnly</span></span>  <br/> |<span data-ttu-id="12da1-114">La valeur de texte de **EnabledOnly** indique si la réponse contient uniquement les extensions activées.</span><span class="sxs-lookup"><span data-stu-id="12da1-114">The text value of the **EnabledOnly** indicates whether the response only contains the enabled extensions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="12da1-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="12da1-115">Child elements</span></span>

<span data-ttu-id="12da1-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span><span class="sxs-lookup"><span data-stu-id="12da1-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12da1-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="12da1-117">Parent elements</span></span>

[<span data-ttu-id="12da1-118">GetClientExtension</span><span class="sxs-lookup"><span data-stu-id="12da1-118">GetClientExtension</span></span>](getclientextension.md)
  
## <a name="remarks"></a><span data-ttu-id="12da1-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="12da1-119">Remarks</span></span>

<span data-ttu-id="12da1-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="12da1-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="12da1-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="12da1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12da1-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="12da1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12da1-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="12da1-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12da1-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="12da1-124">Schema name</span></span>  <br/> |<span data-ttu-id="12da1-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="12da1-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="12da1-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="12da1-126">Validation file</span></span>  <br/> |<span data-ttu-id="12da1-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="12da1-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12da1-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="12da1-128">Can be empty</span></span>  <br/> ||
   

