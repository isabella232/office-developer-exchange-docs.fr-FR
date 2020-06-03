---
title: Opération ResetPIN (service Web de messagerie unifiée)
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
description: L’opération ResetPIN modifie le code confidentiel (mot de passe de la TUI) en une nouvelle valeur aléatoire.
ms.openlocfilehash: 8de64ce7a47e9c426f8eb9298e1ca00508fb616c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465491"
---
# <a name="resetpin-operation-um-web-service"></a><span data-ttu-id="e8cbf-103">Opération ResetPIN (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="e8cbf-103">ResetPIN operation (UM web service)</span></span>

<span data-ttu-id="e8cbf-104">L’opération ResetPIN modifie le code confidentiel (mot de passe de la TUI) en une nouvelle valeur aléatoire.</span><span class="sxs-lookup"><span data-stu-id="e8cbf-104">The ResetPIN operation changes the PIN (TUI password) to a new random value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8cbf-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="e8cbf-105">Remarks</span></span>

<span data-ttu-id="e8cbf-106">L’opération ResetPIN crée un nouveau code confidentiel basé sur les stratégies de code confidentiel.</span><span class="sxs-lookup"><span data-stu-id="e8cbf-106">The ResetPIN operation creates a new PIN based on the PIN policies.</span></span> <span data-ttu-id="e8cbf-107">Si l’opération réussit, un message électronique contenant le nouveau code confidentiel est envoyé à la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e8cbf-107">If the operation is successful, an e-mail message that contains the new PIN is sent to the mailbox of the user.</span></span> <span data-ttu-id="e8cbf-108">Si l’opération échoue, elle génère une exception qui contient des informations sur l’échec.</span><span class="sxs-lookup"><span data-stu-id="e8cbf-108">If the operation fails, it will throw an exception that contains information about the failure.</span></span>
  
## <a name="resetpin-request-example"></a><span data-ttu-id="e8cbf-109">Exemple de requête ResetPIN</span><span class="sxs-lookup"><span data-stu-id="e8cbf-109">ResetPIN request example</span></span>

### <a name="description"></a><span data-ttu-id="e8cbf-110">Description</span><span class="sxs-lookup"><span data-stu-id="e8cbf-110">Description</span></span>

<span data-ttu-id="e8cbf-111">L’exemple de requête ResetPIN suivant indique comment créer une demande de réinitialisation du code confidentiel d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e8cbf-111">The following example of a ResetPIN request shows how to form a request to reset the PIN for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="e8cbf-112">Code</span><span class="sxs-lookup"><span data-stu-id="e8cbf-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a><span data-ttu-id="e8cbf-113">Exemple de réponse ResetPIN réussi</span><span class="sxs-lookup"><span data-stu-id="e8cbf-113">Successful ResetPIN response example</span></span>

### <a name="description"></a><span data-ttu-id="e8cbf-114">Description</span><span class="sxs-lookup"><span data-stu-id="e8cbf-114">Description</span></span>

<span data-ttu-id="e8cbf-115">L’exemple suivant de réponse ResetPIN indique une réponse à la demande ResetPIN.</span><span class="sxs-lookup"><span data-stu-id="e8cbf-115">The following example of a ResetPIN response shows a response to the ResetPIN request.</span></span>
  
### <a name="code"></a><span data-ttu-id="e8cbf-116">Code</span><span class="sxs-lookup"><span data-stu-id="e8cbf-116">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="e8cbf-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e8cbf-117">See also</span></span>



[<span data-ttu-id="e8cbf-118">ResetPIN (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="e8cbf-118">ResetPIN (UM web service)</span></span>](resetpin-um-web-service.md)
  
[<span data-ttu-id="e8cbf-119">ResetPINResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="e8cbf-119">ResetPINResponse (UM web service)</span></span>](resetpinresponse-um-web-service.md)

