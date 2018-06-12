---
title: Type (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: L’élément de Type spécifie le type de dossier utilisé dans une stratégie de rétention.
ms.openlocfilehash: f679a9237a577d26d4b28e1b25f3e135f7193903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838780"
---
# <a name="type-elcfoldertype"></a><span data-ttu-id="a4e8a-103">Type (ElcFolderType)</span><span class="sxs-lookup"><span data-stu-id="a4e8a-103">Type (ElcFolderType)</span></span>

<span data-ttu-id="a4e8a-104">L’élément de **Type** Spécifie le type de dossier utilisé dans une stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="a4e8a-104">The **Type** element specifies the type of folder used in a retention policy.</span></span> 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 <span data-ttu-id="a4e8a-105">**ElcFolderType**</span><span class="sxs-lookup"><span data-stu-id="a4e8a-105">**ElcFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4e8a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a4e8a-106">Attributes and elements</span></span>

<span data-ttu-id="a4e8a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a4e8a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4e8a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a4e8a-108">Attributes</span></span>

<span data-ttu-id="a4e8a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a4e8a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4e8a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a4e8a-110">Child elements</span></span>

<span data-ttu-id="a4e8a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a4e8a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a4e8a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a4e8a-112">Parent elements</span></span>

[<span data-ttu-id="a4e8a-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="a4e8a-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="a4e8a-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a4e8a-114">Text value</span></span>

<span data-ttu-id="a4e8a-115">La valeur de texte de l’élément **Type** est le type de dossier utilisé dans une stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="a4e8a-115">The text value of the **Type** element is the folder type used in a retention policy.</span></span> <span data-ttu-id="a4e8a-116">La valeur de texte peut être une des valeurs suivantes qui représentent un type de dossier par défaut : calendrier, Contacts, DeletedItems, Brouillons, boîte de réception, JunkEmail, Journal, Notes, boîte d’envoi, éléments envoyés, tâches, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, personnel, RecoverableItems ou NonIpmRoot</span><span class="sxs-lookup"><span data-stu-id="a4e8a-116">The text value can be one of the following values that represent a default folder type: Calendar, Contacts, DeletedItems, Drafts, Inbox, JunkEmail, Journal, Notes, Outbox, SentItems, Tasks, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, Personal, RecoverableItems, or NonIpmRoot</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a4e8a-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="a4e8a-117">Remarks</span></span>

<span data-ttu-id="a4e8a-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a4e8a-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a4e8a-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a4e8a-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4e8a-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a4e8a-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4e8a-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a4e8a-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a4e8a-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a4e8a-122">Schema name</span></span>  <br/> |<span data-ttu-id="a4e8a-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a4e8a-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="a4e8a-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a4e8a-124">Validation file</span></span>  <br/> |<span data-ttu-id="a4e8a-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a4e8a-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a4e8a-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a4e8a-126">Can be empty</span></span>  <br/> |<span data-ttu-id="a4e8a-127">false</span><span class="sxs-lookup"><span data-stu-id="a4e8a-127">false</span></span>  <br/> |
   

