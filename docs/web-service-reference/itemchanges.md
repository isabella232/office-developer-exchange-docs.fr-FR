---
title: ItemChanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChanges
api_type:
- schema
ms.assetid: cd307892-2f69-4494-8325-219bdb5c3ad5
description: L’élément ItemChanges contient un tableau d’éléments ItemChange qui identifient les éléments et les mises à jour à appliquer aux éléments.
ms.openlocfilehash: 38fe112441a8773a2d6b494ed57c63341cab2b58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828141"
---
# <a name="itemchanges"></a><span data-ttu-id="d5828-103">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="d5828-103">ItemChanges</span></span>

<span data-ttu-id="d5828-104">L’élément **ItemChanges** contient un tableau d’éléments [ItemChange](itemchange.md) qui identifient les éléments et les mises à jour à appliquer aux éléments.</span><span class="sxs-lookup"><span data-stu-id="d5828-104">The **ItemChanges** element contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span> 
  
[<span data-ttu-id="d5828-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="d5828-105">UpdateItem</span></span>](updateitem.md)
  
[<span data-ttu-id="d5828-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="d5828-106">ItemChanges</span></span>](itemchanges.md)
  
```xml
<ItemChanges>
   <ItemChange/>
</ItemChanges>
```

 <span data-ttu-id="d5828-107">**NonEmptyArrayOfItemChangesType**</span><span class="sxs-lookup"><span data-stu-id="d5828-107">**NonEmptyArrayOfItemChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5828-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d5828-108">Attributes and elements</span></span>

<span data-ttu-id="d5828-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d5828-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5828-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d5828-110">Attributes</span></span>

<span data-ttu-id="d5828-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d5828-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5828-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d5828-112">Child elements</span></span>

|<span data-ttu-id="d5828-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d5828-113">**Element**</span></span>|<span data-ttu-id="d5828-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d5828-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5828-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="d5828-115">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="d5828-116">Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.</span><span class="sxs-lookup"><span data-stu-id="d5828-116">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5828-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d5828-117">Parent elements</span></span>

|<span data-ttu-id="d5828-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d5828-118">**Element**</span></span>|<span data-ttu-id="d5828-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="d5828-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5828-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="d5828-120">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="d5828-121">Définit une demande de mise à jour des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d5828-121">Defines a request to update items in a mailbox.</span></span>  <br/> <span data-ttu-id="d5828-122">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="d5828-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d5828-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="d5828-123">Remarks</span></span>

<span data-ttu-id="d5828-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d5828-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5828-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d5828-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5828-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d5828-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d5828-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d5828-127">Schema Name</span></span>  <br/> |<span data-ttu-id="d5828-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d5828-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d5828-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d5828-129">Validation File</span></span>  <br/> |<span data-ttu-id="d5828-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d5828-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d5828-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d5828-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5828-132">False</span><span class="sxs-lookup"><span data-stu-id="d5828-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5828-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d5828-133">See also</span></span>



[<span data-ttu-id="d5828-134">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="d5828-134">UpdateItem operation</span></span>](updateitem-operation.md)

