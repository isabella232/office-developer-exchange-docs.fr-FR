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
ms.openlocfilehash: 35b66579116a00d27df722629ff980471ca0272e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530295"
---
# <a name="syncfolderid"></a><span data-ttu-id="49090-103">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="49090-103">SyncFolderId</span></span>

<span data-ttu-id="49090-104">L’élément **SyncFolderId** représente le dossier qui contient les éléments à synchroniser.</span><span class="sxs-lookup"><span data-stu-id="49090-104">The **SyncFolderId** element represents the folder that contains the items to synchronize.</span></span> 
  
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

<span data-ttu-id="49090-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="49090-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="49090-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="49090-106">Attributes and elements</span></span>

<span data-ttu-id="49090-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="49090-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49090-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="49090-108">Attributes</span></span>

<span data-ttu-id="49090-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="49090-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49090-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="49090-110">Child elements</span></span>

|<span data-ttu-id="49090-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="49090-111">**Element**</span></span>|<span data-ttu-id="49090-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="49090-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49090-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="49090-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="49090-114">Contient l’identificateur et la clé de modification d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="49090-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="49090-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="49090-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="49090-116">Identifie les dossiers MicrosoftExchange Server 2007 qui peuvent être référencés par nom.</span><span class="sxs-lookup"><span data-stu-id="49090-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49090-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="49090-117">Parent elements</span></span>

|<span data-ttu-id="49090-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="49090-118">**Element**</span></span>|<span data-ttu-id="49090-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="49090-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49090-120">Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="49090-120">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="49090-121">Définit une demande de synchronisation d’une hiérarchie de dossiers dans une banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="49090-121">Defines a request to synchronize a folder hierarchy in an Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="49090-122">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="49090-122">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="49090-123">Définit une demande de synchronisation des éléments dans un dossier de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="49090-123">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="49090-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="49090-124">Remarks</span></span>

<span data-ttu-id="49090-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="49090-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49090-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="49090-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49090-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="49090-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="49090-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="49090-128">Schema name</span></span>  <br/> |<span data-ttu-id="49090-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="49090-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="49090-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="49090-130">Validation file</span></span>  <br/> |<span data-ttu-id="49090-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="49090-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="49090-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="49090-132">Can be empty</span></span>  <br/> |<span data-ttu-id="49090-133">False</span><span class="sxs-lookup"><span data-stu-id="49090-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49090-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="49090-134">See also</span></span>

- [<span data-ttu-id="49090-135">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="49090-135">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="49090-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="49090-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

