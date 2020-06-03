---
title: BaseFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseFolderIds
api_type:
- schema
ms.assetid: bdaa6093-f960-469a-b338-0e75aaa536c6
description: L’élément BaseFolderIds représente la collection de dossiers qui seront extraites pour déterminer le contenu d’un dossier de recherche.
ms.openlocfilehash: 97159ec1ded685e63aafedfaf90a06eff39adaab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460266"
---
# <a name="basefolderids"></a><span data-ttu-id="92044-103">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="92044-103">BaseFolderIds</span></span>

<span data-ttu-id="92044-104">L’élément **BaseFolderIds** représente la collection de dossiers qui seront extraites pour déterminer le contenu d’un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="92044-104">The **BaseFolderIds** element represents the collection of folders that will be mined to determine the contents of a search folder.</span></span> 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 <span data-ttu-id="92044-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="92044-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92044-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="92044-106">Attributes and elements</span></span>

<span data-ttu-id="92044-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="92044-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92044-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="92044-108">Attributes</span></span>

<span data-ttu-id="92044-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="92044-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92044-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="92044-110">Child elements</span></span>

|<span data-ttu-id="92044-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="92044-111">**Element**</span></span>|<span data-ttu-id="92044-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="92044-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92044-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="92044-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="92044-114">Contient l’identificateur et la clé de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="92044-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="92044-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="92044-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="92044-116">Identifie les dossiers MicrosoftExchange Server 2007 qui peuvent être référencés par nom.</span><span class="sxs-lookup"><span data-stu-id="92044-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92044-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="92044-117">Parent elements</span></span>

|<span data-ttu-id="92044-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="92044-118">**Element**</span></span>|<span data-ttu-id="92044-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="92044-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92044-120">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="92044-120">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="92044-121">Représente les paramètres qui définissent un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="92044-121">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="92044-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="92044-122">Remarks</span></span>

<span data-ttu-id="92044-123">L’élément **BaseFolderIds** doit contenir au moins un élément [FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="92044-123">The **BaseFolderIds** element must contain at least one [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="92044-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="92044-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92044-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="92044-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92044-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="92044-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92044-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="92044-127">Schema name</span></span>  <br/> |<span data-ttu-id="92044-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="92044-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="92044-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="92044-129">Validation file</span></span>  <br/> |<span data-ttu-id="92044-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="92044-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92044-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="92044-131">Can be empty</span></span>  <br/> |<span data-ttu-id="92044-132">False</span><span class="sxs-lookup"><span data-stu-id="92044-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92044-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="92044-133">See also</span></span>



- [<span data-ttu-id="92044-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="92044-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

