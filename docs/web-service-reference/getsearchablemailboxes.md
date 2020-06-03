---
title: GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 949871f7-0d10-498e-84aa-f0652f1193be
description: L’élément GetSearchableMailboxes contient une demande pour obtenir la liste des boîtes aux lettres pour lesquelles le client est autorisé à effectuer une recherche de découverte électronique.
ms.openlocfilehash: a327f8766e53e9f1fae6928179d5a4b8e3d044a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530189"
---
# <a name="getsearchablemailboxes"></a><span data-ttu-id="fe2e1-103">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="fe2e1-103">GetSearchableMailboxes</span></span>

<span data-ttu-id="fe2e1-104">L’élément **GetSearchableMailboxes** contient une demande pour obtenir la liste des boîtes aux lettres pour lesquelles le client est autorisé à effectuer une recherche de découverte électronique.</span><span class="sxs-lookup"><span data-stu-id="fe2e1-104">The **GetSearchableMailboxes** element contains a request to get a list of mailboxes that the client has permission to perform an eDiscovery search.</span></span> 
  
```XML
<GetSearchableMailboxes>
   <SearchFilter/>
   <ExpandGroupMembership/>
</GetSearchableMailboxes>
```

 <span data-ttu-id="fe2e1-105">**GetSearchableMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="fe2e1-105">**GetSearchableMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fe2e1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fe2e1-106">Attributes and elements</span></span>

<span data-ttu-id="fe2e1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fe2e1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe2e1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fe2e1-108">Attributes</span></span>

<span data-ttu-id="fe2e1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fe2e1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe2e1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fe2e1-110">Child elements</span></span>

<span data-ttu-id="fe2e1-111">[Unsearchfilter](searchfilter.md)  |  [ExpandGroupMembership](expandgroupmembership.md)</span><span class="sxs-lookup"><span data-stu-id="fe2e1-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fe2e1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fe2e1-112">Parent elements</span></span>

<span data-ttu-id="fe2e1-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fe2e1-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fe2e1-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="fe2e1-114">Remarks</span></span>

<span data-ttu-id="fe2e1-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fe2e1-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fe2e1-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe2e1-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe2e1-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fe2e1-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe2e1-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fe2e1-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fe2e1-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fe2e1-119">Schema name</span></span>  <br/> |<span data-ttu-id="fe2e1-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="fe2e1-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fe2e1-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fe2e1-121">Validation file</span></span>  <br/> |<span data-ttu-id="fe2e1-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fe2e1-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fe2e1-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fe2e1-123">Can be empty</span></span>  <br/> ||
   

