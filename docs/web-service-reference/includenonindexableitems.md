---
title: IncludeNonIndexableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af7f202b-2889-447e-bdeb-aaad18ce6b46
description: L’élément IncludeNonIndexableItems contient une valeur booléenne indiquant s’il faut inclure des éléments qui ne peuvent pas être indexés.
ms.openlocfilehash: eab559e938f0b949d79626ae5bf61b3d4a838924
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460623"
---
# <a name="includenonindexableitems"></a><span data-ttu-id="d632a-103">IncludeNonIndexableItems</span><span class="sxs-lookup"><span data-stu-id="d632a-103">IncludeNonIndexableItems</span></span>

<span data-ttu-id="d632a-104">L’élément **IncludeNonIndexableItems** contient une valeur **booléenne** indiquant s’il faut inclure des éléments qui ne peuvent pas être indexés.</span><span class="sxs-lookup"><span data-stu-id="d632a-104">The **IncludeNonIndexableItems** element contains a **Boolean** value to indicate whether to include items that cannot be indexed.</span></span> 
  
```XML
<IncludeNonIndexableItems>true | false</IncludeNonIndexableItems>
```

 <span data-ttu-id="d632a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d632a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d632a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d632a-106">Attributes and elements</span></span>

<span data-ttu-id="d632a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d632a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d632a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d632a-108">Attributes</span></span>

<span data-ttu-id="d632a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d632a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d632a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d632a-110">Child elements</span></span>

<span data-ttu-id="d632a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d632a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d632a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d632a-112">Parent elements</span></span>

[<span data-ttu-id="d632a-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="d632a-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="d632a-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="d632a-114">Text value</span></span>

<span data-ttu-id="d632a-115">Une valeur de texte de **true** pour l’élément **IncludeNonIndexableItems** indique que les éléments qui ne peuvent pas être indexés sont inclus dans les conservations des boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d632a-115">A text value of **true** for the **IncludeNonIndexableItems** element indicates that items that cannot be indexed are included with mailbox holds.</span></span> <span data-ttu-id="d632a-116">La valeur **false** indique que les éléments qui ne peuvent pas être indexés ne sont pas inclus dans les conservations des boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d632a-116">A value of **false** indicates that the items that cannot be indexed are not included in mailbox holds.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d632a-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="d632a-117">Remarks</span></span>

<span data-ttu-id="d632a-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d632a-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d632a-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d632a-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d632a-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d632a-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d632a-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d632a-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d632a-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d632a-122">Schema name</span></span>  <br/> |<span data-ttu-id="d632a-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d632a-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d632a-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d632a-124">Validation file</span></span>  <br/> |<span data-ttu-id="d632a-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d632a-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d632a-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d632a-126">Can be empty</span></span>  <br/> |<span data-ttu-id="d632a-127">false</span><span class="sxs-lookup"><span data-stu-id="d632a-127">false</span></span>  <br/> |
   

