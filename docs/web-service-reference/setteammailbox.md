---
title: SetTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d6ee7cc-8f88-4de2-ae5c-cabf2f2193d0
description: L’élément SetTeamMailbox contient une demande de définition d’une boîte aux lettres de site.
ms.openlocfilehash: e4b7ebd308f4b58b6b6491289f24b9176c5dcf15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465260"
---
# <a name="setteammailbox"></a><span data-ttu-id="21f7f-103">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="21f7f-103">SetTeamMailbox</span></span>

<span data-ttu-id="21f7f-104">L’élément **SetTeamMailbox** contient une demande de définition d’une boîte aux lettres de site.</span><span class="sxs-lookup"><span data-stu-id="21f7f-104">The **SetTeamMailbox** element contains a request to set a site mailbox.</span></span> 
  
```XML
<SetTeamMailbox>
   <EmailAddress/>
   <SharePointSiteUrl/>
   <State/>
</SetTeamMailbox>
```

 <span data-ttu-id="21f7f-105">**SetTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="21f7f-105">**SetTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21f7f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="21f7f-106">Attributes and elements</span></span>

<span data-ttu-id="21f7f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="21f7f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21f7f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="21f7f-108">Attributes</span></span>

<span data-ttu-id="21f7f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="21f7f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21f7f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="21f7f-110">Child elements</span></span>

<span data-ttu-id="21f7f-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)  |  [SharePointSiteUrl](sharepointsiteurl.md)  |  [État (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span><span class="sxs-lookup"><span data-stu-id="21f7f-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [State (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="21f7f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="21f7f-112">Parent elements</span></span>

<span data-ttu-id="21f7f-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="21f7f-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="21f7f-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="21f7f-114">Remarks</span></span>

<span data-ttu-id="21f7f-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="21f7f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="21f7f-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="21f7f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21f7f-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="21f7f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21f7f-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="21f7f-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21f7f-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="21f7f-119">Schema name</span></span>  <br/> |<span data-ttu-id="21f7f-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="21f7f-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="21f7f-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="21f7f-121">Validation file</span></span>  <br/> |<span data-ttu-id="21f7f-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="21f7f-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21f7f-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="21f7f-123">Can be empty</span></span>  <br/> ||
   

