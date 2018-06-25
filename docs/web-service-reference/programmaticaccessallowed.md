---
title: ProgrammaticAccessAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a1fc7dff-a303-4809-b7f4-9672f86c183c
description: L’élément ProgrammaticAccessAllowed indique si l’accès par programme est activée pour les données gérées par des droits.
ms.openlocfilehash: 50bcce745bd94bf9c2e5ced93825722307e0a096
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828889"
---
# <a name="programmaticaccessallowed"></a><span data-ttu-id="cc26e-103">ProgrammaticAccessAllowed</span><span class="sxs-lookup"><span data-stu-id="cc26e-103">ProgrammaticAccessAllowed</span></span>

<span data-ttu-id="cc26e-104">L’élément **ProgrammaticAccessAllowed** indique si l’accès par programme est activée pour les données gérées par des droits.</span><span class="sxs-lookup"><span data-stu-id="cc26e-104">The **ProgrammaticAccessAllowed** element specifies whether programmatic access is enabled for rights managed data.</span></span> 
  
```XML
<ProgrammaticAccessAllowed> true | false </ProgrammaticAccessAllowed>
```

 <span data-ttu-id="cc26e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="cc26e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc26e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cc26e-106">Attributes and elements</span></span>

<span data-ttu-id="cc26e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cc26e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc26e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cc26e-108">Attributes</span></span>

<span data-ttu-id="cc26e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cc26e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc26e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cc26e-110">Child elements</span></span>

<span data-ttu-id="cc26e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cc26e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cc26e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cc26e-112">Parent elements</span></span>

[<span data-ttu-id="cc26e-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="cc26e-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="cc26e-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="cc26e-114">Text value</span></span>

<span data-ttu-id="cc26e-115">Une valeur de texte de **la valeur true** pour l’élément **ProgrammaticAccessAllowed** indique que les données sont accessibles par programme.</span><span class="sxs-lookup"><span data-stu-id="cc26e-115">A text value of **true** for the **ProgrammaticAccessAllowed** element indicates that the data is programmatically accessible.</span></span> <span data-ttu-id="cc26e-116">La valeur **false** indique que les données ne sont pas accessibles par programme.</span><span class="sxs-lookup"><span data-stu-id="cc26e-116">A value of **false** indicates that the data is not programmatically accessible.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cc26e-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="cc26e-117">Remarks</span></span>

<span data-ttu-id="cc26e-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cc26e-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cc26e-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc26e-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc26e-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cc26e-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc26e-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cc26e-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cc26e-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cc26e-122">Schema name</span></span>  <br/> |<span data-ttu-id="cc26e-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cc26e-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="cc26e-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cc26e-124">Validation file</span></span>  <br/> |<span data-ttu-id="cc26e-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cc26e-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cc26e-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cc26e-126">Can be empty</span></span>  <br/> |<span data-ttu-id="cc26e-127">false</span><span class="sxs-lookup"><span data-stu-id="cc26e-127">false</span></span>  <br/> |
   

