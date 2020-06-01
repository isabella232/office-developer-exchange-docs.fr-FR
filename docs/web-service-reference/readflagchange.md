---
title: ReadFlagChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadFlagChange
api_type:
- schema
ms.assetid: 527bfe90-63d0-4b2f-97f7-7875b3a516b2
description: L’élément ReadFlagChange est renvoyé dans les réponses à une opération SyncFolderItems lorsqu’un élément a été lu. Cette propriété est en lecture seule.
ms.openlocfilehash: 354f8085a6ea5b738d8619e2ffeb0fbccefd51da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468305"
---
# <a name="readflagchange"></a><span data-ttu-id="03b92-104">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="03b92-104">ReadFlagChange</span></span>

<span data-ttu-id="03b92-105">L’élément **ReadFlagChange** est renvoyé dans les réponses à une [opération SyncFolderItems](syncfolderitems-operation.md) lorsqu’un élément a été lu.</span><span class="sxs-lookup"><span data-stu-id="03b92-105">The **ReadFlagChange** element is returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="03b92-106">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="03b92-106">This property is read-only.</span></span> 
  
```xml
<ReadFlagChange>
   <ItemId/>
   <IsRead/>
</ReadFlagChange>
```

 <span data-ttu-id="03b92-107">**SyncFolderItemsReadFlagType**</span><span class="sxs-lookup"><span data-stu-id="03b92-107">**SyncFolderItemsReadFlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03b92-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="03b92-108">Attributes and elements</span></span>

<span data-ttu-id="03b92-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="03b92-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03b92-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="03b92-110">Attributes</span></span>

<span data-ttu-id="03b92-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="03b92-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03b92-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="03b92-112">Child elements</span></span>

|<span data-ttu-id="03b92-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="03b92-113">**Element**</span></span>|<span data-ttu-id="03b92-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="03b92-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03b92-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="03b92-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="03b92-116">Identifie l’élément pour lequel l’indicateur de lecture a été modifié.</span><span class="sxs-lookup"><span data-stu-id="03b92-116">Identifies the item for which the read-flag has been changed.</span></span>  <br/> |
|[<span data-ttu-id="03b92-117">IsRead</span><span class="sxs-lookup"><span data-stu-id="03b92-117">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="03b92-118">Indique si l’indicateur de lecture a été défini sur **true**.</span><span class="sxs-lookup"><span data-stu-id="03b92-118">Indicates whether the read-flag has been set to **true**.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="03b92-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="03b92-119">Parent elements</span></span>

|<span data-ttu-id="03b92-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="03b92-120">**Element**</span></span>|<span data-ttu-id="03b92-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="03b92-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03b92-122">Changes (éléments)</span><span class="sxs-lookup"><span data-stu-id="03b92-122">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="03b92-123">Contient un tableau de séquence de types de modifications qui représentent les types de différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="03b92-123">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="03b92-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="03b92-124">Remarks</span></span>

<span data-ttu-id="03b92-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="03b92-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03b92-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="03b92-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03b92-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="03b92-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="03b92-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="03b92-128">Schema Name</span></span>  <br/> |<span data-ttu-id="03b92-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="03b92-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="03b92-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="03b92-130">Validation File</span></span>  <br/> |<span data-ttu-id="03b92-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="03b92-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="03b92-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="03b92-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="03b92-133">False</span><span class="sxs-lookup"><span data-stu-id="03b92-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03b92-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="03b92-134">See also</span></span>



- [<span data-ttu-id="03b92-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="03b92-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

