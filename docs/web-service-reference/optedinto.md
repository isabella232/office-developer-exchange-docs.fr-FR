---
title: OptedInto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 083a23d9-acc3-4c15-9d30-c20bf7e6808d
description: L’élément OptedInto spécifie une valeur de type Boolean qui indique si l’utilisateur connecté à la stratégie de rétention.
ms.openlocfilehash: 0d8fb2b07c6c98ba6973ab6efabe9c35d2d1ac12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828657"
---
# <a name="optedinto"></a><span data-ttu-id="a9fec-103">OptedInto</span><span class="sxs-lookup"><span data-stu-id="a9fec-103">OptedInto</span></span>

<span data-ttu-id="a9fec-104">L’élément **OptedInto** spécifie une valeur de type Boolean qui indique si l’utilisateur connecté à la stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="a9fec-104">The **OptedInto** element specifies a Boolean value that indicates whether the user opted in to the retention policy.</span></span> 
  
```XML
<OptedInto>true | false</OptedInto>
```

 <span data-ttu-id="a9fec-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a9fec-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a9fec-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a9fec-106">Attributes and elements</span></span>

<span data-ttu-id="a9fec-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a9fec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9fec-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a9fec-108">Attributes</span></span>

<span data-ttu-id="a9fec-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a9fec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a9fec-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a9fec-110">Child elements</span></span>

<span data-ttu-id="a9fec-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a9fec-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a9fec-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a9fec-112">Parent elements</span></span>

[<span data-ttu-id="a9fec-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="a9fec-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="a9fec-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a9fec-114">Text value</span></span>

<span data-ttu-id="a9fec-115">Une valeur de texte de **la valeur true** pour l’élément **OptedInto** indique que l’utilisateur connecté à la stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="a9fec-115">A text value of **true** for the **OptedInto** element indicates that the user opted in to the retention policy.</span></span> <span data-ttu-id="a9fec-116">La valeur **false** indique que l’utilisateur ne pas inclure dans la stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="a9fec-116">A value of **false** indicates that the user did not opt into the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a9fec-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="a9fec-117">Remarks</span></span>

<span data-ttu-id="a9fec-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a9fec-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a9fec-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9fec-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a9fec-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a9fec-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a9fec-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a9fec-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a9fec-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a9fec-122">Schema name</span></span>  <br/> |<span data-ttu-id="a9fec-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a9fec-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="a9fec-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a9fec-124">Validation file</span></span>  <br/> |<span data-ttu-id="a9fec-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a9fec-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a9fec-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a9fec-126">Can be empty</span></span>  <br/> ||
   

