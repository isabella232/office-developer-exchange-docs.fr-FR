---
title: Opérationsyncfolderhierarchy
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
description: L’élément Opérationsyncfolderhierarchy définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.
ms.openlocfilehash: 68b607dbf603e955f74dfaccadd3ce6c4c9fb6ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466646"
---
# <a name="syncfolderhierarchy"></a><span data-ttu-id="94350-103">Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="94350-103">SyncFolderHierarchy</span></span>

<span data-ttu-id="94350-104">L’élément **opérationsyncfolderhierarchy** définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.</span><span class="sxs-lookup"><span data-stu-id="94350-104">The **SyncFolderHierarchy** element defines a request to synchronize a folder hierarchy on a client.</span></span> 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 <span data-ttu-id="94350-105">**SyncFolderHierarchyType**</span><span class="sxs-lookup"><span data-stu-id="94350-105">**SyncFolderHierarchyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94350-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="94350-106">Attributes and elements</span></span>

<span data-ttu-id="94350-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="94350-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94350-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="94350-108">Attributes</span></span>

<span data-ttu-id="94350-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="94350-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94350-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="94350-110">Child elements</span></span>

|<span data-ttu-id="94350-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="94350-111">**Element**</span></span>|<span data-ttu-id="94350-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="94350-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94350-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="94350-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="94350-114">Identifie les propriétés de dossier à inclure dans une réponse [opérationsyncfolderhierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="94350-114">Identifies the folder properties to include in a [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span>  <br/> |
|[<span data-ttu-id="94350-115">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="94350-115">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="94350-116">Représente le dossier qui contient les éléments à synchroniser.</span><span class="sxs-lookup"><span data-stu-id="94350-116">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="94350-117">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="94350-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="94350-118">SyncState</span><span class="sxs-lookup"><span data-stu-id="94350-118">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="94350-119">Contient un formulaire codé en base64 des données de synchronisation qui sont mises à jour après chaque demande réussie.</span><span class="sxs-lookup"><span data-stu-id="94350-119">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="94350-120">Il est utilisé pour identifier l’état de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="94350-120">This is used to identify the synchronization state.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="94350-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="94350-121">Parent elements</span></span>

<span data-ttu-id="94350-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="94350-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="94350-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="94350-123">Remarks</span></span>

<span data-ttu-id="94350-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="94350-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94350-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="94350-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94350-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="94350-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="94350-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="94350-127">Schema name</span></span>  <br/> |<span data-ttu-id="94350-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="94350-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="94350-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="94350-129">Validation file</span></span>  <br/> |<span data-ttu-id="94350-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="94350-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="94350-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="94350-131">Can be empty</span></span>  <br/> |<span data-ttu-id="94350-132">False</span><span class="sxs-lookup"><span data-stu-id="94350-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94350-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="94350-133">See also</span></span>



[<span data-ttu-id="94350-134">Opération Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="94350-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="94350-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="94350-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

