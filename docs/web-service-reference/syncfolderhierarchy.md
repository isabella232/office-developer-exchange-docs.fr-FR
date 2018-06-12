---
title: SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: 55df4d01-e48e-4263-a851-78a66ad1093a
description: L’élément SyncFolderHierarchy définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.
ms.openlocfilehash: f72640e5605dd83e92cd323cb00e4d2f64406245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838658"
---
# <a name="syncfolderhierarchy"></a><span data-ttu-id="fb0f2-103">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="fb0f2-103">SyncFolderHierarchy</span></span>

<span data-ttu-id="fb0f2-104">L’élément **SyncFolderHierarchy** définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-104">The **SyncFolderHierarchy** element defines a request to synchronize a folder hierarchy on a client.</span></span> 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 <span data-ttu-id="fb0f2-105">**SyncFolderHierarchyType**</span><span class="sxs-lookup"><span data-stu-id="fb0f2-105">**SyncFolderHierarchyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb0f2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fb0f2-106">Attributes and elements</span></span>

<span data-ttu-id="fb0f2-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb0f2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fb0f2-108">Attributes</span></span>

<span data-ttu-id="fb0f2-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb0f2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fb0f2-110">Child elements</span></span>

|<span data-ttu-id="fb0f2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fb0f2-111">**Element**</span></span>|<span data-ttu-id="fb0f2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb0f2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb0f2-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="fb0f2-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="fb0f2-114">Identifie les propriétés du dossier à inclure dans une réponse [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="fb0f2-114">Identifies the folder properties to include in a [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span>  <br/> |
|[<span data-ttu-id="fb0f2-115">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="fb0f2-115">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="fb0f2-116">Représente le dossier qui contient les éléments à synchroniser.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-116">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="fb0f2-117">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="fb0f2-118">SyncState</span><span class="sxs-lookup"><span data-stu-id="fb0f2-118">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="fb0f2-119">Contient un formulaire de la synchronisation de données est mis à jour après chaque requête réussie codé en base64.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-119">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="fb0f2-120">Il est utilisé pour identifier l’état de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-120">This is used to identify the synchronization state.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb0f2-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fb0f2-121">Parent elements</span></span>

<span data-ttu-id="fb0f2-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb0f2-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="fb0f2-123">Remarks</span></span>

<span data-ttu-id="fb0f2-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fb0f2-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb0f2-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fb0f2-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb0f2-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fb0f2-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fb0f2-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fb0f2-127">Schema name</span></span>  <br/> |<span data-ttu-id="fb0f2-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="fb0f2-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fb0f2-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fb0f2-129">Validation file</span></span>  <br/> |<span data-ttu-id="fb0f2-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fb0f2-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb0f2-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fb0f2-131">Can be empty</span></span>  <br/> |<span data-ttu-id="fb0f2-132">False</span><span class="sxs-lookup"><span data-stu-id="fb0f2-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb0f2-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fb0f2-133">See also</span></span>



[<span data-ttu-id="fb0f2-134">Opération SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="fb0f2-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="fb0f2-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fb0f2-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

