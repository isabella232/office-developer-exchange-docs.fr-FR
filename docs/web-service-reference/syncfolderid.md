---
title: SyncFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderId
api_type:
- schema
ms.assetid: 3645fa03-236d-4e5f-b8b9-5d98f7f35fa2
description: L’élément SyncFolderId représente le dossier qui contient les éléments à synchroniser.
ms.openlocfilehash: c90a20095ca4706f0c6edae3e98eaadd6024d817
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354399"
---
# <a name="syncfolderid"></a><span data-ttu-id="c5a18-103">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="c5a18-103">SyncFolderId</span></span>

<span data-ttu-id="c5a18-104">L’élément **SyncFolderId** représente le dossier qui contient les éléments à synchroniser.</span><span class="sxs-lookup"><span data-stu-id="c5a18-104">The **SyncFolderId** element represents the folder that contains the items to synchronize.</span></span> 
  
```xml
<SyncFolderId>
   <FolderId/>
</SyncFolderId>
```

```xml
<SyncFolderId>
   <DistinguishedFolderId/> 
</SyncFolderId>
```

<span data-ttu-id="c5a18-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="c5a18-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c5a18-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c5a18-106">Attributes and elements</span></span>

<span data-ttu-id="c5a18-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c5a18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5a18-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c5a18-108">Attributes</span></span>

<span data-ttu-id="c5a18-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c5a18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5a18-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c5a18-110">Child elements</span></span>

|<span data-ttu-id="c5a18-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c5a18-111">**Element**</span></span>|<span data-ttu-id="c5a18-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c5a18-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5a18-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="c5a18-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="c5a18-114">Contient la clé d’identificateur et de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="c5a18-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="c5a18-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="c5a18-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="c5a18-116">Identifie les dossiers MicrosoftExchange Server 2007 qui peuvent être référencés par son nom.</span><span class="sxs-lookup"><span data-stu-id="c5a18-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5a18-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c5a18-117">Parent elements</span></span>

|<span data-ttu-id="c5a18-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c5a18-118">**Element**</span></span>|<span data-ttu-id="c5a18-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="c5a18-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5a18-120">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="c5a18-120">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="c5a18-121">Définit une demande de synchronisation d’une hiérarchie de dossiers dans une banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5a18-121">Defines a request to synchronize a folder hierarchy in an Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c5a18-122">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="c5a18-122">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="c5a18-123">Définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5a18-123">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c5a18-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="c5a18-124">Remarks</span></span>

<span data-ttu-id="c5a18-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="c5a18-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5a18-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c5a18-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5a18-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c5a18-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c5a18-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c5a18-128">Schema name</span></span>  <br/> |<span data-ttu-id="c5a18-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c5a18-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c5a18-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c5a18-130">Validation file</span></span>  <br/> |<span data-ttu-id="c5a18-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c5a18-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c5a18-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c5a18-132">Can be empty</span></span>  <br/> |<span data-ttu-id="c5a18-133">False</span><span class="sxs-lookup"><span data-stu-id="c5a18-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5a18-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c5a18-134">See also</span></span>

- [<span data-ttu-id="c5a18-135">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="c5a18-135">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="c5a18-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c5a18-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

