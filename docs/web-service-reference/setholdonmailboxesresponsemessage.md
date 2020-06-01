---
title: SetHoldOnMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d61de0f3-24e0-434a-946a-c53d393b7d04
description: L’élément SetHoldOnMailboxesResponseMessage spécifie le message de réponse pour une demande SetHoldOnMailboxes.
ms.openlocfilehash: a6af4181218391bc9d3c177467295d771cce4c89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456408"
---
# <a name="setholdonmailboxesresponsemessage"></a><span data-ttu-id="a72e0-103">SetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a72e0-103">SetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="a72e0-104">L’élément **SetHoldOnMailboxesResponseMessage** spécifie le message de réponse pour une demande **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="a72e0-104">The **SetHoldOnMailboxesResponseMessage** element specifies the response message for a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="a72e0-105">**SetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a72e0-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a72e0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a72e0-106">Attributes and elements</span></span>

<span data-ttu-id="a72e0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a72e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a72e0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a72e0-108">Attributes</span></span>

<span data-ttu-id="a72e0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a72e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a72e0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a72e0-110">Child elements</span></span>

<span data-ttu-id="a72e0-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [Messagexml](messagexml.md)  |  [MailboxHoldResult](mailboxholdresult.md)</span><span class="sxs-lookup"><span data-stu-id="a72e0-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a72e0-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a72e0-112">Parent elements</span></span>

[<span data-ttu-id="a72e0-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a72e0-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="a72e0-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="a72e0-114">Remarks</span></span>

<span data-ttu-id="a72e0-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a72e0-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a72e0-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a72e0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a72e0-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a72e0-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a72e0-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a72e0-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a72e0-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a72e0-119">Schema name</span></span>  <br/> |<span data-ttu-id="a72e0-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a72e0-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a72e0-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a72e0-121">Validation file</span></span>  <br/> |<span data-ttu-id="a72e0-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a72e0-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a72e0-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a72e0-123">Can be empty</span></span>  <br/> ||
   

