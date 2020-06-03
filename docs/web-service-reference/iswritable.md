---
title: IsWritable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: L’élément IsWritable spécifie si le contact sous-jacent ou le destinataire Active Directory peut être écrit.
ms.openlocfilehash: 96075adc1772027456f8829eee43bdc734644c09
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467570"
---
# <a name="iswritable"></a><span data-ttu-id="b2b57-103">IsWritable</span><span class="sxs-lookup"><span data-stu-id="b2b57-103">IsWritable</span></span>

<span data-ttu-id="b2b57-104">L’élément **isWritable** spécifie si le contact sous-jacent ou le destinataire Active Directory peut être écrit.</span><span class="sxs-lookup"><span data-stu-id="b2b57-104">The **IsWritable** element specifies whether the underlying contact or Active Directory recipient can be written to.</span></span> 
  
```XML
<IsWritable> true | false </IsWritable>
```

 <span data-ttu-id="b2b57-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b2b57-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2b57-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b2b57-106">Attributes and elements</span></span>

<span data-ttu-id="b2b57-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b2b57-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2b57-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b2b57-108">Attributes</span></span>

<span data-ttu-id="b2b57-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b2b57-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2b57-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b2b57-110">Child elements</span></span>

<span data-ttu-id="b2b57-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b2b57-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2b57-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b2b57-112">Parent elements</span></span>

[<span data-ttu-id="b2b57-113">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="b2b57-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
  
## <a name="text-value"></a><span data-ttu-id="b2b57-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="b2b57-114">Text value</span></span>

<span data-ttu-id="b2b57-115">Une valeur de texte de **true** pour l’élément **isWritable** indique que l’objet contact ou Active Directory est disponible pour l’accès en écriture.</span><span class="sxs-lookup"><span data-stu-id="b2b57-115">A text value of **true** for the **IsWritable** element indicates that the contact or Active Directory object is available for write access.</span></span> <span data-ttu-id="b2b57-116">La valeur **false** indique que l’objet contact ou Active Directory n’est pas disponible pour l’accès en écriture.</span><span class="sxs-lookup"><span data-stu-id="b2b57-116">A value of **false** indicates that the contact or Active Directory object is not available for write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b2b57-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="b2b57-117">Remarks</span></span>

<span data-ttu-id="b2b57-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b2b57-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b2b57-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2b57-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

