---
title: GlobalParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f5fcbcb-05ed-462a-99cf-a6b112a4aef6
description: L’élément GlobalParentFolderIds spécifie les identificateurs des dossiers parents globale.
ms.openlocfilehash: b0ff9ab00f3e46351b5a2db9bc4b6282fa4385cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827747"
---
# <a name="globalparentfolderids"></a><span data-ttu-id="5593e-103">GlobalParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="5593e-103">GlobalParentFolderIds</span></span>

<span data-ttu-id="5593e-104">L’élément **GlobalParentFolderIds** spécifie les identificateurs des dossiers parents globale.</span><span class="sxs-lookup"><span data-stu-id="5593e-104">The **GlobalParentFolderIds** element specifies the identifiers of the global parent folders.</span></span> 
  
```XML
<GlobalParentFolderIds>
    <FolderId/>
    <DistinguishedFolderId/>
</GlobalParentFolderIds>
```

 <span data-ttu-id="5593e-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="5593e-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5593e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5593e-106">Attributes and elements</span></span>

<span data-ttu-id="5593e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5593e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5593e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5593e-108">Attributes</span></span>

<span data-ttu-id="5593e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5593e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5593e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5593e-110">Child elements</span></span>

|<span data-ttu-id="5593e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5593e-111">**Element**</span></span>|<span data-ttu-id="5593e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="5593e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5593e-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="5593e-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="5593e-114">Contient la clé d’identificateur et de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="5593e-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="5593e-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="5593e-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="5593e-116">Identifie les dossiers qui peuvent être référencés par un nom.</span><span class="sxs-lookup"><span data-stu-id="5593e-116">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5593e-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5593e-117">Parent elements</span></span>

|<span data-ttu-id="5593e-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5593e-118">**Element**</span></span>|<span data-ttu-id="5593e-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="5593e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5593e-120">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="5593e-120">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="5593e-121">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="5593e-121">Represents a single conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5593e-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="5593e-122">Remarks</span></span>

<span data-ttu-id="5593e-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5593e-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5593e-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5593e-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5593e-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5593e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5593e-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5593e-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5593e-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5593e-127">Schema Name</span></span>  <br/> |<span data-ttu-id="5593e-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="5593e-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="5593e-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="5593e-129">Validation File</span></span>  <br/> |<span data-ttu-id="5593e-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="5593e-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5593e-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5593e-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5593e-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5593e-132">See also</span></span>



- [<span data-ttu-id="5593e-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5593e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

