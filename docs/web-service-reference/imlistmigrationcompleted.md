---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: L’élément ImListMigrationCompleted indique si la banque d’informations Exchange contient les éléments de messagerie instantanées utilisés par les clients de messagerie instantanée.
ms.openlocfilehash: 25f1b583b354a71958fbc8052c492726dc0eb7db
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827893"
---
# <a name="imlistmigrationcompleted"></a><span data-ttu-id="2f025-103">ImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="2f025-103">ImListMigrationCompleted</span></span>

<span data-ttu-id="2f025-104">L’élément **ImListMigrationCompleted** indique si la banque d’informations Exchange contient les éléments utilisés par les clients de messagerie instantanée de la messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="2f025-104">The **ImListMigrationCompleted** element indicates whether the Exchange store contains the instant messaging items used by instant messaging clients.</span></span> 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 <span data-ttu-id="2f025-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2f025-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f025-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2f025-106">Attributes and elements</span></span>

<span data-ttu-id="2f025-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2f025-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f025-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2f025-108">Attributes</span></span>

<span data-ttu-id="2f025-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2f025-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f025-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2f025-110">Child elements</span></span>

<span data-ttu-id="2f025-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2f025-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2f025-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2f025-112">Parent elements</span></span>

[<span data-ttu-id="2f025-113">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="2f025-113">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a><span data-ttu-id="2f025-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2f025-114">Text value</span></span>

<span data-ttu-id="2f025-115">Une valeur de texte de **la valeur true** pour l’élément **ImListMigrationCompleted** indique que les contacts de messagerie instantanée store a été migré vers la version d’Exchange stockent.</span><span class="sxs-lookup"><span data-stu-id="2f025-115">A text value of **true** for the **ImListMigrationCompleted** element indicates that the instant messaging contacts store has been migrated to the Exchange store.</span></span> <span data-ttu-id="2f025-116">La valeur **false** indique que le magasin de contacts de messagerie instantanée n’a pas été migré.</span><span class="sxs-lookup"><span data-stu-id="2f025-116">A value of **false** indicates that the instant message contacts store has not been migrated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2f025-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="2f025-117">Remarks</span></span>

<span data-ttu-id="2f025-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2f025-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2f025-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f025-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f025-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2f025-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f025-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2f025-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2f025-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2f025-122">Schema name</span></span>  <br/> |<span data-ttu-id="2f025-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="2f025-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2f025-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2f025-124">Validation file</span></span>  <br/> |<span data-ttu-id="2f025-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2f025-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2f025-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2f025-126">Can be empty</span></span>  <br/> ||
   

