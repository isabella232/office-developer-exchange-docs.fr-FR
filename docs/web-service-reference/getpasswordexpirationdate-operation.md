---
title: Opération GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: L’opération GetPasswordExpirationDate fournit la date d’expiration de messagerie compte le mot de passe pour l’utilisateur actuel.
ms.openlocfilehash: c57942c88b09a910e2d529a12ea279bb2da5d693
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756700"
---
# <a name="getpasswordexpirationdate-operation"></a><span data-ttu-id="5dccd-103">Opération GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="5dccd-103">GetPasswordExpirationDate operation</span></span>

<span data-ttu-id="5dccd-104">L’opération **GetPasswordExpirationDate** fournit la date d’expiration de messagerie compte le mot de passe pour l’utilisateur actuel.</span><span class="sxs-lookup"><span data-stu-id="5dccd-104">The **GetPasswordExpirationDate** operation provides the email account password expiration date for the current user.</span></span> 
  
<span data-ttu-id="5dccd-105">Cette opération a été introduite dans Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5dccd-105">This operation was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a><span data-ttu-id="5dccd-106">En-têtes SOAP GetPasswordExpirationDate opération</span><span class="sxs-lookup"><span data-stu-id="5dccd-106">GetPasswordExpirationDate operation SOAP headers</span></span>

<span data-ttu-id="5dccd-107">L’opération **GetPasswordExpirationDate** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="5dccd-107">The **GetPasswordExpirationDate** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5dccd-108">**Header**</span><span class="sxs-lookup"><span data-stu-id="5dccd-108">**Header**</span></span>|<span data-ttu-id="5dccd-109">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5dccd-109">**Element**</span></span>|<span data-ttu-id="5dccd-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="5dccd-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5dccd-111">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="5dccd-111">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="5dccd-112">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="5dccd-112">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="5dccd-113">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5dccd-113">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="5dccd-114">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="5dccd-114">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5dccd-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="5dccd-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5dccd-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="5dccd-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5dccd-117">Identifie le schéma de la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="5dccd-117">Identifies the schema for the operation request.</span></span> <span data-ttu-id="5dccd-118">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="5dccd-118">This is applicable to a request.</span></span> <span data-ttu-id="5dccd-119">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="5dccd-119">This is applicable to a request.</span></span>  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a><span data-ttu-id="5dccd-120">Exemple de requête d’opération GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="5dccd-120">GetPasswordExpirationDate operation request example</span></span>

### <a name="description"></a><span data-ttu-id="5dccd-121">Description</span><span class="sxs-lookup"><span data-stu-id="5dccd-121">Description</span></span>

<span data-ttu-id="5dccd-122">Une demande d’opération **GetPasswordExpirationDate** l’exemple suivant montre comment obtenir la date d’expiration de mot de passe pour un compte de messagerie.</span><span class="sxs-lookup"><span data-stu-id="5dccd-122">The following example of a **GetPasswordExpirationDate** operation request shows how to get the password expiration date for an email account.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5dccd-123">Code</span><span class="sxs-lookup"><span data-stu-id="5dccd-123">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="5dccd-124">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="5dccd-124">Request elements</span></span>

<span data-ttu-id="5dccd-125">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="5dccd-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5dccd-126">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="5dccd-126">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md)
    
- [<span data-ttu-id="5dccd-127">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5dccd-127">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a><span data-ttu-id="5dccd-128">Réponse d’opération GetPasswordExpirationDate réussie</span><span class="sxs-lookup"><span data-stu-id="5dccd-128">Successful GetPasswordExpirationDate operation response</span></span>

<span data-ttu-id="5dccd-129">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="5dccd-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5dccd-130">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="5dccd-130">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
    
- [<span data-ttu-id="5dccd-131">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="5dccd-131">PasswordExpirationDate</span></span>](passwordexpirationdate.md)
    

