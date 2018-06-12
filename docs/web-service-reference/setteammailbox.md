---
title: SetTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d6ee7cc-8f88-4de2-ae5c-cabf2f2193d0
description: L’élément SetTeamMailbox contient une demande pour définir une boîte aux lettres du site.
ms.openlocfilehash: 708863168f4e89775deee8c5d66427df41515089
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829455"
---
# <a name="setteammailbox"></a><span data-ttu-id="0cd13-103">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="0cd13-103">SetTeamMailbox</span></span>

<span data-ttu-id="0cd13-104">L’élément **SetTeamMailbox** contient une demande pour définir une boîte aux lettres du site.</span><span class="sxs-lookup"><span data-stu-id="0cd13-104">The **SetTeamMailbox** element contains a request to set a site mailbox.</span></span> 
  
```XML
<SetTeamMailbox>
   <EmailAddress/>
   <SharePointSiteUrl/>
   <State/>
</SetTeamMailbox>
```

 <span data-ttu-id="0cd13-105">**SetTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="0cd13-105">**SetTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0cd13-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0cd13-106">Attributes and elements</span></span>

<span data-ttu-id="0cd13-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0cd13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0cd13-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0cd13-108">Attributes</span></span>

<span data-ttu-id="0cd13-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0cd13-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0cd13-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0cd13-110">Child elements</span></span>

<span data-ttu-id="0cd13-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [état (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span><span class="sxs-lookup"><span data-stu-id="0cd13-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [State (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0cd13-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0cd13-112">Parent elements</span></span>

<span data-ttu-id="0cd13-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0cd13-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0cd13-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="0cd13-114">Remarks</span></span>

<span data-ttu-id="0cd13-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0cd13-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0cd13-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0cd13-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0cd13-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0cd13-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0cd13-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0cd13-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0cd13-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0cd13-119">Schema name</span></span>  <br/> |<span data-ttu-id="0cd13-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0cd13-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0cd13-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0cd13-121">Validation file</span></span>  <br/> |<span data-ttu-id="0cd13-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0cd13-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0cd13-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0cd13-123">Can be empty</span></span>  <br/> ||
   

