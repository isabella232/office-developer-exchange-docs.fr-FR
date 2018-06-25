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
description: L’élément SyncState contient un formulaire de la synchronisation de données est mis à jour après chaque requête réussie codé en base64. Il est utilisé pour identifier l’état de synchronisation.
ms.openlocfilehash: 3c600dde09fd813dcfb1f6e74671ebe9004701a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838667"
---
# <a name="syncstate"></a><span data-ttu-id="7ffea-104">SyncState</span><span class="sxs-lookup"><span data-stu-id="7ffea-104">SyncState</span></span>

<span data-ttu-id="7ffea-105">L’élément **SyncState** contient un formulaire de la synchronisation de données est mis à jour après chaque requête réussie codé en base64.</span><span class="sxs-lookup"><span data-stu-id="7ffea-105">The **SyncState** element contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="7ffea-106">Il est utilisé pour identifier l’état de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="7ffea-106">This is used to identify the synchronization state.</span></span> 
  
```xml
<SyncState/>
```

 <span data-ttu-id="7ffea-107">**Chaîne**</span><span class="sxs-lookup"><span data-stu-id="7ffea-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ffea-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7ffea-108">Attributes and elements</span></span>

<span data-ttu-id="7ffea-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7ffea-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ffea-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="7ffea-110">Attributes</span></span>

<span data-ttu-id="7ffea-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7ffea-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ffea-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7ffea-112">Child elements</span></span>

<span data-ttu-id="7ffea-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7ffea-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7ffea-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7ffea-114">Parent elements</span></span>

|<span data-ttu-id="7ffea-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7ffea-115">**Element**</span></span>|<span data-ttu-id="7ffea-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="7ffea-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ffea-117">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="7ffea-117">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="7ffea-118">Définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.</span><span class="sxs-lookup"><span data-stu-id="7ffea-118">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> |
|[<span data-ttu-id="7ffea-119">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7ffea-119">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="7ffea-120">Contient l’état et les résultats d’une demande SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="7ffea-120">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
|[<span data-ttu-id="7ffea-121">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7ffea-121">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="7ffea-122">Définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ffea-122">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
|[<span data-ttu-id="7ffea-123">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7ffea-123">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="7ffea-124">Contient l’état et les résultats d’une demande SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="7ffea-124">Contains the status and result of a SyncFolderItems request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7ffea-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7ffea-125">Text value</span></span>

<span data-ttu-id="7ffea-126">Une valeur de texte est requise lorsque cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="7ffea-126">A text value is required when this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7ffea-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="7ffea-127">Remarks</span></span>

<span data-ttu-id="7ffea-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7ffea-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ffea-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7ffea-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ffea-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7ffea-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7ffea-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7ffea-131">Schema name</span></span>  <br/> |<span data-ttu-id="7ffea-132">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7ffea-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7ffea-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7ffea-133">Validation file</span></span>  <br/> |<span data-ttu-id="7ffea-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7ffea-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7ffea-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7ffea-135">Can be empty</span></span>  <br/> |<span data-ttu-id="7ffea-136">False</span><span class="sxs-lookup"><span data-stu-id="7ffea-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ffea-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7ffea-137">See also</span></span>



[<span data-ttu-id="7ffea-138">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7ffea-138">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
  
[<span data-ttu-id="7ffea-139">Opération SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="7ffea-139">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="7ffea-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7ffea-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

