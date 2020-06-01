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
description: L’élément GetItem définit une demande pour obtenir un élément à partir d’une boîte aux lettres dans la Banque d’Exchange.
ms.openlocfilehash: a02403ee84195a41387d5dbe1785ae6d12b47da5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458697"
---
# <a name="getitem"></a><span data-ttu-id="22a67-103">GetItem</span><span class="sxs-lookup"><span data-stu-id="22a67-103">GetItem</span></span>

<span data-ttu-id="22a67-104">L’élément **GetItem** définit une demande pour obtenir un élément à partir d’une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="22a67-104">The **GetItem** element defines a request to get an item from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetItem>
   <ItemShape/>
   <ItemIds/>
</GetItem>
```

 <span data-ttu-id="22a67-105">**GetItemType**</span><span class="sxs-lookup"><span data-stu-id="22a67-105">**GetItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22a67-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="22a67-106">Attributes and elements</span></span>

<span data-ttu-id="22a67-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="22a67-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22a67-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="22a67-108">Attributes</span></span>

<span data-ttu-id="22a67-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="22a67-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22a67-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="22a67-110">Child elements</span></span>

|<span data-ttu-id="22a67-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22a67-111">**Element**</span></span>|<span data-ttu-id="22a67-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="22a67-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22a67-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="22a67-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="22a67-114">Identifie les propriétés et le contenu de l’élément à inclure dans une réponse **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="22a67-114">Identifies the item properties and content to include in a **GetItem** response.</span></span>  <br/> |
|[<span data-ttu-id="22a67-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="22a67-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="22a67-116">Contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques qui sont utilisés pour obtenir des éléments de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="22a67-116">Contains the unique identities of items, occurrence items, and recurring master items that are used to get items from the Exchange store.</span></span> <span data-ttu-id="22a67-117">Ces éléments représentent des contacts, des tâches, des messages, des éléments de calendrier, des demandes de réunion et d’autres éléments valides dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="22a67-117">These items represent contacts, tasks, messages, calendar items, meeting requests, and other valid items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22a67-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="22a67-118">Parent elements</span></span>

<span data-ttu-id="22a67-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="22a67-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="22a67-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="22a67-120">Remarks</span></span>

<span data-ttu-id="22a67-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="22a67-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22a67-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="22a67-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22a67-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="22a67-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="22a67-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="22a67-124">Schema Name</span></span>  <br/> |<span data-ttu-id="22a67-125">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="22a67-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="22a67-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="22a67-126">Validation File</span></span>  <br/> |<span data-ttu-id="22a67-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="22a67-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="22a67-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="22a67-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="22a67-129">False</span><span class="sxs-lookup"><span data-stu-id="22a67-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22a67-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="22a67-130">See also</span></span>



[<span data-ttu-id="22a67-131">Opération GetItem</span><span class="sxs-lookup"><span data-stu-id="22a67-131">GetItem operation</span></span>](getitem-operation.md)

