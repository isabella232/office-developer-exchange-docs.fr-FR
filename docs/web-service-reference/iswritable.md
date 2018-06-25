---
title: IsWritable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: L’élément IsWritable Spécifie si l’ou les destinataires d’Active Directory sous-jacent peut être écrite.
ms.openlocfilehash: 03f258d01ecfc12dfa4e09ac88f4a75340d2acf3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828158"
---
# <a name="iswritable"></a><span data-ttu-id="a71ed-103">IsWritable</span><span class="sxs-lookup"><span data-stu-id="a71ed-103">IsWritable</span></span>

<span data-ttu-id="a71ed-104">L’élément **IsWritable** Spécifie si l’ou les destinataires d’Active Directory sous-jacent peut être écrite.</span><span class="sxs-lookup"><span data-stu-id="a71ed-104">The **IsWritable** element specifies whether the underlying contact or Active Directory recipient can be written to.</span></span> 
  
```XML
<IsWritable> true | false </IsWritable>
```

 <span data-ttu-id="a71ed-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a71ed-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a71ed-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a71ed-106">Attributes and elements</span></span>

<span data-ttu-id="a71ed-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a71ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a71ed-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a71ed-108">Attributes</span></span>

<span data-ttu-id="a71ed-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a71ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a71ed-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a71ed-110">Child elements</span></span>

<span data-ttu-id="a71ed-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a71ed-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a71ed-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a71ed-112">Parent elements</span></span>

[<span data-ttu-id="a71ed-113">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="a71ed-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
  
## <a name="text-value"></a><span data-ttu-id="a71ed-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a71ed-114">Text value</span></span>

<span data-ttu-id="a71ed-115">Une valeur de texte de **la valeur true** pour l’élément **IsWritable** indique que le contact ou un objet Active Directory est accessible en écriture.</span><span class="sxs-lookup"><span data-stu-id="a71ed-115">A text value of **true** for the **IsWritable** element indicates that the contact or Active Directory object is available for write access.</span></span> <span data-ttu-id="a71ed-116">La valeur **false** indique que le contact ou un objet Active Directory n’est pas disponible pour un accès en écriture.</span><span class="sxs-lookup"><span data-stu-id="a71ed-116">A value of **false** indicates that the contact or Active Directory object is not available for write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a71ed-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="a71ed-117">Remarks</span></span>

<span data-ttu-id="a71ed-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a71ed-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a71ed-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a71ed-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

