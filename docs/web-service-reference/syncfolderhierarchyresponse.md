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
description: L’élément SyncFolderHierarchyResponse définit une réponse à une demande Opérationsyncfolderhierarchy.
ms.openlocfilehash: bf17ee9080405d308328197f7cbeb92e9b1e02d3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456422"
---
# <a name="syncfolderhierarchyresponse"></a><span data-ttu-id="c6176-103">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="c6176-103">SyncFolderHierarchyResponse</span></span>

<span data-ttu-id="c6176-104">L’élément **SyncFolderHierarchyResponse** définit une réponse à une demande opérationsyncfolderhierarchy.</span><span class="sxs-lookup"><span data-stu-id="c6176-104">The **SyncFolderHierarchyResponse** element defines a response to a SyncFolderHierarchy request.</span></span> 
  
```xml
<SyncFolderHierarchyResponse>
   <ResponseMessages/>
</SyncFolderHierarchyResponse>
```

 <span data-ttu-id="c6176-105">**SyncFolderHierarchyResponseType**</span><span class="sxs-lookup"><span data-stu-id="c6176-105">**SyncFolderHierarchyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6176-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c6176-106">Attributes and elements</span></span>

<span data-ttu-id="c6176-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c6176-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6176-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c6176-108">Attributes</span></span>

<span data-ttu-id="c6176-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c6176-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6176-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c6176-110">Child elements</span></span>

|<span data-ttu-id="c6176-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c6176-111">**Element**</span></span>|<span data-ttu-id="c6176-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c6176-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6176-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c6176-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c6176-114">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c6176-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c6176-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c6176-115">Parent elements</span></span>

<span data-ttu-id="c6176-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c6176-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c6176-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="c6176-117">Remarks</span></span>

<span data-ttu-id="c6176-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c6176-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6176-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c6176-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6176-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c6176-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c6176-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c6176-121">Schema name</span></span>  <br/> |<span data-ttu-id="c6176-122">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="c6176-122">messages schema</span></span>  <br/> |
|<span data-ttu-id="c6176-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c6176-123">Validation file</span></span>  <br/> |<span data-ttu-id="c6176-124">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c6176-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c6176-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c6176-125">Can be empty</span></span>  <br/> |<span data-ttu-id="c6176-126">False</span><span class="sxs-lookup"><span data-stu-id="c6176-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6176-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c6176-127">See also</span></span>



[<span data-ttu-id="c6176-128">Opération Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="c6176-128">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="c6176-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c6176-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

