---
title: UserParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: L’élément UserParameters contient la liste des extensions clientes activées et désactivées.
ms.openlocfilehash: 76bf858adfb6d2ef76a25c234117131752c60d7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526752"
---
# <a name="userparameters"></a><span data-ttu-id="66f4b-103">UserParameters</span><span class="sxs-lookup"><span data-stu-id="66f4b-103">UserParameters</span></span>

<span data-ttu-id="66f4b-104">L’élément **UserParameters** contient la liste des extensions clientes activées et désactivées.</span><span class="sxs-lookup"><span data-stu-id="66f4b-104">The **UserParameters** element contains a list of enabled and disabled client extensions.</span></span> 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 <span data-ttu-id="66f4b-105">**GetClientExtensionUserParametersType**</span><span class="sxs-lookup"><span data-stu-id="66f4b-105">**GetClientExtensionUserParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66f4b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="66f4b-106">Attributes and elements</span></span>

<span data-ttu-id="66f4b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="66f4b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66f4b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="66f4b-108">Attributes</span></span>

|<span data-ttu-id="66f4b-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="66f4b-109">**Attribute**</span></span>|<span data-ttu-id="66f4b-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="66f4b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="66f4b-111">UserId</span><span class="sxs-lookup"><span data-stu-id="66f4b-111">UserId</span></span>  <br/> |<span data-ttu-id="66f4b-112">La valeur de texte de l’attribut **userid** est l’identificateur de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="66f4b-112">The text value of the **UserId** attribute is the identifier of the user.</span></span>  <br/> |
|<span data-ttu-id="66f4b-113">EnabledOnly</span><span class="sxs-lookup"><span data-stu-id="66f4b-113">EnabledOnly</span></span>  <br/> |<span data-ttu-id="66f4b-114">La valeur de texte de la **EnabledOnly** indique si la réponse ne contient que les extensions activées.</span><span class="sxs-lookup"><span data-stu-id="66f4b-114">The text value of the **EnabledOnly** indicates whether the response only contains the enabled extensions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="66f4b-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="66f4b-115">Child elements</span></span>

<span data-ttu-id="66f4b-116">[UserEnabledExtensions](userenabledextensions.md)  |  [UserDisabledExtensions](userdisabledextensions.md)</span><span class="sxs-lookup"><span data-stu-id="66f4b-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="66f4b-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="66f4b-117">Parent elements</span></span>

[<span data-ttu-id="66f4b-118">GetClientExtension</span><span class="sxs-lookup"><span data-stu-id="66f4b-118">GetClientExtension</span></span>](getclientextension.md)
  
## <a name="remarks"></a><span data-ttu-id="66f4b-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="66f4b-119">Remarks</span></span>

<span data-ttu-id="66f4b-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="66f4b-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="66f4b-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="66f4b-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66f4b-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="66f4b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66f4b-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="66f4b-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="66f4b-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="66f4b-124">Schema name</span></span>  <br/> |<span data-ttu-id="66f4b-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="66f4b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="66f4b-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="66f4b-126">Validation file</span></span>  <br/> |<span data-ttu-id="66f4b-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="66f4b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="66f4b-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="66f4b-128">Can be empty</span></span>  <br/> ||
   

