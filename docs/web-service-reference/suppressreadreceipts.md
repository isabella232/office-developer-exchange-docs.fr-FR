---
title: SuppressReadReceipts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: L’élément SuppressReadReceipts indique si les confirmations de lecture doivent être supprimées.
ms.openlocfilehash: aa604d4907582bd73727ba664958a589a222f9cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455932"
---
# <a name="suppressreadreceipts"></a><span data-ttu-id="ffbe4-103">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="ffbe4-103">SuppressReadReceipts</span></span>

<span data-ttu-id="ffbe4-104">L’élément **SuppressReadReceipts** indique si les confirmations de lecture doivent être supprimées.</span><span class="sxs-lookup"><span data-stu-id="ffbe4-104">The **SuppressReadReceipts** element indicates whether read receipts should be suppressed.</span></span> 
  
```XML
<SuppressReadReceipts>true | false</SuppressReadReceipts>
```

 <span data-ttu-id="ffbe4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ffbe4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffbe4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ffbe4-106">Attributes and elements</span></span>

<span data-ttu-id="ffbe4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ffbe4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffbe4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ffbe4-108">Attributes</span></span>

<span data-ttu-id="ffbe4-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ffbe4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffbe4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ffbe4-110">Child elements</span></span>

<span data-ttu-id="ffbe4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ffbe4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ffbe4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ffbe4-112">Parent elements</span></span>

<span data-ttu-id="ffbe4-113">[ConversationAction](conversationaction.md)  |  [MarkAllItemsAsRead](markallitemsasread.md)</span><span class="sxs-lookup"><span data-stu-id="ffbe4-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ffbe4-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ffbe4-114">Text value</span></span>

<span data-ttu-id="ffbe4-115">Une valeur de texte de **true** pour l’élément **SuppressReadReciepts** indique que les confirmations de lecture sont supprimées.</span><span class="sxs-lookup"><span data-stu-id="ffbe4-115">A text value of **true** for the **SuppressReadReciepts** element indicates that read receipts are suppressed.</span></span> <span data-ttu-id="ffbe4-116">La valeur **false** indique que les confirmations de lecture seront envoyées à l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="ffbe4-116">A value of **false** indicates that read receipts will be sent to the sender.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ffbe4-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="ffbe4-117">Remarks</span></span>

<span data-ttu-id="ffbe4-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ffbe4-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ffbe4-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffbe4-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffbe4-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ffbe4-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffbe4-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ffbe4-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ffbe4-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ffbe4-122">Schema name</span></span>  <br/> |<span data-ttu-id="ffbe4-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ffbe4-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ffbe4-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ffbe4-124">Validation file</span></span>  <br/> |<span data-ttu-id="ffbe4-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ffbe4-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ffbe4-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ffbe4-126">Can be empty</span></span>  <br/> ||
   

