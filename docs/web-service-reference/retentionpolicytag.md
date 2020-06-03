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
ms.openlocfilehash: 3ece841e14e6cf11ab15e4a4d8b83a778ae32e46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465176"
---
# <a name="retentionpolicytag"></a><span data-ttu-id="39751-103">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="39751-103">RetentionPolicyTag</span></span>

<span data-ttu-id="39751-104">L’élément **RetentionPolicyTag** spécifie la stratégie de rétention pour un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="39751-104">The **RetentionPolicyTag** element specifies the retention policy for a mailbox item.</span></span> 
  
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

 <span data-ttu-id="39751-105">**RetentionPolicyTagType**</span><span class="sxs-lookup"><span data-stu-id="39751-105">**RetentionPolicyTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39751-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="39751-106">Attributes and elements</span></span>

<span data-ttu-id="39751-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="39751-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39751-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="39751-108">Attributes</span></span>

<span data-ttu-id="39751-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="39751-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39751-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="39751-110">Child elements</span></span>

<span data-ttu-id="39751-111">[DisplayName (String)](displayname-string.md)  |  [RetentionId](retentionid.md)  |  [RetentionPeriod](retentionperiod.md)  |  [Type (ElcFolderType)](type-elcfoldertype.md)  |  [RetentionAction](retentionaction.md)  |  [Description](description.md)  |  [IsVisible](isvisible.md)  |  [OptedInto](optedinto.md)  |  [IsArchive](isarchive.md)</span><span class="sxs-lookup"><span data-stu-id="39751-111">[DisplayName (string)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [Type (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [Description](description.md) | [IsVisible](isvisible.md) | [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="39751-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="39751-112">Parent elements</span></span>

[<span data-ttu-id="39751-113">RetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="39751-113">RetentionPolicyTags</span></span>](retentionpolicytags.md)
  
## <a name="remarks"></a><span data-ttu-id="39751-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="39751-114">Remarks</span></span>

<span data-ttu-id="39751-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="39751-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="39751-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="39751-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39751-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="39751-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39751-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="39751-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="39751-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="39751-119">Schema name</span></span>  <br/> |<span data-ttu-id="39751-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="39751-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="39751-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="39751-121">Validation file</span></span>  <br/> |<span data-ttu-id="39751-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="39751-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="39751-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="39751-123">Can be empty</span></span>  <br/> ||
   

