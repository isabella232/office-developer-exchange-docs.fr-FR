---
title: MarkAsJunkResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e2b7b53-ef3c-438e-93df-b08409dbab46
description: L’élément MarkAsJunkResponseMessage Spécifie le message de réponse pour une demande MarkAsJunk.
ms.openlocfilehash: 146ece430436c60fced53d4dfbfd7d92c0e42e98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828352"
---
# <a name="markasjunkresponsemessage"></a><span data-ttu-id="c2d05-103">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c2d05-103">MarkAsJunkResponseMessage</span></span>

<span data-ttu-id="c2d05-104">L’élément **MarkAsJunkResponseMessage** Spécifie le message de réponse pour une demande **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="c2d05-104">The **MarkAsJunkResponseMessage** element specifies the response message for a **MarkAsJunk** request.</span></span> 
  
```XML
<MarkAsJunkResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MovedItemId/>
</MarkAsJunkResponseMessage>
```

 <span data-ttu-id="c2d05-105">**MarkAsJunkResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c2d05-105">**MarkAsJunkResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2d05-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c2d05-106">Attributes and elements</span></span>

<span data-ttu-id="c2d05-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c2d05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2d05-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c2d05-108">Attributes</span></span>

<span data-ttu-id="c2d05-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c2d05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2d05-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c2d05-110">Child elements</span></span>

<span data-ttu-id="c2d05-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MovedItemId](moveditemid.md)</span><span class="sxs-lookup"><span data-stu-id="c2d05-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MovedItemId](moveditemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c2d05-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c2d05-112">Parent elements</span></span>

[<span data-ttu-id="c2d05-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c2d05-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="c2d05-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="c2d05-114">Remarks</span></span>

<span data-ttu-id="c2d05-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c2d05-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c2d05-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2d05-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2d05-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c2d05-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2d05-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c2d05-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2d05-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c2d05-119">Schema name</span></span>  <br/> |<span data-ttu-id="c2d05-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c2d05-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c2d05-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c2d05-121">Validation file</span></span>  <br/> |<span data-ttu-id="c2d05-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c2d05-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2d05-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c2d05-123">Can be empty</span></span>  <br/> ||
   

