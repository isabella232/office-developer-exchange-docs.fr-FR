---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: L’élément ReturnNewItemIds indique si les identificateurs d’élément de nouveaux éléments sont renvoyés dans la réponse.
ms.openlocfilehash: 003676c4c034454aa551e42bf3af976183117b8c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465113"
---
# <a name="returnnewitemids"></a><span data-ttu-id="315fc-103">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="315fc-103">ReturnNewItemIds</span></span>

<span data-ttu-id="315fc-104">L’élément **ReturnNewItemIds** indique si les identificateurs d’élément de nouveaux éléments sont renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="315fc-104">The **ReturnNewItemIds** element indicates whether the item identifiers of new items are returned in the response.</span></span> 
  
```XML
<ReturnNewItemIds/>
```

 <span data-ttu-id="315fc-105">**XS : Boolean**</span><span class="sxs-lookup"><span data-stu-id="315fc-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="315fc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="315fc-106">Attributes and elements</span></span>

<span data-ttu-id="315fc-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="315fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="315fc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="315fc-108">Attributes</span></span>

<span data-ttu-id="315fc-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="315fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="315fc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="315fc-110">Child elements</span></span>

<span data-ttu-id="315fc-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="315fc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="315fc-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="315fc-112">Parent elements</span></span>

|<span data-ttu-id="315fc-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="315fc-113">**Element**</span></span>|<span data-ttu-id="315fc-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="315fc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="315fc-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="315fc-115">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="315fc-116">Définit une demande de copie d’un élément dans une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="315fc-116">Defines a request to copy an item in a mailbox in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="315fc-117">MoveItem</span><span class="sxs-lookup"><span data-stu-id="315fc-117">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="315fc-118">Définit une demande de déplacement d’un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="315fc-118">Defines a request to move an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="315fc-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="315fc-119">Text value</span></span>

<span data-ttu-id="315fc-120">Une valeur de texte de **true** pour l’élément **ReturnNewItemIds** indique que les nouveaux identificateurs d’élément sont renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="315fc-120">A text value of **true** for the **ReturnNewItemIds** element indicates that the new item identifiers are returned in the response.</span></span> <span data-ttu-id="315fc-121">La valeur **false** indique que les nouveaux identificateurs d’élément ne sont pas renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="315fc-121">A value of **false** indicates that the new item identifiers are not returned in the response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="315fc-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="315fc-122">Remarks</span></span>

<span data-ttu-id="315fc-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="315fc-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="315fc-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="315fc-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="315fc-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="315fc-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="315fc-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="315fc-126">Schema Name</span></span>  <br/> |<span data-ttu-id="315fc-127">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="315fc-127">Message schema</span></span>  <br/> |
|<span data-ttu-id="315fc-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="315fc-128">Validation File</span></span>  <br/> |<span data-ttu-id="315fc-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="315fc-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="315fc-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="315fc-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="315fc-131">False</span><span class="sxs-lookup"><span data-stu-id="315fc-131">False</span></span>  <br/> |
   

