---
title: GlobalParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f5fcbcb-05ed-462a-99cf-a6b112a4aef6
description: L’élément GlobalParentFolderIds spécifie les identificateurs des dossiers parents globaux.
ms.openlocfilehash: 11c520fa0f4a1ed6d6c9d694b407e39cd036b9cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459096"
---
# <a name="globalparentfolderids"></a><span data-ttu-id="54f42-103">GlobalParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="54f42-103">GlobalParentFolderIds</span></span>

<span data-ttu-id="54f42-104">L’élément **GlobalParentFolderIds** spécifie les identificateurs des dossiers parents globaux.</span><span class="sxs-lookup"><span data-stu-id="54f42-104">The **GlobalParentFolderIds** element specifies the identifiers of the global parent folders.</span></span> 
  
```XML
<GlobalParentFolderIds>
    <FolderId/>
    <DistinguishedFolderId/>
</GlobalParentFolderIds>
```

 <span data-ttu-id="54f42-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="54f42-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54f42-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="54f42-106">Attributes and elements</span></span>

<span data-ttu-id="54f42-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="54f42-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54f42-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="54f42-108">Attributes</span></span>

<span data-ttu-id="54f42-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="54f42-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54f42-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="54f42-110">Child elements</span></span>

|<span data-ttu-id="54f42-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="54f42-111">**Element**</span></span>|<span data-ttu-id="54f42-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="54f42-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54f42-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="54f42-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="54f42-114">Contient l’identificateur et la clé de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="54f42-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="54f42-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="54f42-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="54f42-116">Identifie les dossiers qui peuvent être référencés par leur nom.</span><span class="sxs-lookup"><span data-stu-id="54f42-116">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54f42-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="54f42-117">Parent elements</span></span>

|<span data-ttu-id="54f42-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="54f42-118">**Element**</span></span>|<span data-ttu-id="54f42-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="54f42-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54f42-120">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="54f42-120">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="54f42-121">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="54f42-121">Represents a single conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="54f42-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="54f42-122">Remarks</span></span>

<span data-ttu-id="54f42-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="54f42-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="54f42-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="54f42-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54f42-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="54f42-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54f42-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="54f42-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54f42-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="54f42-127">Schema Name</span></span>  <br/> |<span data-ttu-id="54f42-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="54f42-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="54f42-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="54f42-129">Validation File</span></span>  <br/> |<span data-ttu-id="54f42-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="54f42-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="54f42-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="54f42-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="54f42-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="54f42-132">See also</span></span>



- [<span data-ttu-id="54f42-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="54f42-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

