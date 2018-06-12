---
title: IsPermanentFailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: L’élément IsPermanentFailure indique si une tentative précédente d’index de l’élément a échoué.
ms.openlocfilehash: 39592c15394a57e1c6aa1183ed0ccedeb085e6ea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828085"
---
# <a name="ispermanentfailure"></a><span data-ttu-id="89d36-103">IsPermanentFailure</span><span class="sxs-lookup"><span data-stu-id="89d36-103">IsPermanentFailure</span></span>

<span data-ttu-id="89d36-104">L’élément **IsPermanentFailure** indique si une tentative précédente d’index de l’élément a échoué.</span><span class="sxs-lookup"><span data-stu-id="89d36-104">The **IsPermanentFailure** element indicates whether a previous attempt to index the item was unsuccessful.</span></span> 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 <span data-ttu-id="89d36-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="89d36-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89d36-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="89d36-106">Attributes and elements</span></span>

<span data-ttu-id="89d36-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="89d36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89d36-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="89d36-108">Attributes</span></span>

<span data-ttu-id="89d36-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="89d36-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89d36-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="89d36-110">Child elements</span></span>

<span data-ttu-id="89d36-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="89d36-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="89d36-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="89d36-112">Parent elements</span></span>

[<span data-ttu-id="89d36-113">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="89d36-113">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
  
## <a name="text-value"></a><span data-ttu-id="89d36-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="89d36-114">Text value</span></span>

<span data-ttu-id="89d36-115">Une valeur de texte de **la valeur true** pour l’élément **IsPermanentFailure** indique qu’une tentative précédente d’index de l’élément de boîte aux lettres a échoué.</span><span class="sxs-lookup"><span data-stu-id="89d36-115">A text value of **true** for the **IsPermanentFailure** element indicates that a previous attempt to index the mailbox item was unsuccessful.</span></span> <span data-ttu-id="89d36-116">La valeur **false** indique qu’une tentative précédente d’index de l’élément de boîte aux lettres a réussi.</span><span class="sxs-lookup"><span data-stu-id="89d36-116">A value of **false** indicates that a previous attempt to index the mailbox item was successful.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="89d36-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="89d36-117">Remarks</span></span>

<span data-ttu-id="89d36-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="89d36-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="89d36-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="89d36-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89d36-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="89d36-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89d36-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="89d36-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89d36-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="89d36-122">Schema name</span></span>  <br/> |<span data-ttu-id="89d36-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="89d36-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="89d36-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="89d36-124">Validation file</span></span>  <br/> |<span data-ttu-id="89d36-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="89d36-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="89d36-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="89d36-126">Can be empty</span></span>  <br/> |<span data-ttu-id="89d36-127">false</span><span class="sxs-lookup"><span data-stu-id="89d36-127">false</span></span>  <br/> |
   

