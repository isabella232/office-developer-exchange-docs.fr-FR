---
title: AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65554e4c-c0d9-485e-9f01-ed1baa8280ab
description: L’élément AddImContactToGroup définit une demande pour ajouter un contact de messagerie instantanée existant à un groupe de messagerie instantané.
ms.openlocfilehash: 71c841ce6df2ed7dcbbf77597b26f3e3e742a7fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755246"
---
# <a name="addimcontacttogroup"></a><span data-ttu-id="6d218-103">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="6d218-103">AddImContactToGroup</span></span>

<span data-ttu-id="6d218-104">L’élément **AddImContactToGroup** définit une demande pour ajouter un contact de messagerie instantanée existant à un groupe de messagerie instantané.</span><span class="sxs-lookup"><span data-stu-id="6d218-104">The **AddImContactToGroup** element defines a request to add an existing instant messaging contact to an instant messaging group.</span></span> 
  
```XML
<AddImContactToGroup>
   <ContactId/>
   <GroupId/>
</AddImContactToGroup>
```

 <span data-ttu-id="6d218-105">**AddImContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="6d218-105">**AddImContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d218-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6d218-106">Attributes and elements</span></span>

<span data-ttu-id="6d218-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6d218-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d218-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6d218-108">Attributes</span></span>

<span data-ttu-id="6d218-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6d218-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d218-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6d218-110">Child elements</span></span>

<span data-ttu-id="6d218-111">[ContactId](contactid.md) | [GroupId](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="6d218-111">[ContactId](contactid.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d218-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6d218-112">Parent elements</span></span>

<span data-ttu-id="6d218-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6d218-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6d218-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="6d218-114">Remarks</span></span>

<span data-ttu-id="6d218-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6d218-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6d218-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d218-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d218-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6d218-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d218-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6d218-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6d218-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6d218-119">Schema name</span></span>  <br/> |<span data-ttu-id="6d218-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6d218-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6d218-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6d218-121">Validation file</span></span>  <br/> |<span data-ttu-id="6d218-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6d218-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6d218-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6d218-123">Can be empty</span></span>  <br/> |<span data-ttu-id="6d218-124">false</span><span class="sxs-lookup"><span data-stu-id="6d218-124">false</span></span>  <br/> |
   

