---
title: ExpandGroupMembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: L’élément ExpandGroupMembership indique s’il faut développer l’appartenance au groupe renvoyé à partir d’une demande GetSearchableMailboxes.
ms.openlocfilehash: 11bfcf6893a147c726c94df77f7d9a9dfbaa773e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756259"
---
# <a name="expandgroupmembership"></a><span data-ttu-id="b1aac-103">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="b1aac-103">ExpandGroupMembership</span></span>

<span data-ttu-id="b1aac-104">L’élément **ExpandGroupMembership** indique s’il faut développer l’appartenance au groupe renvoyé à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="b1aac-104">The **ExpandGroupMembership** element indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 <span data-ttu-id="b1aac-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b1aac-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1aac-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b1aac-106">Attributes and elements</span></span>

<span data-ttu-id="b1aac-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b1aac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1aac-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b1aac-108">Attributes</span></span>

<span data-ttu-id="b1aac-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b1aac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b1aac-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b1aac-110">Child elements</span></span>

<span data-ttu-id="b1aac-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b1aac-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b1aac-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b1aac-112">Parent elements</span></span>

<span data-ttu-id="b1aac-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="b1aac-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b1aac-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b1aac-114">Text value</span></span>

<span data-ttu-id="b1aac-115">Une valeur de texte de **la valeur true** pour l’élément **ExpandGroupElement** indique que l’appartenance au groupe est développé.</span><span class="sxs-lookup"><span data-stu-id="b1aac-115">A text value of **true** for the **ExpandGroupElement** element indicates that group membership is expanded.</span></span> <span data-ttu-id="b1aac-116">La valeur **false** indique que l’appartenance au groupe n’est pas développé pour afficher les membres du groupe.</span><span class="sxs-lookup"><span data-stu-id="b1aac-116">A value of **false** indicates that the group membership is not expanded to show the members of the group.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b1aac-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="b1aac-117">Remarks</span></span>

<span data-ttu-id="b1aac-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b1aac-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b1aac-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b1aac-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b1aac-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b1aac-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1aac-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b1aac-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b1aac-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b1aac-122">Schema name</span></span>  <br/> |<span data-ttu-id="b1aac-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b1aac-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b1aac-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b1aac-124">Validation file</span></span>  <br/> |<span data-ttu-id="b1aac-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b1aac-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b1aac-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b1aac-126">Can be empty</span></span>  <br/> |<span data-ttu-id="b1aac-127">false</span><span class="sxs-lookup"><span data-stu-id="b1aac-127">false</span></span>  <br/> |
   

