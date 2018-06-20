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
description: L’élément ReadFlagChange est retournée dans SyncFolderItems réponses opération lorsqu’un élément a été lu. Cette propriété est en lecture seule.
ms.openlocfilehash: 28ef0267e8308ba58057bec01ab2672a19ee94a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828953"
---
# <a name="readflagchange"></a><span data-ttu-id="41a26-104">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="41a26-104">ReadFlagChange</span></span>

<span data-ttu-id="41a26-105">L’élément **ReadFlagChange** est renvoyé dans les réponses de [l’opération SyncFolderItems](syncfolderitems-operation.md) lorsqu’un élément a été lu.</span><span class="sxs-lookup"><span data-stu-id="41a26-105">The **ReadFlagChange** element is returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="41a26-106">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="41a26-106">This property is read-only.</span></span> 
  
```xml
<ReadFlagChange>
   <ItemId/>
   <IsRead/>
</ReadFlagChange>
```

 <span data-ttu-id="41a26-107">**SyncFolderItemsReadFlagType**</span><span class="sxs-lookup"><span data-stu-id="41a26-107">**SyncFolderItemsReadFlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41a26-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="41a26-108">Attributes and elements</span></span>

<span data-ttu-id="41a26-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="41a26-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41a26-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="41a26-110">Attributes</span></span>

<span data-ttu-id="41a26-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="41a26-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41a26-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="41a26-112">Child elements</span></span>

|<span data-ttu-id="41a26-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="41a26-113">**Element**</span></span>|<span data-ttu-id="41a26-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="41a26-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41a26-115">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="41a26-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="41a26-116">Identifie l’élément pour lequel l’indicateur de lecture a été modifié.</span><span class="sxs-lookup"><span data-stu-id="41a26-116">Identifies the item for which the read-flag has been changed.</span></span>  <br/> |
|[<span data-ttu-id="41a26-117">Estlu</span><span class="sxs-lookup"><span data-stu-id="41a26-117">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="41a26-118">Indique si l’indicateur de lecture a été définie sur **true**.</span><span class="sxs-lookup"><span data-stu-id="41a26-118">Indicates whether the read-flag has been set to **true**.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="41a26-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="41a26-119">Parent elements</span></span>

|<span data-ttu-id="41a26-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="41a26-120">**Element**</span></span>|<span data-ttu-id="41a26-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="41a26-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41a26-122">Modifications (éléments)</span><span class="sxs-lookup"><span data-stu-id="41a26-122">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="41a26-123">Contient un tableau de séquence de types de modification qui représentent les types de différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="41a26-123">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="41a26-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="41a26-124">Remarks</span></span>

<span data-ttu-id="41a26-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="41a26-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41a26-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="41a26-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41a26-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="41a26-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41a26-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="41a26-128">Schema Name</span></span>  <br/> |<span data-ttu-id="41a26-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="41a26-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="41a26-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="41a26-130">Validation File</span></span>  <br/> |<span data-ttu-id="41a26-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="41a26-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="41a26-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="41a26-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="41a26-133">False</span><span class="sxs-lookup"><span data-stu-id="41a26-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41a26-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="41a26-134">See also</span></span>



- [<span data-ttu-id="41a26-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="41a26-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

