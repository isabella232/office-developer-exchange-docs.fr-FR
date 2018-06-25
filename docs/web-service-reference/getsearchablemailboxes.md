---
title: GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 949871f7-0d10-498e-84aa-f0652f1193be
description: L’élément GetSearchableMailboxes contient une demande pour obtenir une liste des boîtes aux lettres que le client est autorisé à effectuer une recherche eDiscovery.
ms.openlocfilehash: 8cce18bb62d3840cb9883d20a380cc4f2193303e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756732"
---
# <a name="getsearchablemailboxes"></a><span data-ttu-id="0dda0-103">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="0dda0-103">GetSearchableMailboxes</span></span>

<span data-ttu-id="0dda0-104">L’élément **GetSearchableMailboxes** contient une demande pour obtenir une liste des boîtes aux lettres que le client est autorisé à effectuer une recherche eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="0dda0-104">The **GetSearchableMailboxes** element contains a request to get a list of mailboxes that the client has permission to perform an eDiscovery search.</span></span> 
  
```XML
<GetSearchableMailboxes>
   <SearchFilter/>
   <ExpandGroupMembership/>
</GetSearchableMailboxes>
```

 <span data-ttu-id="0dda0-105">**GetSearchableMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="0dda0-105">**GetSearchableMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0dda0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0dda0-106">Attributes and elements</span></span>

<span data-ttu-id="0dda0-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0dda0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0dda0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0dda0-108">Attributes</span></span>

<span data-ttu-id="0dda0-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0dda0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0dda0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0dda0-110">Child elements</span></span>

<span data-ttu-id="0dda0-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span><span class="sxs-lookup"><span data-stu-id="0dda0-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0dda0-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0dda0-112">Parent elements</span></span>

<span data-ttu-id="0dda0-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0dda0-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0dda0-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="0dda0-114">Remarks</span></span>

<span data-ttu-id="0dda0-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0dda0-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0dda0-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dda0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0dda0-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0dda0-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0dda0-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0dda0-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0dda0-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0dda0-119">Schema name</span></span>  <br/> |<span data-ttu-id="0dda0-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0dda0-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0dda0-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0dda0-121">Validation file</span></span>  <br/> |<span data-ttu-id="0dda0-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0dda0-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0dda0-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0dda0-123">Can be empty</span></span>  <br/> ||
   

