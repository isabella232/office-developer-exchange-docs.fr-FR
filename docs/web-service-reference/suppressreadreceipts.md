---
title: SuppressReadReceipts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: L’élément indique si des confirmations de lecture de SuppressReadReceipts doit être supprimée.
ms.openlocfilehash: 794252da6b3e6b6e6f36181c1811a2a001bfaf53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838654"
---
# <a name="suppressreadreceipts"></a><span data-ttu-id="26a41-103">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="26a41-103">SuppressReadReceipts</span></span>

<span data-ttu-id="26a41-104">L’élément **SuppressReadReceipts** indique si lire réceptions doivent être supprimées.</span><span class="sxs-lookup"><span data-stu-id="26a41-104">The **SuppressReadReceipts** element indicates whether read receipts should be suppressed.</span></span> 
  
```XML
<SuppressReadReceipts>true | false</SuppressReadReceipts>
```

 <span data-ttu-id="26a41-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="26a41-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26a41-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="26a41-106">Attributes and elements</span></span>

<span data-ttu-id="26a41-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="26a41-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26a41-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="26a41-108">Attributes</span></span>

<span data-ttu-id="26a41-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="26a41-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26a41-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="26a41-110">Child elements</span></span>

<span data-ttu-id="26a41-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="26a41-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26a41-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="26a41-112">Parent elements</span></span>

<span data-ttu-id="26a41-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span><span class="sxs-lookup"><span data-stu-id="26a41-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="26a41-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="26a41-114">Text value</span></span>

<span data-ttu-id="26a41-115">Une valeur de texte de **la valeur true** pour l’élément **SuppressReadReciepts** indique read reçus sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="26a41-115">A text value of **true** for the **SuppressReadReciepts** element indicates that read receipts are suppressed.</span></span> <span data-ttu-id="26a41-116">La valeur **false** indique read encaissements seront envoyés à l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="26a41-116">A value of **false** indicates that read receipts will be sent to the sender.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="26a41-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="26a41-117">Remarks</span></span>

<span data-ttu-id="26a41-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="26a41-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="26a41-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="26a41-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26a41-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="26a41-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26a41-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="26a41-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26a41-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="26a41-122">Schema name</span></span>  <br/> |<span data-ttu-id="26a41-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="26a41-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="26a41-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="26a41-124">Validation file</span></span>  <br/> |<span data-ttu-id="26a41-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="26a41-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26a41-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="26a41-126">Can be empty</span></span>  <br/> ||
   

