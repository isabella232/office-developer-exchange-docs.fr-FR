---
title: AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5913619-0c13-429d-b9d2-057e8af220f1
description: L’élément AddNewImContactToGroup définit une demande d’ajout d’un nouveau contact de messagerie instantanée à un groupe de messagerie instantanée.
ms.openlocfilehash: c493ba81b23832a462acd425eb60297801f8768f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463649"
---
# <a name="addnewimcontacttogroup"></a><span data-ttu-id="04d3c-103">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="04d3c-103">AddNewImContactToGroup</span></span>

<span data-ttu-id="04d3c-104">L’élément **AddNewImContactToGroup** définit une demande d’ajout d’un nouveau contact de messagerie instantanée à un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="04d3c-104">The **AddNewImContactToGroup** element defines a request to add a new instant messaging contact to an instant messaging group.</span></span> 
  
```XML
<AddNewImContactToGroup>
   <ImAddress/>
   <DisplayName/>
   <GroupId/>
</AddNewImContactToGroup>
```

 <span data-ttu-id="04d3c-105">**AddNewImContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="04d3c-105">**AddNewImContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04d3c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="04d3c-106">Attributes and elements</span></span>

<span data-ttu-id="04d3c-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="04d3c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04d3c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="04d3c-108">Attributes</span></span>

<span data-ttu-id="04d3c-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="04d3c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04d3c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="04d3c-110">Child elements</span></span>

<span data-ttu-id="04d3c-111">[IMAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md)  |  [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)  |  [GroupID](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="04d3c-111">[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04d3c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="04d3c-112">Parent elements</span></span>

<span data-ttu-id="04d3c-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="04d3c-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04d3c-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="04d3c-114">Remarks</span></span>

<span data-ttu-id="04d3c-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="04d3c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="04d3c-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="04d3c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04d3c-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="04d3c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04d3c-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="04d3c-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="04d3c-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="04d3c-119">Schema name</span></span>  <br/> |<span data-ttu-id="04d3c-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="04d3c-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="04d3c-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="04d3c-121">Validation file</span></span>  <br/> |<span data-ttu-id="04d3c-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="04d3c-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="04d3c-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="04d3c-123">Can be empty</span></span>  <br/> |<span data-ttu-id="04d3c-124">false</span><span class="sxs-lookup"><span data-stu-id="04d3c-124">false</span></span>  <br/> |
   

