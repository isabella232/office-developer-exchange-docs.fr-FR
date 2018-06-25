---
title: Opération PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Opération de recherche plus d’informations sur la PerformReminderAction EWS.
ms.openlocfilehash: 778fbb508413721f58cfcf9143a5296874e6cd1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828722"
---
# <a name="performreminderaction-operation"></a><span data-ttu-id="01a66-103">Opération PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="01a66-103">PerformReminderAction operation</span></span>

<span data-ttu-id="01a66-104">Trouvez des informations sur l’opération EWS **PerformReminderAction** .</span><span class="sxs-lookup"><span data-stu-id="01a66-104">Find information about the **PerformReminderAction** EWS operation.</span></span> 
  
<span data-ttu-id="01a66-105">L’opération d’Exchange Web Services (EWS) **PerformReminderAction** lance une action d’ignorer ou répéter un rappel.</span><span class="sxs-lookup"><span data-stu-id="01a66-105">The **PerformReminderAction** Exchange Web Services (EWS) operation initiates a dismiss or snooze action on a reminder.</span></span> 
  
<span data-ttu-id="01a66-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="01a66-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-performreminderaction-operation"></a><span data-ttu-id="01a66-107">Utilisation de l’opération PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="01a66-107">Using the PerformReminderAction operation</span></span>

<span data-ttu-id="01a66-108">Vous pouvez utiliser l’opération **PerformReminderAction** pour fermer ou de répéter rappels (retard) retournées par l’opération [GetReminders](getreminders-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="01a66-108">You can use the **PerformReminderAction** operation to dismiss or snooze (delay) reminders returned by the [GetReminders](getreminders-operation.md) operation.</span></span> <span data-ttu-id="01a66-109">Pour répéter un rappel, définir l' [ActionType](actiontype-reminderactiontype.md) **répétés**et définir la valeur de [NewReminderTime](newremindertime.md) à une date postérieure à la actuel [ReminderTime](remindertime.md), sinon la **NewReminderTime** est ignoré par le serveur.</span><span class="sxs-lookup"><span data-stu-id="01a66-109">To snooze a reminder, set the [ActionType](actiontype-reminderactiontype.md) to **Snooze**, and set the [NewReminderTime](newremindertime.md) value to a time later than the current [ReminderTime](remindertime.md), otherwise the **NewReminderTime** is ignored by the server.</span></span> <span data-ttu-id="01a66-110">Si le rappel est une occurrence d’une réunion périodique, et l’action **Snooze** est exécutée sur le rappel avec un **NewReminderTime** qui a passé le rappel de la prochaine occurrence, le rappel est rejeté efficacement.</span><span class="sxs-lookup"><span data-stu-id="01a66-110">If the reminder is for an occurrence of a recurring meeting, and the **Snooze** action is taken on the reminder with a **NewReminderTime** that is past the reminder of the next occurrence, the reminder is effectively dismissed.</span></span> 
  
<span data-ttu-id="01a66-111">Pour faire disparaître un rappel, définissez l' **ActionType** pour **faire disparaître**.</span><span class="sxs-lookup"><span data-stu-id="01a66-111">To dismiss a reminder, set the **ActionType** to **Dismiss**.</span></span> <span data-ttu-id="01a66-112">Lorsque le serveur traite la demande, le serveur modifie la valeur de [IsReminderSet](isreminderset.md) pour l’élément de **la valeur True** à **False**.</span><span class="sxs-lookup"><span data-stu-id="01a66-112">When the server processes the request, the server changes the [IsReminderSet](isreminderset.md) value for the item from **True** to **False**.</span></span>
  
### <a name="performreminderaction-operation-soap-headers"></a><span data-ttu-id="01a66-113">En-têtes SOAP PerformReminderAction opération</span><span class="sxs-lookup"><span data-stu-id="01a66-113">PerformReminderAction operation SOAP headers</span></span>

<span data-ttu-id="01a66-114">L’opération **PerformReminderAction** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="01a66-114">The **PerformReminderAction** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="01a66-115">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="01a66-115">**Header name**</span></span>|<span data-ttu-id="01a66-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="01a66-116">**Element**</span></span>|<span data-ttu-id="01a66-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="01a66-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="01a66-118">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="01a66-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="01a66-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="01a66-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="01a66-120">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="01a66-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="01a66-121">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="01a66-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="01a66-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="01a66-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="01a66-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="01a66-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="01a66-124">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="01a66-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="01a66-125">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="01a66-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="01a66-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="01a66-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="01a66-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="01a66-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="01a66-128">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="01a66-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="01a66-129">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="01a66-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="01a66-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="01a66-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="01a66-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="01a66-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="01a66-132">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="01a66-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="01a66-133">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="01a66-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a><span data-ttu-id="01a66-134">Exemple de requête d’opération PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="01a66-134">PerformReminderAction operation request example</span></span>

<span data-ttu-id="01a66-135">Une demande d’opération **PerformReminderAction** l’exemple suivant montre comment répéter un rappel en cours et définir une nouvelle heure du rappel.</span><span class="sxs-lookup"><span data-stu-id="01a66-135">The following example of a **PerformReminderAction** operation request shows how to snooze a current reminder and set a new reminder time.</span></span> <span data-ttu-id="01a66-136">Notez que vous devez inclure le **ChangeKey** pour l' [ID d’élément](itemid.md) et le **NewReminderTime** doit être définie à une date postérieure à la **ReminderTime** retournées par l’opération [GetReminders](getreminders-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="01a66-136">Note that you need to include the **ChangeKey** for the [ItemId](itemid.md) and the **NewReminderTime** must be set to a time later than the **ReminderTime** returned by the [GetReminders](getreminders-operation.md) operation.</span></span> 
  
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
    <m:PerformReminderAction>
      <m:ReminderItemActions>
        <t:ReminderItemAction>
          <t:ActionType>Snooze</t:ActionType>
          <t:ItemId Id="vwAAAA=="
           ChangeKey="DwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAUDA=="/>
          <t:NewReminderTime>2014-04-16T17:00:00Z</t:NewReminderTime>
        </t:ReminderItemAction>
      </m:ReminderItemActions>
    </m:PerformReminderAction>
  </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> <span data-ttu-id="01a66-137">La valeur **ItemId** a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="01a66-137">The **ItemId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="01a66-138">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="01a66-138">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="01a66-139">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="01a66-139">PerformReminderAction</span></span>](performreminderaction.md)
    
- [<span data-ttu-id="01a66-140">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="01a66-140">ReminderItemActions</span></span>](reminderitemactions.md)
    
- [<span data-ttu-id="01a66-141">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="01a66-141">ReminderItemAction</span></span>](reminderitemaction.md)
    
- [<span data-ttu-id="01a66-142">ActionType</span><span class="sxs-lookup"><span data-stu-id="01a66-142">ActionType</span></span>](actiontype-reminderactiontype.md)
    
- [<span data-ttu-id="01a66-143">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="01a66-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="01a66-144">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="01a66-144">NewReminderTime</span></span>](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a><span data-ttu-id="01a66-145">Réponse d’opération PerformReminderAction réussie</span><span class="sxs-lookup"><span data-stu-id="01a66-145">Successful PerformReminderAction operation response</span></span>

<span data-ttu-id="01a66-146">L’exemple suivant montre une réponse positive à une demande d’opération **PerformReminderAction** .</span><span class="sxs-lookup"><span data-stu-id="01a66-146">The following example shows a successful response to a **PerformReminderAction** operation request.</span></span> <span data-ttu-id="01a66-147">L’élément **UpdatedItemIds** contient les **numéros d’objet** de l’élément de calendrier mis à jour.</span><span class="sxs-lookup"><span data-stu-id="01a66-147">The **UpdatedItemIds** element contains the **ItemIds** of the updated calendar item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="01a66-148">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="01a66-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="01a66-149">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="01a66-149">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="01a66-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="01a66-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="01a66-151">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="01a66-151">UpdatedItemIds</span></span>](updateditemids.md)
    
- [<span data-ttu-id="01a66-152">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="01a66-152">ItemId</span></span>](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a><span data-ttu-id="01a66-153">Exemple de réponse d’erreur opération PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="01a66-153">PerformReminderAction operation error response example</span></span>

<span data-ttu-id="01a66-154">L’exemple suivant montre une réponse à une demande d’opération **PerformReminderAction** lorsqu’aucune modification n’a été effectuée sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="01a66-154">The following example shows a response to a **PerformReminderAction** operation request when no change was made on the server.</span></span> <span data-ttu-id="01a66-155">Il s’agit d’une réponse dans lequel une demande a été envoyée, mais aucun **UpdatedItemIds** ont été retournés, ce qui signifie aucune rappels ont été modifiées.</span><span class="sxs-lookup"><span data-stu-id="01a66-155">This is a response in which a request was sent, but no **UpdatedItemIds** were returned, meaning no reminders were changed.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="01a66-156">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="01a66-156">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="01a66-157">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="01a66-157">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="01a66-158">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="01a66-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="01a66-159">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="01a66-159">UpdatedItemIds</span></span>](updateditemids.md)
    
<span data-ttu-id="01a66-160">Pour les codes d’erreur supplémentaires qui sont génériques pour EWS, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="01a66-160">For additional error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="01a66-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="01a66-161">See also</span></span>


- [<span data-ttu-id="01a66-162">Opération GetReminders</span><span class="sxs-lookup"><span data-stu-id="01a66-162">GetReminders operation</span></span>](getreminders-operation.md)
    

