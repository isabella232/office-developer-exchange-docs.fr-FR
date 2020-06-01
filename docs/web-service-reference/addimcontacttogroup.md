---
title: AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65554e4c-c0d9-485e-9f01-ed1baa8280ab
description: L’élément AddImContactToGroup définit une demande d’ajout d’un contact de messagerie instantanée existant à un groupe de messagerie instantanée.
ms.openlocfilehash: b86b1cb69a1ebc7034e5a27047c14efbab7236ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459664"
---
# <a name="addimcontacttogroup"></a><span data-ttu-id="f7fc8-103">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="f7fc8-103">AddImContactToGroup</span></span>

<span data-ttu-id="f7fc8-104">L’élément **AddImContactToGroup** définit une demande d’ajout d’un contact de messagerie instantanée existant à un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="f7fc8-104">The **AddImContactToGroup** element defines a request to add an existing instant messaging contact to an instant messaging group.</span></span> 
  
```XML
<AddImContactToGroup>
   <ContactId/>
   <GroupId/>
</AddImContactToGroup>
```

 <span data-ttu-id="f7fc8-105">**AddImContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="f7fc8-105">**AddImContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7fc8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f7fc8-106">Attributes and elements</span></span>

<span data-ttu-id="f7fc8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f7fc8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7fc8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f7fc8-108">Attributes</span></span>

<span data-ttu-id="f7fc8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f7fc8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7fc8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f7fc8-110">Child elements</span></span>

<span data-ttu-id="f7fc8-111">[ContactID](contactid.md)  |  [GroupID](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="f7fc8-111">[ContactId](contactid.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f7fc8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f7fc8-112">Parent elements</span></span>

<span data-ttu-id="f7fc8-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f7fc8-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f7fc8-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="f7fc8-114">Remarks</span></span>

<span data-ttu-id="f7fc8-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f7fc8-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f7fc8-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7fc8-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7fc8-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f7fc8-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7fc8-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f7fc8-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f7fc8-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f7fc8-119">Schema name</span></span>  <br/> |<span data-ttu-id="f7fc8-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f7fc8-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f7fc8-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f7fc8-121">Validation file</span></span>  <br/> |<span data-ttu-id="f7fc8-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f7fc8-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f7fc8-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f7fc8-123">Can be empty</span></span>  <br/> |<span data-ttu-id="f7fc8-124">false</span><span class="sxs-lookup"><span data-stu-id="f7fc8-124">false</span></span>  <br/> |
   

