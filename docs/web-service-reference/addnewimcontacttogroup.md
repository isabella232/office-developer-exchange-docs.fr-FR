---
title: AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5913619-0c13-429d-b9d2-057e8af220f1
description: L’élément AddNewImContactToGroup définit une demande pour ajouter un nouveau contact de messagerie instantané à un groupe de messagerie instantané.
ms.openlocfilehash: 2736bac6880a11101e9bffee12033c838705700e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755174"
---
# <a name="addnewimcontacttogroup"></a><span data-ttu-id="7b510-103">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="7b510-103">AddNewImContactToGroup</span></span>

<span data-ttu-id="7b510-104">L’élément **AddNewImContactToGroup** définit une demande pour ajouter un nouveau contact de messagerie instantané à un groupe de messagerie instantané.</span><span class="sxs-lookup"><span data-stu-id="7b510-104">The **AddNewImContactToGroup** element defines a request to add a new instant messaging contact to an instant messaging group.</span></span> 
  
```XML
<AddNewImContactToGroup>
   <ImAddress/>
   <DisplayName/>
   <GroupId/>
</AddNewImContactToGroup>
```

 <span data-ttu-id="7b510-105">**AddNewImContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="7b510-105">**AddNewImContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b510-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7b510-106">Attributes and elements</span></span>

<span data-ttu-id="7b510-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7b510-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b510-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7b510-108">Attributes</span></span>

<span data-ttu-id="7b510-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7b510-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b510-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7b510-110">Child elements</span></span>

<span data-ttu-id="7b510-111">[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupId](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="7b510-111">[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7b510-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7b510-112">Parent elements</span></span>

<span data-ttu-id="7b510-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7b510-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7b510-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="7b510-114">Remarks</span></span>

<span data-ttu-id="7b510-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7b510-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7b510-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b510-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b510-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7b510-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b510-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7b510-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7b510-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7b510-119">Schema name</span></span>  <br/> |<span data-ttu-id="7b510-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7b510-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7b510-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7b510-121">Validation file</span></span>  <br/> |<span data-ttu-id="7b510-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7b510-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7b510-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7b510-123">Can be empty</span></span>  <br/> |<span data-ttu-id="7b510-124">false</span><span class="sxs-lookup"><span data-stu-id="7b510-124">false</span></span>  <br/> |
   

