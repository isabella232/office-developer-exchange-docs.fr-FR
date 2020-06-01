---
title: IsReadReceipt
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReadReceipt
api_type:
- schema
ms.assetid: e60e525f-c136-469a-b68b-b3dc01f400a6
description: L’élément IsReadReceipt indique si les messages entrants doivent être des accusés de lecture afin que la condition ou l’exception s’applique.
ms.openlocfilehash: e86a7776bc43204dae9fc92f21d4304255ddb888
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463901"
---
# <a name="isreadreceipt"></a><span data-ttu-id="6e8c2-103">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="6e8c2-103">IsReadReceipt</span></span>

<span data-ttu-id="6e8c2-104">L’élément **IsReadReceipt** indique si les messages entrants doivent être des accusés de lecture afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="6e8c2-104">The **IsReadReceipt** element indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span> 
  
```XML
<IsReadReceipt> true | false</IsReadReceipt>
```

 <span data-ttu-id="6e8c2-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6e8c2-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e8c2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6e8c2-106">Attributes and elements</span></span>

<span data-ttu-id="6e8c2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6e8c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e8c2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6e8c2-108">Attributes</span></span>

<span data-ttu-id="6e8c2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6e8c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e8c2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6e8c2-110">Child elements</span></span>

<span data-ttu-id="6e8c2-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6e8c2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6e8c2-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6e8c2-112">Parent elements</span></span>

|<span data-ttu-id="6e8c2-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6e8c2-113">**Element**</span></span>|<span data-ttu-id="6e8c2-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="6e8c2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e8c2-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="6e8c2-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="6e8c2-116">Représente les conditions qui, une fois traité, déclenche les actions de règle associée à cette règle.</span><span class="sxs-lookup"><span data-stu-id="6e8c2-116">Represents the conditions that, when fulfilled, will trigger the rule actions for that rule.</span></span>  <br/> |
|[<span data-ttu-id="6e8c2-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="6e8c2-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="6e8c2-118">Représente toutes les conditions d'exception de règle disponibles pour la règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="6e8c2-118">Represents all the available rule exception conditions for the Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e8c2-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="6e8c2-119">Text value</span></span>

<span data-ttu-id="6e8c2-120">Une valeur de texte **true** indique que le message doit être une confirmation de lecture pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="6e8c2-120">A text value of **true** indicates that the message must be a read receipt in order for the condition or exception to apply.</span></span> <span data-ttu-id="6e8c2-121">Si le message ne doit pas être une confirmation de lecture pour la condition ou l’exception à appliquer, la valeur est **false**.</span><span class="sxs-lookup"><span data-stu-id="6e8c2-121">If the message does not have to be a read receipt for the condition or exception to apply, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e8c2-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="6e8c2-122">Remarks</span></span>

<span data-ttu-id="6e8c2-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e8c2-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e8c2-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6e8c2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e8c2-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6e8c2-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6e8c2-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6e8c2-126">Schema Name</span></span>  <br/> |<span data-ttu-id="6e8c2-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6e8c2-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6e8c2-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6e8c2-128">Validation File</span></span>  <br/> |<span data-ttu-id="6e8c2-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6e8c2-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e8c2-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6e8c2-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e8c2-131">True</span><span class="sxs-lookup"><span data-stu-id="6e8c2-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e8c2-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6e8c2-132">See also</span></span>



- [<span data-ttu-id="6e8c2-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6e8c2-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

