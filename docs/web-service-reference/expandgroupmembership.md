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
ms.openlocfilehash: 8a94aa3da165ecc13282127e75c8d166f3972ead
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456905"
---
# <a name="expandgroupmembership"></a><span data-ttu-id="3802d-103">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="3802d-103">ExpandGroupMembership</span></span>

<span data-ttu-id="3802d-104">L’élément **ExpandGroupMembership** indique s’il faut développer l’appartenance au groupe renvoyé à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="3802d-104">The **ExpandGroupMembership** element indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 <span data-ttu-id="3802d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3802d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3802d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3802d-106">Attributes and elements</span></span>

<span data-ttu-id="3802d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3802d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3802d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3802d-108">Attributes</span></span>

<span data-ttu-id="3802d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3802d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3802d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3802d-110">Child elements</span></span>

<span data-ttu-id="3802d-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3802d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3802d-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3802d-112">Parent elements</span></span>

<span data-ttu-id="3802d-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md)  |  [GetSearchableMailboxes](getsearchablemailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="3802d-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3802d-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="3802d-114">Text value</span></span>

<span data-ttu-id="3802d-115">Une valeur de texte de **true** pour l’élément **ExpandGroupElement** indique que l’appartenance au groupe est étendue.</span><span class="sxs-lookup"><span data-stu-id="3802d-115">A text value of **true** for the **ExpandGroupElement** element indicates that group membership is expanded.</span></span> <span data-ttu-id="3802d-116">La valeur **false** indique que l’appartenance au groupe n’est pas développée pour afficher les membres du groupe.</span><span class="sxs-lookup"><span data-stu-id="3802d-116">A value of **false** indicates that the group membership is not expanded to show the members of the group.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3802d-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="3802d-117">Remarks</span></span>

<span data-ttu-id="3802d-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3802d-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3802d-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3802d-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3802d-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3802d-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3802d-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3802d-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3802d-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3802d-122">Schema name</span></span>  <br/> |<span data-ttu-id="3802d-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3802d-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3802d-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3802d-124">Validation file</span></span>  <br/> |<span data-ttu-id="3802d-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3802d-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3802d-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3802d-126">Can be empty</span></span>  <br/> |<span data-ttu-id="3802d-127">false</span><span class="sxs-lookup"><span data-stu-id="3802d-127">false</span></span>  <br/> |
   

