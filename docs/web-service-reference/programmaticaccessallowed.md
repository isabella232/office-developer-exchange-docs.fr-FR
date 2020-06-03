---
title: ProgrammaticAccessAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a1fc7dff-a303-4809-b7f4-9672f86c183c
description: L’élément ProgrammaticAccessAllowed spécifie si l’accès par programme est activé pour les données gérées par des droits.
ms.openlocfilehash: 8a5cf4e57a97807e5940a0402768d7123b9912d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465638"
---
# <a name="programmaticaccessallowed"></a><span data-ttu-id="64a4f-103">ProgrammaticAccessAllowed</span><span class="sxs-lookup"><span data-stu-id="64a4f-103">ProgrammaticAccessAllowed</span></span>

<span data-ttu-id="64a4f-104">L’élément **ProgrammaticAccessAllowed** spécifie si l’accès par programme est activé pour les données gérées par des droits.</span><span class="sxs-lookup"><span data-stu-id="64a4f-104">The **ProgrammaticAccessAllowed** element specifies whether programmatic access is enabled for rights managed data.</span></span> 
  
```XML
<ProgrammaticAccessAllowed> true | false </ProgrammaticAccessAllowed>
```

 <span data-ttu-id="64a4f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="64a4f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64a4f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="64a4f-106">Attributes and elements</span></span>

<span data-ttu-id="64a4f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="64a4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64a4f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="64a4f-108">Attributes</span></span>

<span data-ttu-id="64a4f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="64a4f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64a4f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="64a4f-110">Child elements</span></span>

<span data-ttu-id="64a4f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="64a4f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="64a4f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="64a4f-112">Parent elements</span></span>

[<span data-ttu-id="64a4f-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="64a4f-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="64a4f-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="64a4f-114">Text value</span></span>

<span data-ttu-id="64a4f-115">Une valeur de texte de **true** pour l’élément **ProgrammaticAccessAllowed** indique que les données sont accessibles par programme.</span><span class="sxs-lookup"><span data-stu-id="64a4f-115">A text value of **true** for the **ProgrammaticAccessAllowed** element indicates that the data is programmatically accessible.</span></span> <span data-ttu-id="64a4f-116">La valeur **false** indique que les données ne sont pas accessibles par programme.</span><span class="sxs-lookup"><span data-stu-id="64a4f-116">A value of **false** indicates that the data is not programmatically accessible.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="64a4f-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="64a4f-117">Remarks</span></span>

<span data-ttu-id="64a4f-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="64a4f-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="64a4f-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="64a4f-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64a4f-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="64a4f-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64a4f-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="64a4f-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64a4f-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="64a4f-122">Schema name</span></span>  <br/> |<span data-ttu-id="64a4f-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="64a4f-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="64a4f-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="64a4f-124">Validation file</span></span>  <br/> |<span data-ttu-id="64a4f-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="64a4f-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64a4f-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="64a4f-126">Can be empty</span></span>  <br/> |<span data-ttu-id="64a4f-127">false</span><span class="sxs-lookup"><span data-stu-id="64a4f-127">false</span></span>  <br/> |
   

