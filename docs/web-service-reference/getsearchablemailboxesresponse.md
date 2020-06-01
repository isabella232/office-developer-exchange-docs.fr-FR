---
title: GetSearchableMailboxesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0fcc2f53-742b-46ae-bbab-c3295a3d69e7
description: L’élément GetSearchableMailboxesResponse contient la réponse à une demande GetSearchableMailboxes.
ms.openlocfilehash: 680fde9d9ad34dd0384e00da023796d004b66b1b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458263"
---
# <a name="getsearchablemailboxesresponse"></a><span data-ttu-id="3dcb2-103">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="3dcb2-103">GetSearchableMailboxesResponse</span></span>

<span data-ttu-id="3dcb2-104">L’élément **GetSearchableMailboxesResponse** contient la réponse à une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="3dcb2-104">The **GetSearchableMailboxesResponse** element contains the response to a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SearchableMailboxes/>
   <FailedMailboxes/>
</GetSearchableMailboxesResponse>
```

 <span data-ttu-id="3dcb2-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3dcb2-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3dcb2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3dcb2-106">Attributes and elements</span></span>

<span data-ttu-id="3dcb2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3dcb2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3dcb2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3dcb2-108">Attributes</span></span>

<span data-ttu-id="3dcb2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3dcb2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3dcb2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3dcb2-110">Child elements</span></span>

<span data-ttu-id="3dcb2-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [Messagexml](messagexml.md)  |  [SearchableMailboxes](searchablemailboxes.md)  |  [FailedMailboxes](failedmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="3dcb2-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchableMailboxes](searchablemailboxes.md) | [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3dcb2-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3dcb2-112">Parent elements</span></span>

<span data-ttu-id="3dcb2-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3dcb2-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3dcb2-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="3dcb2-114">Remarks</span></span>

<span data-ttu-id="3dcb2-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3dcb2-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3dcb2-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3dcb2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3dcb2-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3dcb2-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3dcb2-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3dcb2-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3dcb2-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3dcb2-119">Schema name</span></span>  <br/> |<span data-ttu-id="3dcb2-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3dcb2-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3dcb2-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3dcb2-121">Validation file</span></span>  <br/> |<span data-ttu-id="3dcb2-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3dcb2-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3dcb2-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3dcb2-123">Can be empty</span></span>  <br/> |<span data-ttu-id="3dcb2-124">false</span><span class="sxs-lookup"><span data-stu-id="3dcb2-124">false</span></span>  <br/> |
   

