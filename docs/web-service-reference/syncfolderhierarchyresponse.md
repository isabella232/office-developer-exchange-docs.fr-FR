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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838660"
---
# <a name="syncfolderhierarchyresponse"></a><span data-ttu-id="cbea9-103">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="cbea9-103">SyncFolderHierarchyResponse</span></span>

<span data-ttu-id="cbea9-104">L’élément **SyncFolderHierarchyResponse** définit une réponse à une demande SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="cbea9-104">The **SyncFolderHierarchyResponse** element defines a response to a SyncFolderHierarchy request.</span></span> 
  
```xml
<SyncFolderHierarchyResponse>
   <ResponseMessages/>
</SyncFolderHierarchyResponse>
```

 <span data-ttu-id="cbea9-105">**SyncFolderHierarchyResponseType**</span><span class="sxs-lookup"><span data-stu-id="cbea9-105">**SyncFolderHierarchyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cbea9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cbea9-106">Attributes and elements</span></span>

<span data-ttu-id="cbea9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cbea9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cbea9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cbea9-108">Attributes</span></span>

<span data-ttu-id="cbea9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cbea9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cbea9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cbea9-110">Child elements</span></span>

|<span data-ttu-id="cbea9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cbea9-111">**Element**</span></span>|<span data-ttu-id="cbea9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="cbea9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cbea9-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cbea9-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="cbea9-114">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cbea9-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cbea9-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cbea9-115">Parent elements</span></span>

<span data-ttu-id="cbea9-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cbea9-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cbea9-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="cbea9-117">Remarks</span></span>

<span data-ttu-id="cbea9-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="cbea9-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cbea9-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cbea9-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cbea9-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cbea9-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cbea9-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cbea9-121">Schema name</span></span>  <br/> |<span data-ttu-id="cbea9-122">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="cbea9-122">messages schema</span></span>  <br/> |
|<span data-ttu-id="cbea9-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cbea9-123">Validation file</span></span>  <br/> |<span data-ttu-id="cbea9-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cbea9-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cbea9-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cbea9-125">Can be empty</span></span>  <br/> |<span data-ttu-id="cbea9-126">False</span><span class="sxs-lookup"><span data-stu-id="cbea9-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cbea9-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cbea9-127">See also</span></span>



[<span data-ttu-id="cbea9-128">Opération SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="cbea9-128">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="cbea9-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cbea9-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

