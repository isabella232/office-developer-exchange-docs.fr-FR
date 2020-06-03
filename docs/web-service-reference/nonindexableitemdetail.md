---
title: NonIndexableItemDetail
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a26d4c02-f1bd-40c4-9257-5db45e839f17
description: L’élément NonIndexableItemDetail spécifie des informations détaillées sur un élément qui ne peuvent pas être indexées.
ms.openlocfilehash: 4fc4324501570402d22aa303d6af2a60b50b3cc6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466737"
---
# <a name="nonindexableitemdetail"></a><span data-ttu-id="ab801-103">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="ab801-103">NonIndexableItemDetail</span></span>

<span data-ttu-id="ab801-104">L’élément **NonIndexableItemDetail** spécifie des informations détaillées sur un élément qui ne peuvent pas être indexées.</span><span class="sxs-lookup"><span data-stu-id="ab801-104">The **NonIndexableItemDetail** element specifies detail information about an item that cannot be indexed.</span></span> 
  
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

 <span data-ttu-id="ab801-105">**NonIndexableItemDetailType**</span><span class="sxs-lookup"><span data-stu-id="ab801-105">**NonIndexableItemDetailType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ab801-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ab801-106">Attributes and elements</span></span>

<span data-ttu-id="ab801-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ab801-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ab801-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ab801-108">Attributes</span></span>

<span data-ttu-id="ab801-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ab801-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ab801-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ab801-110">Child elements</span></span>

<span data-ttu-id="ab801-111">[ItemId](itemid.md)  |  [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md)  |  [ErrorDescription](errordescription.md)  |  [IsPartiallyIndexed](ispartiallyindexed.md)  |  [IsPermanentFailure](ispermanentfailure.md)  |  [SortValue](sortvalue.md)  |  [AttemptCount](attemptcount.md)  |  [LastAttemptTime](lastattempttime.md)  |  [AdditionalInfo](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="ab801-111">[ItemId](itemid.md) | [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount](attemptcount.md) | [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ab801-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ab801-112">Parent elements</span></span>

[<span data-ttu-id="ab801-113">Items (ArrayOfNonIndexableItemDetailsType)</span><span class="sxs-lookup"><span data-stu-id="ab801-113">Items (ArrayOfNonIndexableItemDetailsType)</span></span>](items-arrayofnonindexableitemdetailstype.md)
  
## <a name="remarks"></a><span data-ttu-id="ab801-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="ab801-114">Remarks</span></span>

<span data-ttu-id="ab801-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ab801-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ab801-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab801-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ab801-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ab801-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ab801-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ab801-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ab801-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ab801-119">Schema name</span></span>  <br/> |<span data-ttu-id="ab801-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ab801-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="ab801-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ab801-121">Validation file</span></span>  <br/> |<span data-ttu-id="ab801-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ab801-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ab801-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ab801-123">Can be empty</span></span>  <br/> ||
   

