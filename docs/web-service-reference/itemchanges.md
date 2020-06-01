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
description: L’élément ItemChanges contient un tableau d’éléments ItemChange, qui identifient les éléments et les mises à jour à appliquer aux éléments.
ms.openlocfilehash: ea6fb2023b88360f9558057e80c7fe0d855173b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459909"
---
# <a name="itemchanges"></a><span data-ttu-id="24374-103">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="24374-103">ItemChanges</span></span>

<span data-ttu-id="24374-104">L’élément **itemChanges** contient un tableau d’éléments [ItemChange,](itemchange.md) qui identifient les éléments et les mises à jour à appliquer aux éléments.</span><span class="sxs-lookup"><span data-stu-id="24374-104">The **ItemChanges** element contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span> 
  
[<span data-ttu-id="24374-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="24374-105">UpdateItem</span></span>](updateitem.md)
  
[<span data-ttu-id="24374-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="24374-106">ItemChanges</span></span>](itemchanges.md)
  
```xml
<ItemChanges>
   <ItemChange/>
</ItemChanges>
```

 <span data-ttu-id="24374-107">**NonEmptyArrayOfItemChangesType**</span><span class="sxs-lookup"><span data-stu-id="24374-107">**NonEmptyArrayOfItemChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24374-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="24374-108">Attributes and elements</span></span>

<span data-ttu-id="24374-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="24374-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24374-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="24374-110">Attributes</span></span>

<span data-ttu-id="24374-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="24374-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24374-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="24374-112">Child elements</span></span>

|<span data-ttu-id="24374-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="24374-113">**Element**</span></span>|<span data-ttu-id="24374-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="24374-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24374-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="24374-115">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="24374-116">Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.</span><span class="sxs-lookup"><span data-stu-id="24374-116">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24374-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="24374-117">Parent elements</span></span>

|<span data-ttu-id="24374-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="24374-118">**Element**</span></span>|<span data-ttu-id="24374-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="24374-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24374-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="24374-120">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="24374-121">Définit une demande de mise à jour des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="24374-121">Defines a request to update items in a mailbox.</span></span>  <br/> <span data-ttu-id="24374-122">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="24374-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="24374-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="24374-123">Remarks</span></span>

<span data-ttu-id="24374-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="24374-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24374-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="24374-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24374-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="24374-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="24374-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="24374-127">Schema Name</span></span>  <br/> |<span data-ttu-id="24374-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="24374-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="24374-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="24374-129">Validation File</span></span>  <br/> |<span data-ttu-id="24374-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="24374-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="24374-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="24374-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="24374-132">False</span><span class="sxs-lookup"><span data-stu-id="24374-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24374-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="24374-133">See also</span></span>



[<span data-ttu-id="24374-134">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="24374-134">UpdateItem operation</span></span>](updateitem-operation.md)

