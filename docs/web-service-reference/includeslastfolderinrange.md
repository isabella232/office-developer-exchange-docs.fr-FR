---
title: IncludesLastFolderInRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludesLastFolderInRange
api_type:
- schema
ms.assetid: 95837904-17be-49b7-831c-de4fb20fccfb
description: L’élément IncludesLastFolderInRange indique si le dernier élément à synchroniser a été inclus dans la réponse.
ms.openlocfilehash: 9ba401cf639ef7988fa7a1437a64d09ff54c5960
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466450"
---
# <a name="includeslastfolderinrange"></a><span data-ttu-id="1fe43-103">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="1fe43-103">IncludesLastFolderInRange</span></span>

<span data-ttu-id="1fe43-104">L’élément **IncludesLastFolderInRange** indique si le dernier élément à synchroniser a été inclus dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="1fe43-104">The **IncludesLastFolderInRange** element indicates whether the last item to synchronize has been included in the response.</span></span> 
  
[<span data-ttu-id="1fe43-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="1fe43-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="1fe43-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1fe43-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="1fe43-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1fe43-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="1fe43-108">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="1fe43-108">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
  
```xml
<IncludesLastFolderInRange/>
```

 <span data-ttu-id="1fe43-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1fe43-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1fe43-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1fe43-110">Attributes and elements</span></span>

<span data-ttu-id="1fe43-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1fe43-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1fe43-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="1fe43-112">Attributes</span></span>

<span data-ttu-id="1fe43-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1fe43-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1fe43-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1fe43-114">Child elements</span></span>

<span data-ttu-id="1fe43-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1fe43-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1fe43-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1fe43-116">Parent elements</span></span>

|<span data-ttu-id="1fe43-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1fe43-117">**Element**</span></span>|<span data-ttu-id="1fe43-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="1fe43-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1fe43-119">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1fe43-119">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="1fe43-120">Contient l’État et le résultat d’une demande Opérationsyncfolderhierarchy.</span><span class="sxs-lookup"><span data-stu-id="1fe43-120">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1fe43-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="1fe43-121">Text value</span></span>

<span data-ttu-id="1fe43-122">Une valeur de texte qui représente une valeur Boolean est requise.</span><span class="sxs-lookup"><span data-stu-id="1fe43-122">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1fe43-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="1fe43-123">Remarks</span></span>

<span data-ttu-id="1fe43-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1fe43-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1fe43-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1fe43-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1fe43-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1fe43-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1fe43-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1fe43-127">Schema name</span></span>  <br/> |<span data-ttu-id="1fe43-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1fe43-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1fe43-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1fe43-129">Validation file</span></span>  <br/> |<span data-ttu-id="1fe43-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1fe43-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1fe43-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1fe43-131">Can be empty</span></span>  <br/> |<span data-ttu-id="1fe43-132">False</span><span class="sxs-lookup"><span data-stu-id="1fe43-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1fe43-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1fe43-133">See also</span></span>



[<span data-ttu-id="1fe43-134">Opération Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="1fe43-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


[<span data-ttu-id="1fe43-135">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="1fe43-135">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
  
- [<span data-ttu-id="1fe43-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1fe43-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

