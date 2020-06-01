---
title: IsPermanentFailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: L’élément IsPermanentFailure indique si une précédente tentative d’indexation de l’élément a échoué.
ms.openlocfilehash: 48a13eebfa16c538c1b10d92f080d51f1b318d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460392"
---
# <a name="ispermanentfailure"></a><span data-ttu-id="3888e-103">IsPermanentFailure</span><span class="sxs-lookup"><span data-stu-id="3888e-103">IsPermanentFailure</span></span>

<span data-ttu-id="3888e-104">L’élément **IsPermanentFailure** indique si une précédente tentative d’indexation de l’élément a échoué.</span><span class="sxs-lookup"><span data-stu-id="3888e-104">The **IsPermanentFailure** element indicates whether a previous attempt to index the item was unsuccessful.</span></span> 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 <span data-ttu-id="3888e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3888e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3888e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3888e-106">Attributes and elements</span></span>

<span data-ttu-id="3888e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3888e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3888e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3888e-108">Attributes</span></span>

<span data-ttu-id="3888e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3888e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3888e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3888e-110">Child elements</span></span>

<span data-ttu-id="3888e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3888e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3888e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3888e-112">Parent elements</span></span>

[<span data-ttu-id="3888e-113">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="3888e-113">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
  
## <a name="text-value"></a><span data-ttu-id="3888e-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="3888e-114">Text value</span></span>

<span data-ttu-id="3888e-115">Une valeur de texte de **true** pour l’élément **IsPermanentFailure** indique qu’une tentative précédente d’indexation de l’élément de boîte aux lettres a échoué.</span><span class="sxs-lookup"><span data-stu-id="3888e-115">A text value of **true** for the **IsPermanentFailure** element indicates that a previous attempt to index the mailbox item was unsuccessful.</span></span> <span data-ttu-id="3888e-116">La valeur **false** indique qu’une précédente tentative d’indexation de l’élément de boîte aux lettres a réussi.</span><span class="sxs-lookup"><span data-stu-id="3888e-116">A value of **false** indicates that a previous attempt to index the mailbox item was successful.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3888e-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="3888e-117">Remarks</span></span>

<span data-ttu-id="3888e-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3888e-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3888e-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3888e-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3888e-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3888e-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3888e-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3888e-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3888e-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3888e-122">Schema name</span></span>  <br/> |<span data-ttu-id="3888e-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3888e-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="3888e-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3888e-124">Validation file</span></span>  <br/> |<span data-ttu-id="3888e-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3888e-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3888e-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3888e-126">Can be empty</span></span>  <br/> |<span data-ttu-id="3888e-127">false</span><span class="sxs-lookup"><span data-stu-id="3888e-127">false</span></span>  <br/> |
   

