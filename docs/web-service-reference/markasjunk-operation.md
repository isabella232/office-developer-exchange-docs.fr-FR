---
title: MarkAsJunk Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Opération de recherche plus d’informations sur la MarkAsJunk EWS.
ms.openlocfilehash: b9d79e6fbec87ce41030b4981f3c16f2f9ce9507
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828353"
---
# <a name="markasjunk-operation"></a><span data-ttu-id="2f8c2-103">MarkAsJunk Operation</span><span class="sxs-lookup"><span data-stu-id="2f8c2-103">MarkAsJunk operation</span></span>

<span data-ttu-id="2f8c2-104">Trouvez des informations sur l’opération EWS **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="2f8c2-104">Find information about the **MarkAsJunk** EWS operation.</span></span> 
  
<span data-ttu-id="2f8c2-105">L’opération **MarkAsJunk** ajoute et supprime les utilisateurs de la liste de courrier électronique bloqué et déplace les messages électroniques vers le dossier courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-105">The **MarkAsJunk** operation adds and removes users from the blocked email list and moves email messages to the Junk Email folder.</span></span> 
  
<span data-ttu-id="2f8c2-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markasjunk-operation"></a><span data-ttu-id="2f8c2-107">Utilisation de l’opération MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="2f8c2-107">Using the MarkAsJunk operation</span></span>

<span data-ttu-id="2f8c2-108">L’opération **MarkAsJunk** contient deux options de type Boolean pour indiquer si un expéditeur de courrier électronique doit être ajouté à la liste des expéditeurs bloqués et si le message électronique cible doit être déplacé vers le dossier de courrier indésirable par défaut ou le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-108">The **MarkAsJunk** operation contains two Boolean options to indicate whether an email sender should be added to the blocked sender list and whether the target email message should be moved to the default Junk Email folder or the Inbox folder.</span></span> <span data-ttu-id="2f8c2-109">Les actions sont déterminées par les valeurs des attributs **IsJunk** et **MoveItem** .</span><span class="sxs-lookup"><span data-stu-id="2f8c2-109">The actions are determined by the values of the **IsJunk** and **MoveItem** attributes.</span></span> <span data-ttu-id="2f8c2-110">Basée sur les combinaisons de valeurs pour les attributs **IsJunk** et **MoveItem** actions possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="2f8c2-110">The following are the possible actions based on the value combinations for the **IsJunk** and **MoveItem** attributes:</span></span> 
  
- <span data-ttu-id="2f8c2-111">Si l’attribut **IsJunk** est défini sur **true**, et l’attribut **MoveItem** est défini sur **true**, l’expéditeur du message électronique cible est ajouté à la liste des expéditeurs bloqués et le message électronique est déplacé vers le dossier Dmail indésirable.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-111">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **true**, the sender of the target email message is added to the blocked sender list and the email message is moved to the Junk Dmail folder.</span></span>
    
- <span data-ttu-id="2f8c2-112">Si l’attribut **IsJunk** est défini sur **true**, et l’attribut **MoveItem** est défini sur **false**, l’expéditeur du message électronique cible est ajouté à la liste des expéditeurs bloqués et le message électronique n’est pas déplacé à partir du dossier.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-112">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is added to the blocked sender list and the email message is not moved from the folder.</span></span>
    
- <span data-ttu-id="2f8c2-113">Si l’attribut **IsJunk** a la valeur **false**et la **MoveItem** attribut est défini sur **true**, l’expéditeur de le messageis de messagerie cible supprimé de la liste des expéditeurs bloqués et le message électronique est déplacé vers le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-113">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **true**, the sender of the target email messageis removed from the blocked sender list and the email message is moved to the Inbox folder.</span></span>
    
- <span data-ttu-id="2f8c2-114">Si l’attribut **IsJunk** est défini sur **false**, et l’attribut **MoveItem** est défini sur **false**, l’expéditeur du message électronique cible est supprimé de la liste des expéditeurs bloqués et le message électronique n’est pas déplacé à partir du dossier.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-114">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is removed from the blocked sender list and the email message is not moved from the folder.</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="2f8c2-115">Le contenu de la liste des expéditeurs bloqués n’est pas accessibles à partir de EWS.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-115">The contents of the blocked sender list are not discoverable from EWS.</span></span> <span data-ttu-id="2f8c2-116">Si un expéditeur est ajouté à la liste des expéditeurs bloqués, vous devez conserver une copie d’un message électronique envoyé par l’expéditeur bloqué à débloquer l’expéditeur à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-116">If a sender is added to the blocked sender list, you need to keep a copy of an email message sent by the blocked sender to unblock the sender in the future.</span></span> 
  
### <a name="markasjunk-operation-soap-headers"></a><span data-ttu-id="2f8c2-117">En-têtes SOAP MarkAsJunk opération</span><span class="sxs-lookup"><span data-stu-id="2f8c2-117">MarkAsJunk operation SOAP headers</span></span>

<span data-ttu-id="2f8c2-118">L’opération **MarkAsJunk** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-118">The **MarkAsJunk** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="2f8c2-119">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="2f8c2-119">**Header name**</span></span>|<span data-ttu-id="2f8c2-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2f8c2-120">**Element**</span></span>|<span data-ttu-id="2f8c2-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="2f8c2-121">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2f8c2-122">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="2f8c2-122">**Impersonation**</span></span> <br/> |[<span data-ttu-id="2f8c2-123">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="2f8c2-123">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="2f8c2-124">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-124">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="2f8c2-125">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2f8c2-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="2f8c2-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="2f8c2-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="2f8c2-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="2f8c2-128">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="2f8c2-129">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2f8c2-130">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="2f8c2-130">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="2f8c2-131">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="2f8c2-131">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="2f8c2-132">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-132">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="2f8c2-133">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-133">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2f8c2-134">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="2f8c2-134">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="2f8c2-135">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2f8c2-135">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="2f8c2-136">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-136">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="2f8c2-137">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-137">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a><span data-ttu-id="2f8c2-138">Exemple de requête d’opération MarkAsJunk : ajouter un expéditeur à la liste des expéditeurs bloqués</span><span class="sxs-lookup"><span data-stu-id="2f8c2-138">MarkAsJunk operation request example: Add a sender to the blocked sender list</span></span>

<span data-ttu-id="2f8c2-139">Une demande d’opération **MarkAsJunk** l’exemple suivant montre comment ajouter l’expéditeur d’un message électronique à la liste des expéditeurs bloqués et déplacer le courrier électronique vers le dossier courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-139">The following example of a **MarkAsJunk** operation request shows how to add the sender of an email to the blocked sender list and move the email to the junk mail folder.</span></span> <span data-ttu-id="2f8c2-140">L’opération **MarkAsJunk** accepte l’identificateur de message électronique unique pour identifier le courrier électronique qui est utilisé pour faire référence à l’expéditeur est ajouté à la liste des expéditeurs bloqués.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-140">The **MarkAsJunk** operation accepts the unique email message identifier to identify the email that is used to reference the sender that is added to the blocked sender list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2f8c2-141">Tous les identificateurs d’article et modifier des clés dans cet article ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-141">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
        <t:RequestServerVersion Version="Exchange2013" />
    </soap:Header>
    <soap:Body>
        <m:MarkAsJunk IsJunk="true" MoveItem="true">
            <m:ItemIds>
                <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYA" />
            </m:ItemIds>
        </m:MarkAsJunk>
    </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="2f8c2-142">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="2f8c2-142">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2f8c2-143">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="2f8c2-143">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="2f8c2-144">ItemId</span><span class="sxs-lookup"><span data-stu-id="2f8c2-144">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="2f8c2-145">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="2f8c2-145">ItemId</span></span>](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a><span data-ttu-id="2f8c2-146">Réponse d’opération MarkAsJunk réussie</span><span class="sxs-lookup"><span data-stu-id="2f8c2-146">Successful MarkAsJunk operation response</span></span>

<span data-ttu-id="2f8c2-147">L’exemple suivant montre une réponse positive à une demande d’opération **MarkAsJunk** pour ajouter un expéditeur à la liste des expéditeurs bloqués et de déplacer le message vers le dossier courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-147">The following example shows a successful response to a **MarkAsJunk** operation request to add a sender to the blocked sender list and move the email message to the Junk Email folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                             MinorVersion="0" 
                             MajorBuildNumber="545" 
                             MinorBuildNumber="11" 
                             Version="Exchange2013" 
                             xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                             xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
        <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
           <m:ResponseMessages>
               <m:MarkAsJunkResponseMessage ResponseClass="Success">
                  <m:ResponseCode>NoError</m:ResponseCode>
                 <m:MovedItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
               </m:MarkAsJunkResponseMessage>
           </m:ResponseMessages>
        </m:MarkAsJunkResponse>
    </s:Body>
</s:Envelope>
```

<span data-ttu-id="2f8c2-148">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="2f8c2-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2f8c2-149">MarkAsJunkResponse</span><span class="sxs-lookup"><span data-stu-id="2f8c2-149">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="2f8c2-150">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2f8c2-150">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2f8c2-151">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2f8c2-151">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="2f8c2-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2f8c2-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2f8c2-153">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="2f8c2-153">MovedItemId</span></span>](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a><span data-ttu-id="2f8c2-154">Exemple de requête d’opération MarkAsJunk : supprimer un expéditeur de la liste des expéditeurs bloqués</span><span class="sxs-lookup"><span data-stu-id="2f8c2-154">MarkAsJunk operation request example: Remove a sender from the blocked sender list</span></span>

<span data-ttu-id="2f8c2-155">Une demande d’opération **MarkAsJunk** l’exemple suivant montre comment supprimer l’expéditeur d’un message électronique à partir de la liste des expéditeurs bloqués et de déplacer le message électronique vers le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-155">The following example of a **MarkAsJunk** operation request shows how to remove the sender of an email message from the blocked sender list and move the email message to the Inbox folder.</span></span> <span data-ttu-id="2f8c2-156">Vous devez conserver un message électronique envoyé par l’expéditeur bloqué pour supprimer l’expéditeur de la liste des expéditeurs bloqués.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-156">You need to keep an email message sent by the blocked sender to remove the sender from the blocked sender list.</span></span> <span data-ttu-id="2f8c2-157">Adresse de messagerie de l’expéditeur est associé à des messages électroniques qui ont été envoyés par l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-157">The sender's email address is associated with email messages that have been sent by the sender.</span></span> <span data-ttu-id="2f8c2-158">Suppression d’un expéditeur dans la liste des expéditeurs bloqués ne fonctionnera pas si le message électronique de référence n’existe plus dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-158">Removing a sender from the blocked sender list will not succeed if the reference email message no longer exists in the user's mailbox.</span></span> <span data-ttu-id="2f8c2-159">L’identificateur d’élément utilisé pour associer un message électronique à l’expéditeur doit être associé à un élément qui existe dans la boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-159">The item identifier used to associate an email message with its sender must be associated with an item that exists in the Exchange mailbox.</span></span> <span data-ttu-id="2f8c2-160">Nous vous conseillons de créer un dossier masqué pour stocker les éléments envoyés par des expéditeurs bloqués précédemment afin que les expéditeurs peuvent être non bloqués à partir de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-160">We recommend that you create a hidden folder to store items sent by previously blocked senders so that the senders can be unblocked from the client application.</span></span> <span data-ttu-id="2f8c2-161">Dans le cas où un élément est supprimé de la boîte aux lettres Exchange, un administrateur doit utiliser la Console de gestion Exchange pour accéder à la liste des expéditeurs bloqués pour supprimer un expéditeur de la liste.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-161">In the event that an item has been removed from the Exchange mailbox, an administrator has to use the Exchange Management Console to access the blocked sender list to remove a sender from the list.</span></span> <span data-ttu-id="2f8c2-162">Pour plus d’informations sur comment débloquer un utilisateur à l’aide de la Console de gestion Exchange, voir [comment configurer l’expéditeurs fiables et expéditeurs bloqués dans Office 365](http://support.microsoft.com/kb/2545137).</span><span class="sxs-lookup"><span data-stu-id="2f8c2-162">For information about how to unblock a user by using the Exchange Management Console, see [How to configure the safe senders and blocked senders settings in Office 365](http://support.microsoft.com/kb/2545137).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
    </soap:Header>
    <soap:Body>
      <m:MarkAsJunk IsJunk="false" MoveItem="true">
        <m:ItemIds>
          <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
        </m:ItemIds>
      </m:MarkAsJunk>
    </soap:Body>
 </soap:Envelope>

```

<span data-ttu-id="2f8c2-163">Une réponse positive de suppression d’un expéditeur dans la liste des expéditeurs bloqués est la même que la réponse à l’ajout d’un expéditeur à la liste des expéditeurs bloqués.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-163">A successful response for removing a sender from the blocked sender list is the same as the response for adding a sender to the blocked sender list.</span></span>
  
<span data-ttu-id="2f8c2-164">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="2f8c2-164">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2f8c2-165">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="2f8c2-165">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="2f8c2-166">ItemId</span><span class="sxs-lookup"><span data-stu-id="2f8c2-166">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="2f8c2-167">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="2f8c2-167">ItemId</span></span>](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a><span data-ttu-id="2f8c2-168">Réponse d’erreur d’opération MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="2f8c2-168">MarkAsJunk operation error response</span></span>

<span data-ttu-id="2f8c2-169">L’exemple suivant montre une réponse d’erreur à une demande d’opération **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="2f8c2-169">The following example shows an error response to a **MarkAsJunk** operation request.</span></span> <span data-ttu-id="2f8c2-170">Il s’agit d’une réponse à une demande pour ajouter ou supprimer un expéditeur dans la liste des expéditeurs bloqués lorsque le message électronique spécifié par l’identificateur d’élément n’existe plus dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2f8c2-170">This is a response to a request to add or remove a sender from the blocked sender list when the email message specified by the item identifier no longer exists in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="545" 
                         MinorBuildNumber="11" 
                         Version="Exchange2013" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="2f8c2-171">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="2f8c2-171">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2f8c2-172">MarkAsJunkResponse</span><span class="sxs-lookup"><span data-stu-id="2f8c2-172">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="2f8c2-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2f8c2-173">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2f8c2-174">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2f8c2-174">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="2f8c2-175">MessageText</span><span class="sxs-lookup"><span data-stu-id="2f8c2-175">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="2f8c2-176">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2f8c2-176">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2f8c2-177">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2f8c2-177">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="2f8c2-178">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2f8c2-178">See also</span></span>

- [<span data-ttu-id="2f8c2-179">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2f8c2-179">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- <span data-ttu-id="2f8c2-180">[GetItem operation](getitem-operation.md) Opération GetItem</span><span class="sxs-lookup"><span data-stu-id="2f8c2-180">[GetItem operation](getitem-operation.md) GetItem operation</span></span> 
    
- [<span data-ttu-id="2f8c2-181">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="2f8c2-181">FindItem operation</span></span>](finditem-operation.md)
    

