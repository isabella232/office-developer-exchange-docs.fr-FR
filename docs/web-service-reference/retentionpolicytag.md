---
title: RetentionPolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: L’élément RetentionPolicyTag spécifie la stratégie de rétention pour un élément de boîte aux lettres.
ms.openlocfilehash: 2525f6d7a0ca583342d28dd9f4857a69b3a8c05a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829226"
---
# <a name="retentionpolicytag"></a><span data-ttu-id="19c84-103">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="19c84-103">RetentionPolicyTag</span></span>

<span data-ttu-id="19c84-104">L’élément **RetentionPolicyTag** spécifie la stratégie de rétention pour un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="19c84-104">The **RetentionPolicyTag** element specifies the retention policy for a mailbox item.</span></span> 
  
```XML
<RetentionPolicyTag>
   <DisplayName/>
   <RetentionId/>
   <RetentionPeriod/>
   <Type/>
   <RetentionAction/>
   <Description/>
   <IsVisible/>
   <OptedInto/>
   <IsArchive/>
</RetentionPolicyTag>
```

 <span data-ttu-id="19c84-105">**RetentionPolicyTagType**</span><span class="sxs-lookup"><span data-stu-id="19c84-105">**RetentionPolicyTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19c84-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="19c84-106">Attributes and elements</span></span>

<span data-ttu-id="19c84-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="19c84-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19c84-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="19c84-108">Attributes</span></span>

<span data-ttu-id="19c84-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="19c84-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19c84-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="19c84-110">Child elements</span></span>

<span data-ttu-id="19c84-111">[DisplayName (string)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [Type (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [Description](description.md) | [IsVisible](isvisible.md)  |  [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span><span class="sxs-lookup"><span data-stu-id="19c84-111">[DisplayName (string)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [Type (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [Description](description.md) | [IsVisible](isvisible.md) | [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19c84-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="19c84-112">Parent elements</span></span>

[<span data-ttu-id="19c84-113">RetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="19c84-113">RetentionPolicyTags</span></span>](retentionpolicytags.md)
  
## <a name="remarks"></a><span data-ttu-id="19c84-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="19c84-114">Remarks</span></span>

<span data-ttu-id="19c84-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="19c84-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="19c84-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="19c84-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19c84-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="19c84-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19c84-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="19c84-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19c84-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="19c84-119">Schema name</span></span>  <br/> |<span data-ttu-id="19c84-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="19c84-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="19c84-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="19c84-121">Validation file</span></span>  <br/> |<span data-ttu-id="19c84-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="19c84-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19c84-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="19c84-123">Can be empty</span></span>  <br/> ||
   

