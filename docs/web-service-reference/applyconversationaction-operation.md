---
title: Opération de ApplyConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: 73d7943d-d361-4f8b-9948-d85f886efa1a
description: L’opération ApplyConversationAction définit une action de suivi unique ou ponctuelle sur tous les éléments d’une conversation. L’opération ApplyConversationAction vous permet de classer, déplacer, copier, supprimer et définir l’état de lecture sur tous les éléments d’une conversation. Les actions peuvent également être définies pour les nouveaux messages d’une conversation.
ms.openlocfilehash: cdab239a5b0b1406d2ce31f4604e4737d037cd7e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463502"
---
# <a name="applyconversationaction-operation"></a><span data-ttu-id="c8083-105">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="c8083-105">ApplyConversationAction operation</span></span>

<span data-ttu-id="c8083-106">L’opération **ApplyConversationAction** définit une action de suivi unique ou ponctuelle sur tous les éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="c8083-106">The **ApplyConversationAction** operation sets a one-time or follow up action on all the items in a conversation.</span></span> <span data-ttu-id="c8083-107">L’opération **ApplyConversationAction** vous permet de classer, déplacer, copier, supprimer et définir l’état de lecture sur tous les éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="c8083-107">The **ApplyConversationAction** operation allows you to categorize, move, copy, delete, and set the read state on all items in a conversation.</span></span> <span data-ttu-id="c8083-108">Les actions peuvent également être définies pour les nouveaux messages d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="c8083-108">Actions can also be set for new messages in a conversation.</span></span> 
  
## <a name="applyconversationaction-request-example"></a><span data-ttu-id="c8083-109">Exemple de requête ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="c8083-109">ApplyConversationAction request example</span></span>

### <a name="description"></a><span data-ttu-id="c8083-110">Description</span><span class="sxs-lookup"><span data-stu-id="c8083-110">Description</span></span>

<span data-ttu-id="c8083-111">L’exemple de requête **ApplyConversationAction** suivant montre comment déplacer les éléments de la conversation spécifiée dans un autre dossier.</span><span class="sxs-lookup"><span data-stu-id="c8083-111">The following example of an **ApplyConversationAction** request shows how to move the items in the specified conversation to another folder.</span></span> <span data-ttu-id="c8083-112">Les éléments ajoutés à la conversation seront également déplacés vers le dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="c8083-112">Items that are added to the conversation will also be moved to the specified folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c8083-113">Code</span><span class="sxs-lookup"><span data-stu-id="c8083-113">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ApplyConversationAction>
      <m:ConversationActions>
        <t:ConversationAction>
          <t:Action>AlwaysMove</t:Action>
          <t:ConversationId Id="AAQkADVkNjM1EH39AWcDUGrnrnJ32hHpdc="/>
          <t:DestinationFolderId>
            <t:FolderId Id="AAMkADVkNjM1ODI3LTEwYTAtNDUBTTT6tWal35iSoKAAAABZZWAAA="/>
          </t:DestinationFolderId>
        </t:ConversationAction>
      </m:ConversationActions>
    </m:ApplyConversationAction>
  </soap:Body>
</soap:Envelope>
```

### <a name="remarks"></a><span data-ttu-id="c8083-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="c8083-114">Remarks</span></span>

<span data-ttu-id="c8083-115">Les identificateurs de dossier et de conversation ont été raccourcis pour conserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c8083-115">The conversation and folder identifiers have been shortened to preserve readability.</span></span>
  
## <a name="applyconversationaction-response-example"></a><span data-ttu-id="c8083-116">Exemple de réponse ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="c8083-116">ApplyConversationAction response example</span></span>

### <a name="description"></a><span data-ttu-id="c8083-117">Description</span><span class="sxs-lookup"><span data-stu-id="c8083-117">Description</span></span>

<span data-ttu-id="c8083-118">L’exemple suivant montre une réponse réussie à une demande **ApplyConversationAction** .</span><span class="sxs-lookup"><span data-stu-id="c8083-118">The following example shows a successful response to an **ApplyConversationAction** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c8083-119">Code</span><span class="sxs-lookup"><span data-stu-id="c8083-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="91" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ApplyConversationActionResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ApplyConversationActionResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:ApplyConversationActionResponseMessage>
      </m:ResponseMessages>
    </m:ApplyConversationActionResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="c8083-120">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c8083-120">See also</span></span>

- [<span data-ttu-id="c8083-121">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="c8083-121">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="c8083-122">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c8083-122">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="c8083-123">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c8083-123">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="c8083-124">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="c8083-124">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

