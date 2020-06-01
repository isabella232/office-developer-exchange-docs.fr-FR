---
title: MarkAsJunkResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e2b7b53-ef3c-438e-93df-b08409dbab46
description: L’élément MarkAsJunkResponseMessage spécifie le message de réponse pour une demande MarkAsJunk.
ms.openlocfilehash: be03fc964b56c463320f09e68d143a0377300f5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460098"
---
# <a name="markasjunkresponsemessage"></a><span data-ttu-id="5074a-103">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5074a-103">MarkAsJunkResponseMessage</span></span>

<span data-ttu-id="5074a-104">L’élément **MarkAsJunkResponseMessage** spécifie le message de réponse pour une demande **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="5074a-104">The **MarkAsJunkResponseMessage** element specifies the response message for a **MarkAsJunk** request.</span></span> 
  
```XML
<MarkAsJunkResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MovedItemId/>
</MarkAsJunkResponseMessage>
```

 <span data-ttu-id="5074a-105">**MarkAsJunkResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5074a-105">**MarkAsJunkResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5074a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5074a-106">Attributes and elements</span></span>

<span data-ttu-id="5074a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5074a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5074a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5074a-108">Attributes</span></span>

<span data-ttu-id="5074a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5074a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5074a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5074a-110">Child elements</span></span>

<span data-ttu-id="5074a-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [Messagexml](messagexml.md)  |  [MovedItemId](moveditemid.md)</span><span class="sxs-lookup"><span data-stu-id="5074a-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MovedItemId](moveditemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5074a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5074a-112">Parent elements</span></span>

[<span data-ttu-id="5074a-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5074a-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="5074a-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="5074a-114">Remarks</span></span>

<span data-ttu-id="5074a-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5074a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5074a-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5074a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5074a-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5074a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5074a-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5074a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5074a-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5074a-119">Schema name</span></span>  <br/> |<span data-ttu-id="5074a-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="5074a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5074a-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5074a-121">Validation file</span></span>  <br/> |<span data-ttu-id="5074a-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5074a-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5074a-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5074a-123">Can be empty</span></span>  <br/> ||
   

