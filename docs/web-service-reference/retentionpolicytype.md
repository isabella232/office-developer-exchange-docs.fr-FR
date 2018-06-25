---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: L’élément RetentionPolicyType Spécifie le type de stratégie de rétention appliqué aux éléments d’une conversation.
ms.openlocfilehash: dacb3fa75611cbd6e6e29eab7c791dfd8964c9ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829229"
---
# <a name="retentionpolicytype"></a><span data-ttu-id="10c86-103">RetentionPolicyType</span><span class="sxs-lookup"><span data-stu-id="10c86-103">RetentionPolicyType</span></span>

<span data-ttu-id="10c86-104">L’élément **RetentionPolicyType** Spécifie le type de stratégie de rétention appliqué aux éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="10c86-104">The **RetentionPolicyType** element specifies the retention policy type applied to items in a conversation.</span></span> 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 <span data-ttu-id="10c86-105">**RetentionType**</span><span class="sxs-lookup"><span data-stu-id="10c86-105">**RetentionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="10c86-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="10c86-106">Attributes and elements</span></span>

<span data-ttu-id="10c86-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="10c86-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10c86-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="10c86-108">Attributes</span></span>

<span data-ttu-id="10c86-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="10c86-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10c86-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="10c86-110">Child elements</span></span>

<span data-ttu-id="10c86-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="10c86-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="10c86-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="10c86-112">Parent elements</span></span>

[<span data-ttu-id="10c86-113">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="10c86-113">ConversationAction</span></span>](conversationaction.md)
  
## <a name="text-value"></a><span data-ttu-id="10c86-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="10c86-114">Text value</span></span>

<span data-ttu-id="10c86-115">La valeur de texte de l’élément **RetentionPolicyType** est le type de rétention appliqué aux éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="10c86-115">The text value of the **RetentionPolicyType** element is the retention type applied to items in a conversation.</span></span> <span data-ttu-id="10c86-116">La valeur de texte de **suppression** indique que les éléments de la conversation sont supprimés lorsque le blocage de rétention arrive à expiration.</span><span class="sxs-lookup"><span data-stu-id="10c86-116">The text value of **Delete** indicates that the items in the conversation are deleted when the retention hold expires.</span></span> <span data-ttu-id="10c86-117">La valeur de texte de **l’Archive** indique que les éléments de la conversation sont déplacés vers la boîte aux lettres d’archive lorsque le blocage de rétention arrive à expiration.</span><span class="sxs-lookup"><span data-stu-id="10c86-117">The text value of **Archive** indicates that the items in the conversation are moved to the archive mailbox when the retention hold expires.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="10c86-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="10c86-118">Remarks</span></span>

<span data-ttu-id="10c86-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="10c86-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="10c86-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="10c86-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10c86-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="10c86-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10c86-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="10c86-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="10c86-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="10c86-123">Schema name</span></span>  <br/> |<span data-ttu-id="10c86-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="10c86-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="10c86-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="10c86-125">Validation file</span></span>  <br/> |<span data-ttu-id="10c86-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="10c86-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="10c86-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="10c86-127">Can be empty</span></span>  <br/> ||
   

