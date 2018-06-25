---
title: GroupId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 656d9b9a-8a65-4a75-8466-5b0d96512dab
description: L’élément GroupId identifie de manière unique un groupe.
ms.openlocfilehash: eaba176321c0dd872b71ef50cbaa298d1277bb79
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827750"
---
# <a name="groupid"></a><span data-ttu-id="2b658-103">GroupId</span><span class="sxs-lookup"><span data-stu-id="2b658-103">GroupId</span></span>

<span data-ttu-id="2b658-104">L’élément **GroupId** identifie de manière unique un groupe.</span><span class="sxs-lookup"><span data-stu-id="2b658-104">The **GroupId** element uniquely identifies a group.</span></span> 
  
```XML
<GroupId Id="" ChangeKey=""/>
```

 <span data-ttu-id="2b658-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="2b658-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b658-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2b658-106">Attributes and elements</span></span>

<span data-ttu-id="2b658-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2b658-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b658-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2b658-108">Attributes</span></span>

|<span data-ttu-id="2b658-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="2b658-109">**Attribute**</span></span>|<span data-ttu-id="2b658-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b658-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2b658-111">ID</span><span class="sxs-lookup"><span data-stu-id="2b658-111">Id</span></span>  <br/> |<span data-ttu-id="2b658-112">La valeur de texte de l’attribut **Id** est l’identificateur du groupe.</span><span class="sxs-lookup"><span data-stu-id="2b658-112">The text value of the **Id** attribute is the identifier of the group.</span></span>  <br/> |
|<span data-ttu-id="2b658-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="2b658-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="2b658-114">La valeur de texte de l’attribut **ChangeKey** est la clé de modification du groupe.</span><span class="sxs-lookup"><span data-stu-id="2b658-114">The text value of the **ChangeKey** attribute is the change key of the group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2b658-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2b658-115">Child elements</span></span>

<span data-ttu-id="2b658-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2b658-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2b658-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2b658-117">Parent elements</span></span>

<span data-ttu-id="2b658-118">[AddNewImContactToGroup](addnewimcontacttogroup.md) | [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md) | [AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md) | [RemoveImGroup](removeimgroup.md)  |  [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md) | [SetImGroup](setimgroup.md)</span><span class="sxs-lookup"><span data-stu-id="2b658-118">[AddNewImContactToGroup](addnewimcontacttogroup.md) | [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md) | [AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md) | [RemoveImGroup](removeimgroup.md) | [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md) | [SetImGroup](setimgroup.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2b658-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="2b658-119">Remarks</span></span>

<span data-ttu-id="2b658-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2b658-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2b658-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b658-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b658-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2b658-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b658-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2b658-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2b658-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2b658-124">Schema name</span></span>  <br/> |<span data-ttu-id="2b658-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="2b658-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2b658-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2b658-126">Validation file</span></span>  <br/> |<span data-ttu-id="2b658-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2b658-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2b658-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2b658-128">Can be empty</span></span>  <br/> ||
   

