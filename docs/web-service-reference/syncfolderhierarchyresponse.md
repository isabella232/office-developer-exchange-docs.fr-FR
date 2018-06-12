---
title: SyncFolderHierarchyResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchyResponse
api_type:
- schema
ms.assetid: 7e6061d2-bbce-4864-a7bb-a6457628cb7c
description: L’élément SyncFolderHierarchyResponse définit une réponse à une demande SyncFolderHierarchy.
ms.openlocfilehash: aee70603b84dfdf5f7f580fd2566f7ebfbbce383
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838660"
---
# <a name="syncfolderhierarchyresponse"></a><span data-ttu-id="56dbd-103">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="56dbd-103">SyncFolderHierarchyResponse</span></span>

<span data-ttu-id="56dbd-104">L’élément **SyncFolderHierarchyResponse** définit une réponse à une demande SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="56dbd-104">The **SyncFolderHierarchyResponse** element defines a response to a SyncFolderHierarchy request.</span></span> 
  
```xml
<SyncFolderHierarchyResponse>
   <ResponseMessages/>
</SyncFolderHierarchyResponse>
```

 <span data-ttu-id="56dbd-105">**SyncFolderHierarchyResponseType**</span><span class="sxs-lookup"><span data-stu-id="56dbd-105">**SyncFolderHierarchyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56dbd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="56dbd-106">Attributes and elements</span></span>

<span data-ttu-id="56dbd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="56dbd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56dbd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="56dbd-108">Attributes</span></span>

<span data-ttu-id="56dbd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="56dbd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56dbd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="56dbd-110">Child elements</span></span>

|<span data-ttu-id="56dbd-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="56dbd-111">**Element**</span></span>|<span data-ttu-id="56dbd-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="56dbd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56dbd-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="56dbd-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="56dbd-114">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="56dbd-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="56dbd-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="56dbd-115">Parent elements</span></span>

<span data-ttu-id="56dbd-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="56dbd-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="56dbd-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="56dbd-117">Remarks</span></span>

<span data-ttu-id="56dbd-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="56dbd-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56dbd-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="56dbd-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56dbd-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="56dbd-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="56dbd-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="56dbd-121">Schema name</span></span>  <br/> |<span data-ttu-id="56dbd-122">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="56dbd-122">messages schema</span></span>  <br/> |
|<span data-ttu-id="56dbd-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="56dbd-123">Validation file</span></span>  <br/> |<span data-ttu-id="56dbd-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="56dbd-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="56dbd-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="56dbd-125">Can be empty</span></span>  <br/> |<span data-ttu-id="56dbd-126">False</span><span class="sxs-lookup"><span data-stu-id="56dbd-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56dbd-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="56dbd-127">See also</span></span>



[<span data-ttu-id="56dbd-128">Opération SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="56dbd-128">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="56dbd-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="56dbd-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

