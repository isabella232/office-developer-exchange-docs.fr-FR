---
title: SearchParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchParameters
api_type:
- schema
ms.assetid: 34602cb1-dc33-4552-a98c-3e77f614daa3
description: L’élément SearchParameters représente les paramètres qui définissent un dossier de recherche.
ms.openlocfilehash: cd9f255621b17d01113392e67a0301b01b70f326
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466667"
---
# <a name="searchparameters"></a><span data-ttu-id="80a74-103">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="80a74-103">SearchParameters</span></span>

<span data-ttu-id="80a74-104">L’élément **SearchParameters** représente les paramètres qui définissent un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="80a74-104">The **SearchParameters** element represents the parameters that define a search folder.</span></span> 
  
```xml
<SearchParameters Traversal="">
   <Restriction/>
   <BaseFolderIds/>
</SearchParameters>
```

 <span data-ttu-id="80a74-105">**SearchParametersType**</span><span class="sxs-lookup"><span data-stu-id="80a74-105">**SearchParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80a74-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="80a74-106">Attributes and elements</span></span>

<span data-ttu-id="80a74-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="80a74-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80a74-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="80a74-108">Attributes</span></span>

|<span data-ttu-id="80a74-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="80a74-109">**Attribute**</span></span>|<span data-ttu-id="80a74-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="80a74-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="80a74-111">**Traversée**</span><span class="sxs-lookup"><span data-stu-id="80a74-111">**Traversal**</span></span> <br/> |<span data-ttu-id="80a74-112">Décrit comment un dossier de recherche parcourt la hiérarchie de dossiers.</span><span class="sxs-lookup"><span data-stu-id="80a74-112">Describes how a search folder traverses the folder hierarchy.</span></span> <span data-ttu-id="80a74-113">Les options sont pour une recherche **approfondie** ou **superficielle** .</span><span class="sxs-lookup"><span data-stu-id="80a74-113">The options are for either a **Deep** or a **Shallow** search.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="80a74-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="80a74-114">Child elements</span></span>

|<span data-ttu-id="80a74-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="80a74-115">**Element**</span></span>|<span data-ttu-id="80a74-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="80a74-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80a74-117">Restriction</span><span class="sxs-lookup"><span data-stu-id="80a74-117">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="80a74-118">Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="80a74-118">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="80a74-119">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="80a74-119">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="80a74-120">Représente la collection de dossiers qui seront extraites pour déterminer le contenu d’un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="80a74-120">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="80a74-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="80a74-121">Parent elements</span></span>

|<span data-ttu-id="80a74-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="80a74-122">**Element**</span></span>|<span data-ttu-id="80a74-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="80a74-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80a74-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="80a74-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="80a74-125">Représente un dossier de recherche contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="80a74-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="80a74-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="80a74-126">Remarks</span></span>

<span data-ttu-id="80a74-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="80a74-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80a74-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="80a74-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80a74-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="80a74-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80a74-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="80a74-130">Schema Name</span></span>  <br/> |<span data-ttu-id="80a74-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="80a74-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="80a74-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="80a74-132">Validation File</span></span>  <br/> |<span data-ttu-id="80a74-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="80a74-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80a74-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="80a74-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="80a74-135">False</span><span class="sxs-lookup"><span data-stu-id="80a74-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80a74-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="80a74-136">See also</span></span>



- [<span data-ttu-id="80a74-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="80a74-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

