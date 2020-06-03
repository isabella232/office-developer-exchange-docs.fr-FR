---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: L’élément RetentionPolicyType spécifie le type de stratégie de rétention appliqué aux éléments d’une conversation.
ms.openlocfilehash: 3900718f10e1e11d5864ebf7e64a3e1e22aa45c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462870"
---
# <a name="retentionpolicytype"></a><span data-ttu-id="4ef6c-103">RetentionPolicyType</span><span class="sxs-lookup"><span data-stu-id="4ef6c-103">RetentionPolicyType</span></span>

<span data-ttu-id="4ef6c-104">L’élément **RetentionPolicyType** spécifie le type de stratégie de rétention appliqué aux éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="4ef6c-104">The **RetentionPolicyType** element specifies the retention policy type applied to items in a conversation.</span></span> 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 <span data-ttu-id="4ef6c-105">**RetentionType**</span><span class="sxs-lookup"><span data-stu-id="4ef6c-105">**RetentionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ef6c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4ef6c-106">Attributes and elements</span></span>

<span data-ttu-id="4ef6c-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4ef6c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ef6c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4ef6c-108">Attributes</span></span>

<span data-ttu-id="4ef6c-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4ef6c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ef6c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4ef6c-110">Child elements</span></span>

<span data-ttu-id="4ef6c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4ef6c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ef6c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4ef6c-112">Parent elements</span></span>

[<span data-ttu-id="4ef6c-113">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="4ef6c-113">ConversationAction</span></span>](conversationaction.md)
  
## <a name="text-value"></a><span data-ttu-id="4ef6c-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4ef6c-114">Text value</span></span>

<span data-ttu-id="4ef6c-115">La valeur de texte de l’élément **RetentionPolicyType** est le type de rétention appliqué aux éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="4ef6c-115">The text value of the **RetentionPolicyType** element is the retention type applied to items in a conversation.</span></span> <span data-ttu-id="4ef6c-116">La valeur texte de **Delete** indique que les éléments de la conversation sont supprimés lorsque le blocage de rétention expire.</span><span class="sxs-lookup"><span data-stu-id="4ef6c-116">The text value of **Delete** indicates that the items in the conversation are deleted when the retention hold expires.</span></span> <span data-ttu-id="4ef6c-117">La valeur texte d' **Archive** indique que les éléments de la conversation sont déplacés vers la boîte aux lettres d’archivage lorsque le blocage de rétention expire.</span><span class="sxs-lookup"><span data-stu-id="4ef6c-117">The text value of **Archive** indicates that the items in the conversation are moved to the archive mailbox when the retention hold expires.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4ef6c-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="4ef6c-118">Remarks</span></span>

<span data-ttu-id="4ef6c-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4ef6c-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4ef6c-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ef6c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ef6c-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4ef6c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ef6c-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4ef6c-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ef6c-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4ef6c-123">Schema name</span></span>  <br/> |<span data-ttu-id="4ef6c-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4ef6c-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="4ef6c-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4ef6c-125">Validation file</span></span>  <br/> |<span data-ttu-id="4ef6c-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4ef6c-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ef6c-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4ef6c-127">Can be empty</span></span>  <br/> ||
   

