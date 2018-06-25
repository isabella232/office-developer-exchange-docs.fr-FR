---
title: ErrorCode (int)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65537d96-edf9-41ee-9ad5-91ffe37e2269
description: L’élément ErrorCode Spécifie le code d’erreur d’un échec de la recherche effectué sur une boîte aux lettres.
ms.openlocfilehash: ed8a7771376f921303ea093f4be727c4146faa76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756203"
---
# <a name="errorcode-int"></a><span data-ttu-id="9bf55-103">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="9bf55-103">ErrorCode (int)</span></span>

<span data-ttu-id="9bf55-104">L’élément **ErrorCode** Spécifie le code d’erreur d’un échec de la recherche effectué sur une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9bf55-104">The **ErrorCode** element specifies the error code of a failed search performed against a mailbox.</span></span> 
  
```XML
<ErrorCode></ErrorCode>
```

 <span data-ttu-id="9bf55-105">**int**</span><span class="sxs-lookup"><span data-stu-id="9bf55-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9bf55-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9bf55-106">Attributes and elements</span></span>

<span data-ttu-id="9bf55-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9bf55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9bf55-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9bf55-108">Attributes</span></span>

<span data-ttu-id="9bf55-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9bf55-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9bf55-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9bf55-110">Child elements</span></span>

<span data-ttu-id="9bf55-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9bf55-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9bf55-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9bf55-112">Parent elements</span></span>

|<span data-ttu-id="9bf55-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9bf55-113">**Element**</span></span>|<span data-ttu-id="9bf55-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9bf55-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9bf55-115">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="9bf55-115">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="9bf55-116">Spécifie l’état de conservation de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9bf55-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9bf55-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9bf55-117">Text value</span></span>

<span data-ttu-id="9bf55-118">La valeur de texte de l’élément de **code d’erreur** est le code d’erreur renvoyé pour un échec de la recherche effectué sur une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9bf55-118">The text value of the **ErrorCode** element is the error code returned for a failed search performed against a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9bf55-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="9bf55-119">Remarks</span></span>

<span data-ttu-id="9bf55-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9bf55-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9bf55-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9bf55-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9bf55-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9bf55-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9bf55-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9bf55-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9bf55-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9bf55-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9bf55-125">Schéma type</span><span class="sxs-lookup"><span data-stu-id="9bf55-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="9bf55-126">Validation File</span><span class="sxs-lookup"><span data-stu-id="9bf55-126">Validation File</span></span>  <br/> |<span data-ttu-id="9bf55-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="9bf55-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9bf55-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9bf55-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9bf55-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9bf55-129">See also</span></span>



- [<span data-ttu-id="9bf55-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9bf55-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

