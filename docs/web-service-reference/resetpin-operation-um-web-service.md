---
title: Opération ResetPIN (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: L’opération ResetPIN modifie le code confidentiel (via le mot de passe) avec une nouvelle valeur aléatoire.
ms.openlocfilehash: e6417b86ce17c0d34fe857cf1209a18972cbef63
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829146"
---
# <a name="resetpin-operation-um-web-service"></a><span data-ttu-id="8dff9-103">Opération ResetPIN (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="8dff9-103">ResetPIN operation (UM web service)</span></span>

<span data-ttu-id="8dff9-104">L’opération ResetPIN modifie le code confidentiel (via le mot de passe) avec une nouvelle valeur aléatoire.</span><span class="sxs-lookup"><span data-stu-id="8dff9-104">The ResetPIN operation changes the PIN (TUI password) to a new random value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8dff9-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="8dff9-105">Remarks</span></span>

<span data-ttu-id="8dff9-106">L’opération ResetPIN crée un nouveau code confidentiel basé sur les stratégies de code confidentiel.</span><span class="sxs-lookup"><span data-stu-id="8dff9-106">The ResetPIN operation creates a new PIN based on the PIN policies.</span></span> <span data-ttu-id="8dff9-107">Si l’opération réussit, un message électronique qui contient le nouveau code confidentiel est envoyé à la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8dff9-107">If the operation is successful, an e-mail message that contains the new PIN is sent to the mailbox of the user.</span></span> <span data-ttu-id="8dff9-108">Si l’opération échoue, elle lève une exception qui contient des informations sur l’échec.</span><span class="sxs-lookup"><span data-stu-id="8dff9-108">If the operation fails, it will throw an exception that contains information about the failure.</span></span>
  
## <a name="resetpin-request-example"></a><span data-ttu-id="8dff9-109">Exemple de requête ResetPIN</span><span class="sxs-lookup"><span data-stu-id="8dff9-109">ResetPIN request example</span></span>

### <a name="description"></a><span data-ttu-id="8dff9-110">Description</span><span class="sxs-lookup"><span data-stu-id="8dff9-110">Description</span></span>

<span data-ttu-id="8dff9-111">L’exemple suivant d’une demande ResetPIN montre comment former une demande pour réinitialiser le code confidentiel pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8dff9-111">The following example of a ResetPIN request shows how to form a request to reset the PIN for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="8dff9-112">Code</span><span class="sxs-lookup"><span data-stu-id="8dff9-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a><span data-ttu-id="8dff9-113">Exemple de réponse ResetPIN réussie</span><span class="sxs-lookup"><span data-stu-id="8dff9-113">Successful ResetPIN response example</span></span>

### <a name="description"></a><span data-ttu-id="8dff9-114">Description</span><span class="sxs-lookup"><span data-stu-id="8dff9-114">Description</span></span>

<span data-ttu-id="8dff9-115">Une réponse ResetPIN l’exemple suivant montre une réponse à la demande ResetPIN.</span><span class="sxs-lookup"><span data-stu-id="8dff9-115">The following example of a ResetPIN response shows a response to the ResetPIN request.</span></span>
  
### <a name="code"></a><span data-ttu-id="8dff9-116">Code</span><span class="sxs-lookup"><span data-stu-id="8dff9-116">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="8dff9-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8dff9-117">See also</span></span>



[<span data-ttu-id="8dff9-118">ResetPIN (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="8dff9-118">ResetPIN (UM web service)</span></span>](resetpin-um-web-service.md)
  
[<span data-ttu-id="8dff9-119">ResetPINResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="8dff9-119">ResetPINResponse (UM web service)</span></span>](resetpinresponse-um-web-service.md)

