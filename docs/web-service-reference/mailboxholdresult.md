---
title: MailboxHoldResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: da03b877-37c6-4ecb-8549-c639f140302e
description: L’élément MailboxHoldResult contient le résultat de la demande GetHoldOnMailboxes.
ms.openlocfilehash: 333a2d2d4a30a63a78660d167cefe75653f8ea82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828289"
---
# <a name="mailboxholdresult"></a><span data-ttu-id="a7645-103">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="a7645-103">MailboxHoldResult</span></span>

<span data-ttu-id="a7645-104">L’élément **MailboxHoldResult** contient le résultat de la demande **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="a7645-104">The **MailboxHoldResult** element contains the result of the **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<MailboxHoldResult>
   <HoldId/>
   <Query/>
   <MailboxHoldStatuses/>
</MailboxHoldResult>
```

<span data-ttu-id="a7645-105">**MailboxHoldResultType**</span><span class="sxs-lookup"><span data-stu-id="a7645-105">**MailboxHoldResultType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a7645-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a7645-106">Attributes and elements</span></span>

<span data-ttu-id="a7645-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a7645-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7645-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a7645-108">Attributes</span></span>

<span data-ttu-id="a7645-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a7645-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7645-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a7645-110">Child elements</span></span>

<span data-ttu-id="a7645-111">[HoldId](holdid.md) | [requête](query.md) | [MailboxHoldStatuses](mailboxholdstatuses.md)</span><span class="sxs-lookup"><span data-stu-id="a7645-111">[HoldId](holdid.md) | [Query](query.md) | [MailboxHoldStatuses](mailboxholdstatuses.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a7645-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a7645-112">Parent elements</span></span>

<span data-ttu-id="a7645-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a7645-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a7645-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="a7645-114">Remarks</span></span>

<span data-ttu-id="a7645-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a7645-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a7645-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7645-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7645-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a7645-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7645-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a7645-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a7645-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a7645-119">Schema name</span></span>  <br/> |<span data-ttu-id="a7645-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a7645-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a7645-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a7645-121">Validation file</span></span>  <br/> |<span data-ttu-id="a7645-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a7645-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a7645-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a7645-123">Can be empty</span></span>  <br/> ||
   

