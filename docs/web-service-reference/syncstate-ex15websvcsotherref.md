---
title: SyncState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncState
api_type:
- schema
ms.assetid: e5ebaae3-0f07-481d-ac67-d9687a3c7ac3
description: L’élément SyncState contient un formulaire encodé en base64 des données de synchronisation qui est mis à jour après chaque demande réussie. Il est utilisé pour identifier l’état de synchronisation.
ms.openlocfilehash: 8e2d9a633cdad0a124b87e4e794399c06d3b5445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458963"
---
# <a name="syncstate"></a><span data-ttu-id="57c0d-104">SyncState</span><span class="sxs-lookup"><span data-stu-id="57c0d-104">SyncState</span></span>

<span data-ttu-id="57c0d-105">L’élément **SyncState** contient un formulaire encodé en base64 des données de synchronisation qui est mis à jour après chaque demande réussie.</span><span class="sxs-lookup"><span data-stu-id="57c0d-105">The **SyncState** element contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="57c0d-106">Il est utilisé pour identifier l’état de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="57c0d-106">This is used to identify the synchronization state.</span></span> 
  
```xml
<SyncState/>
```

 <span data-ttu-id="57c0d-107">**String**</span><span class="sxs-lookup"><span data-stu-id="57c0d-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57c0d-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="57c0d-108">Attributes and elements</span></span>

<span data-ttu-id="57c0d-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="57c0d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57c0d-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="57c0d-110">Attributes</span></span>

<span data-ttu-id="57c0d-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="57c0d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57c0d-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="57c0d-112">Child elements</span></span>

<span data-ttu-id="57c0d-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="57c0d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57c0d-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="57c0d-114">Parent elements</span></span>

|<span data-ttu-id="57c0d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="57c0d-115">**Element**</span></span>|<span data-ttu-id="57c0d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="57c0d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57c0d-117">Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="57c0d-117">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="57c0d-118">Définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.</span><span class="sxs-lookup"><span data-stu-id="57c0d-118">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> |
|[<span data-ttu-id="57c0d-119">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="57c0d-119">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="57c0d-120">Contient l’État et le résultat d’une demande Opérationsyncfolderhierarchy.</span><span class="sxs-lookup"><span data-stu-id="57c0d-120">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
|[<span data-ttu-id="57c0d-121">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="57c0d-121">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="57c0d-122">Définit une demande de synchronisation des éléments dans un dossier de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="57c0d-122">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
|[<span data-ttu-id="57c0d-123">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="57c0d-123">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="57c0d-124">Contient l’État et le résultat d’une demande SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="57c0d-124">Contains the status and result of a SyncFolderItems request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57c0d-125">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="57c0d-125">Text value</span></span>

<span data-ttu-id="57c0d-126">Une valeur de texte est requise lorsque cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="57c0d-126">A text value is required when this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57c0d-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="57c0d-127">Remarks</span></span>

<span data-ttu-id="57c0d-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="57c0d-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57c0d-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="57c0d-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57c0d-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="57c0d-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57c0d-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="57c0d-131">Schema name</span></span>  <br/> |<span data-ttu-id="57c0d-132">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="57c0d-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="57c0d-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="57c0d-133">Validation file</span></span>  <br/> |<span data-ttu-id="57c0d-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="57c0d-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57c0d-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="57c0d-135">Can be empty</span></span>  <br/> |<span data-ttu-id="57c0d-136">False</span><span class="sxs-lookup"><span data-stu-id="57c0d-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57c0d-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="57c0d-137">See also</span></span>



[<span data-ttu-id="57c0d-138">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="57c0d-138">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
  
[<span data-ttu-id="57c0d-139">Opération Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="57c0d-139">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="57c0d-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="57c0d-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

