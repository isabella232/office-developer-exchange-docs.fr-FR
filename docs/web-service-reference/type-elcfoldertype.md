---
title: Type (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: L’élément type spécifie le type de dossier utilisé dans une stratégie de rétention.
ms.openlocfilehash: f6fcc7942a530ada2d6e72c3e38286a7595b09ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465106"
---
# <a name="type-elcfoldertype"></a><span data-ttu-id="ab31e-103">Type (ElcFolderType)</span><span class="sxs-lookup"><span data-stu-id="ab31e-103">Type (ElcFolderType)</span></span>

<span data-ttu-id="ab31e-104">L’élément **type** spécifie le type de dossier utilisé dans une stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="ab31e-104">The **Type** element specifies the type of folder used in a retention policy.</span></span> 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 <span data-ttu-id="ab31e-105">**ElcFolderType**</span><span class="sxs-lookup"><span data-stu-id="ab31e-105">**ElcFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ab31e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ab31e-106">Attributes and elements</span></span>

<span data-ttu-id="ab31e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ab31e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ab31e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ab31e-108">Attributes</span></span>

<span data-ttu-id="ab31e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ab31e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ab31e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ab31e-110">Child elements</span></span>

<span data-ttu-id="ab31e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ab31e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ab31e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ab31e-112">Parent elements</span></span>

[<span data-ttu-id="ab31e-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="ab31e-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="ab31e-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ab31e-114">Text value</span></span>

<span data-ttu-id="ab31e-115">La valeur de texte de l’élément **type** est le type de dossier utilisé dans une stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="ab31e-115">The text value of the **Type** element is the folder type used in a retention policy.</span></span> <span data-ttu-id="ab31e-116">La valeur de texte peut être une des valeurs suivantes qui représentent un type de dossier par défaut : calendrier, contacts, DeletedItems, brouillons, boîte de réception, JunkEmail, Journal, notes, boîte d’envoi, éléments envoyés, tâches, tout, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, personnel, RecoverableItems ou NonIpmRoot</span><span class="sxs-lookup"><span data-stu-id="ab31e-116">The text value can be one of the following values that represent a default folder type: Calendar, Contacts, DeletedItems, Drafts, Inbox, JunkEmail, Journal, Notes, Outbox, SentItems, Tasks, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, Personal, RecoverableItems, or NonIpmRoot</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ab31e-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="ab31e-117">Remarks</span></span>

<span data-ttu-id="ab31e-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ab31e-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ab31e-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab31e-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ab31e-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ab31e-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ab31e-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ab31e-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ab31e-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ab31e-122">Schema name</span></span>  <br/> |<span data-ttu-id="ab31e-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ab31e-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="ab31e-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ab31e-124">Validation file</span></span>  <br/> |<span data-ttu-id="ab31e-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ab31e-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ab31e-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ab31e-126">Can be empty</span></span>  <br/> |<span data-ttu-id="ab31e-127">false</span><span class="sxs-lookup"><span data-stu-id="ab31e-127">false</span></span>  <br/> |
   

