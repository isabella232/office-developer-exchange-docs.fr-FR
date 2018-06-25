---
title: NonIndexableItemDetail
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a26d4c02-f1bd-40c4-9257-5db45e839f17
description: L’élément NonIndexableItemDetail spécifie des informations détaillées sur un élément qui ne peuvent pas être indexé.
ms.openlocfilehash: ef1bd072a44b42b501a3016c394b89fe6ab25bf0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828543"
---
# <a name="nonindexableitemdetail"></a><span data-ttu-id="702f7-103">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="702f7-103">NonIndexableItemDetail</span></span>

<span data-ttu-id="702f7-104">L’élément **NonIndexableItemDetail** spécifie des informations détaillées sur un élément qui ne peuvent pas être indexé.</span><span class="sxs-lookup"><span data-stu-id="702f7-104">The **NonIndexableItemDetail** element specifies detail information about an item that cannot be indexed.</span></span> 
  
```XML
<NonIndexableItemDetail>
   <ItemId/>
   <ErrorCode/>
   <ErrorDescription/>
   <IsPartiallyIndexed/>
   <IsPermanentFailure/>
   <SortValue/>
   <AttemptCount/>
   <LastAttemptTime/>
   <AdditionalInfo/>
</NonIndexableItemDetail>
```

 <span data-ttu-id="702f7-105">**NonIndexableItemDetailType**</span><span class="sxs-lookup"><span data-stu-id="702f7-105">**NonIndexableItemDetailType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="702f7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="702f7-106">Attributes and elements</span></span>

<span data-ttu-id="702f7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="702f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="702f7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="702f7-108">Attributes</span></span>

<span data-ttu-id="702f7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="702f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="702f7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="702f7-110">Child elements</span></span>

<span data-ttu-id="702f7-111">[ItemId](itemid.md) | [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount ](attemptcount.md)  |  [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="702f7-111">[ItemId](itemid.md) | [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount](attemptcount.md) | [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="702f7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="702f7-112">Parent elements</span></span>

[<span data-ttu-id="702f7-113">Éléments (ArrayOfNonIndexableItemDetailsType)</span><span class="sxs-lookup"><span data-stu-id="702f7-113">Items (ArrayOfNonIndexableItemDetailsType)</span></span>](items-arrayofnonindexableitemdetailstype.md)
  
## <a name="remarks"></a><span data-ttu-id="702f7-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="702f7-114">Remarks</span></span>

<span data-ttu-id="702f7-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="702f7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="702f7-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="702f7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="702f7-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="702f7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="702f7-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="702f7-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="702f7-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="702f7-119">Schema name</span></span>  <br/> |<span data-ttu-id="702f7-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="702f7-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="702f7-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="702f7-121">Validation file</span></span>  <br/> |<span data-ttu-id="702f7-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="702f7-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="702f7-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="702f7-123">Can be empty</span></span>  <br/> ||
   

