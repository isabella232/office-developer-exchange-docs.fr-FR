---
title: GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 769df8eb-9c72-48b5-a49f-82c6b86bc5fc
description: L’élément GetItem définit une demande pour obtenir un élément à partir d’une boîte aux lettres dans la banque d’informations Exchange.
ms.openlocfilehash: 39db141bad62c34bec5ae6a937ba94c2d1288090
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756664"
---
# <a name="getitem"></a><span data-ttu-id="81a18-103">GetItem</span><span class="sxs-lookup"><span data-stu-id="81a18-103">GetItem</span></span>

<span data-ttu-id="81a18-104">L’élément **GetItem** définit une demande pour obtenir un élément à partir d’une boîte aux lettres dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="81a18-104">The **GetItem** element defines a request to get an item from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetItem>
   <ItemShape/>
   <ItemIds/>
</GetItem>
```

 <span data-ttu-id="81a18-105">**GetItemType**</span><span class="sxs-lookup"><span data-stu-id="81a18-105">**GetItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81a18-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="81a18-106">Attributes and elements</span></span>

<span data-ttu-id="81a18-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="81a18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81a18-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="81a18-108">Attributes</span></span>

<span data-ttu-id="81a18-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="81a18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81a18-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="81a18-110">Child elements</span></span>

|<span data-ttu-id="81a18-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="81a18-111">**Element**</span></span>|<span data-ttu-id="81a18-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="81a18-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81a18-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="81a18-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="81a18-114">Identifie les propriétés de l’élément et le contenu à inclure dans une réponse **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="81a18-114">Identifies the item properties and content to include in a **GetItem** response.</span></span>  <br/> |
|[<span data-ttu-id="81a18-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="81a18-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="81a18-116">Contient l’identité unique des éléments, des éléments d’occurrence et éléments périodiques maîtres qui permettent d’obtenir des éléments de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="81a18-116">Contains the unique identities of items, occurrence items, and recurring master items that are used to get items from the Exchange store.</span></span> <span data-ttu-id="81a18-117">Ces éléments représentent des contacts, tâches, messages, éléments de calendrier, les demandes de réunion et autres éléments dans une boîte aux lettres valides.</span><span class="sxs-lookup"><span data-stu-id="81a18-117">These items represent contacts, tasks, messages, calendar items, meeting requests, and other valid items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="81a18-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="81a18-118">Parent elements</span></span>

<span data-ttu-id="81a18-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="81a18-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="81a18-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="81a18-120">Remarks</span></span>

<span data-ttu-id="81a18-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="81a18-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81a18-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="81a18-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81a18-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="81a18-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="81a18-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="81a18-124">Schema Name</span></span>  <br/> |<span data-ttu-id="81a18-125">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="81a18-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="81a18-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="81a18-126">Validation File</span></span>  <br/> |<span data-ttu-id="81a18-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="81a18-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="81a18-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="81a18-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="81a18-129">False</span><span class="sxs-lookup"><span data-stu-id="81a18-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81a18-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="81a18-130">See also</span></span>



[<span data-ttu-id="81a18-131">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="81a18-131">GetItem operation</span></span>](getitem-operation.md)

