---
title: GetSearchableMailboxesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0fcc2f53-742b-46ae-bbab-c3295a3d69e7
description: L’élément GetSearchableMailboxesResponse contient la réponse à une demande de GetSearchableMailboxes.
ms.openlocfilehash: 35a671cd534d1b48b29ef836c24d97d7cbd52401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756740"
---
# <a name="getsearchablemailboxesresponse"></a><span data-ttu-id="0686f-103">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="0686f-103">GetSearchableMailboxesResponse</span></span>

<span data-ttu-id="0686f-104">L’élément **GetSearchableMailboxesResponse** contient la réponse à une demande de **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="0686f-104">The **GetSearchableMailboxesResponse** element contains the response to a **GetSearchableMailboxes** request.</span></span> 
  
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

 <span data-ttu-id="0686f-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0686f-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0686f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0686f-106">Attributes and elements</span></span>

<span data-ttu-id="0686f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0686f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0686f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0686f-108">Attributes</span></span>

<span data-ttu-id="0686f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0686f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0686f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0686f-110">Child elements</span></span>

<span data-ttu-id="0686f-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchableMailboxes](searchablemailboxes.md) | [FailedMailboxes](failedmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="0686f-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchableMailboxes](searchablemailboxes.md) | [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0686f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0686f-112">Parent elements</span></span>

<span data-ttu-id="0686f-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0686f-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0686f-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="0686f-114">Remarks</span></span>

<span data-ttu-id="0686f-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0686f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0686f-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0686f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0686f-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0686f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0686f-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0686f-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0686f-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0686f-119">Schema name</span></span>  <br/> |<span data-ttu-id="0686f-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0686f-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0686f-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0686f-121">Validation file</span></span>  <br/> |<span data-ttu-id="0686f-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0686f-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0686f-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0686f-123">Can be empty</span></span>  <br/> |<span data-ttu-id="0686f-124">false</span><span class="sxs-lookup"><span data-stu-id="0686f-124">false</span></span>  <br/> |
   

