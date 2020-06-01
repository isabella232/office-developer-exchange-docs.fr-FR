---
title: Opération PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Trouvez des informations sur l’opération EWS PerformReminderAction.
ms.openlocfilehash: 4c069d541e9a42167c447a50c405399958d3608d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462289"
---
# <a name="performreminderaction-operation"></a><span data-ttu-id="cc31e-103">Opération PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="cc31e-103">PerformReminderAction operation</span></span>

<span data-ttu-id="cc31e-104">Trouvez des informations sur l’opération EWS **PerformReminderAction** .</span><span class="sxs-lookup"><span data-stu-id="cc31e-104">Find information about the **PerformReminderAction** EWS operation.</span></span> 
  
<span data-ttu-id="cc31e-105">L’opération **PerformReminderAction** les services Web Exchange (EWS) lance une action de rejet ou d’exécution répétée sur un rappel.</span><span class="sxs-lookup"><span data-stu-id="cc31e-105">The **PerformReminderAction** Exchange Web Services (EWS) operation initiates a dismiss or snooze action on a reminder.</span></span> 
  
<span data-ttu-id="cc31e-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cc31e-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-performreminderaction-operation"></a><span data-ttu-id="cc31e-107">Utilisation de l’opération PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="cc31e-107">Using the PerformReminderAction operation</span></span>

<span data-ttu-id="cc31e-108">Vous pouvez utiliser l’opération **PerformReminderAction** pour ignorer ou répéter les rappels renvoyés par l’opération [GetReminders](getreminders-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="cc31e-108">You can use the **PerformReminderAction** operation to dismiss or snooze (delay) reminders returned by the [GetReminders](getreminders-operation.md) operation.</span></span> <span data-ttu-id="cc31e-109">Pour répéter un rappel, définissez le [ActionType](actiontype-reminderactiontype.md) sur **SNOOZE**et définissez la valeur [NewReminderTime](newremindertime.md) à une heure ultérieure à la [ReminderTime](remindertime.md)actuelle, sinon le **NewReminderTime** est ignoré par le serveur.</span><span class="sxs-lookup"><span data-stu-id="cc31e-109">To snooze a reminder, set the [ActionType](actiontype-reminderactiontype.md) to **Snooze**, and set the [NewReminderTime](newremindertime.md) value to a time later than the current [ReminderTime](remindertime.md), otherwise the **NewReminderTime** is ignored by the server.</span></span> <span data-ttu-id="cc31e-110">Si le rappel est destiné à une occurrence d’une réunion périodique et que l’action de **répétition** est effectuée sur le rappel avec un **NewReminderTime** qui se trouve au-delà du rappel de l’occurrence suivante, le rappel est effectivement ignoré.</span><span class="sxs-lookup"><span data-stu-id="cc31e-110">If the reminder is for an occurrence of a recurring meeting, and the **Snooze** action is taken on the reminder with a **NewReminderTime** that is past the reminder of the next occurrence, the reminder is effectively dismissed.</span></span> 
  
<span data-ttu-id="cc31e-111">Pour faire disparaître un rappel, définissez le paramètre **ActionType** sur **faire disparaître**.</span><span class="sxs-lookup"><span data-stu-id="cc31e-111">To dismiss a reminder, set the **ActionType** to **Dismiss**.</span></span> <span data-ttu-id="cc31e-112">Lorsque le serveur traite la demande, le serveur remplace la valeur [IsReminderSet](isreminderset.md) de l’élément **true** par **false**.</span><span class="sxs-lookup"><span data-stu-id="cc31e-112">When the server processes the request, the server changes the [IsReminderSet](isreminderset.md) value for the item from **True** to **False**.</span></span>
  
### <a name="performreminderaction-operation-soap-headers"></a><span data-ttu-id="cc31e-113">En-têtes SOAP d’opération PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="cc31e-113">PerformReminderAction operation SOAP headers</span></span>

<span data-ttu-id="cc31e-114">L’opération **PerformReminderAction** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="cc31e-114">The **PerformReminderAction** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="cc31e-115">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="cc31e-115">**Header name**</span></span>|<span data-ttu-id="cc31e-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cc31e-116">**Element**</span></span>|<span data-ttu-id="cc31e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="cc31e-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cc31e-118">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="cc31e-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="cc31e-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="cc31e-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="cc31e-120">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="cc31e-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="cc31e-121">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="cc31e-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cc31e-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="cc31e-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="cc31e-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="cc31e-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="cc31e-124">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cc31e-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="cc31e-125">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="cc31e-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cc31e-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="cc31e-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="cc31e-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="cc31e-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="cc31e-128">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="cc31e-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="cc31e-129">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="cc31e-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cc31e-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="cc31e-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="cc31e-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="cc31e-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="cc31e-132">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="cc31e-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="cc31e-133">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="cc31e-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a><span data-ttu-id="cc31e-134">Exemple de requête d’opération PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="cc31e-134">PerformReminderAction operation request example</span></span>

<span data-ttu-id="cc31e-135">L’exemple suivant de demande d’opération **PerformReminderAction** indique comment répéter un rappel actif et définir une nouvelle heure de rappel.</span><span class="sxs-lookup"><span data-stu-id="cc31e-135">The following example of a **PerformReminderAction** operation request shows how to snooze a current reminder and set a new reminder time.</span></span> <span data-ttu-id="cc31e-136">Notez que vous devez inclure le **ChangeKey** pour l' [ItemId](itemid.md) et que le **NewReminderTime** doit être défini à une heure ultérieure à la **ReminderTime** renvoyée par l’opération [GetReminders](getreminders-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="cc31e-136">Note that you need to include the **ChangeKey** for the [ItemId](itemid.md) and the **NewReminderTime** must be set to a time later than the **ReminderTime** returned by the [GetReminders](getreminders-operation.md) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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
> <span data-ttu-id="cc31e-137">La valeur **ItemId** a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="cc31e-137">The **ItemId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="cc31e-138">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="cc31e-138">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cc31e-139">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="cc31e-139">PerformReminderAction</span></span>](performreminderaction.md)
    
- [<span data-ttu-id="cc31e-140">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="cc31e-140">ReminderItemActions</span></span>](reminderitemactions.md)
    
- [<span data-ttu-id="cc31e-141">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="cc31e-141">ReminderItemAction</span></span>](reminderitemaction.md)
    
- [<span data-ttu-id="cc31e-142">ActionType</span><span class="sxs-lookup"><span data-stu-id="cc31e-142">ActionType</span></span>](actiontype-reminderactiontype.md)
    
- [<span data-ttu-id="cc31e-143">ItemId</span><span class="sxs-lookup"><span data-stu-id="cc31e-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="cc31e-144">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="cc31e-144">NewReminderTime</span></span>](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a><span data-ttu-id="cc31e-145">Réponse de l’opération PerformReminderAction réussie</span><span class="sxs-lookup"><span data-stu-id="cc31e-145">Successful PerformReminderAction operation response</span></span>

<span data-ttu-id="cc31e-146">L’exemple suivant montre une réponse réussie à une demande d’opération **PerformReminderAction** .</span><span class="sxs-lookup"><span data-stu-id="cc31e-146">The following example shows a successful response to a **PerformReminderAction** operation request.</span></span> <span data-ttu-id="cc31e-147">L’élément **UpdatedItemIds** contient le **ItemIds** de l’élément de calendrier mis à jour.</span><span class="sxs-lookup"><span data-stu-id="cc31e-147">The **UpdatedItemIds** element contains the **ItemIds** of the updated calendar item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="cc31e-148">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="cc31e-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cc31e-149">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="cc31e-149">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="cc31e-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cc31e-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cc31e-151">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="cc31e-151">UpdatedItemIds</span></span>](updateditemids.md)
    
- [<span data-ttu-id="cc31e-152">ItemId</span><span class="sxs-lookup"><span data-stu-id="cc31e-152">ItemId</span></span>](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a><span data-ttu-id="cc31e-153">Exemple de réponse d’erreur d’opération PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="cc31e-153">PerformReminderAction operation error response example</span></span>

<span data-ttu-id="cc31e-154">L’exemple suivant montre une réponse à une demande d’opération **PerformReminderAction** lorsqu’aucune modification n’a été apportée sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="cc31e-154">The following example shows a response to a **PerformReminderAction** operation request when no change was made on the server.</span></span> <span data-ttu-id="cc31e-155">Il s’agit d’une réponse dans laquelle une demande a été envoyée, mais aucune **UpdatedItemIds** n’a été renvoyée, ce qui signifie qu’aucun rappel n’a été modifié.</span><span class="sxs-lookup"><span data-stu-id="cc31e-155">This is a response in which a request was sent, but no **UpdatedItemIds** were returned, meaning no reminders were changed.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="cc31e-156">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="cc31e-156">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cc31e-157">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="cc31e-157">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="cc31e-158">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cc31e-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cc31e-159">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="cc31e-159">UpdatedItemIds</span></span>](updateditemids.md)
    
<span data-ttu-id="cc31e-160">Pour d’autres codes d’erreur qui sont génériques à EWS, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="cc31e-160">For additional error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="cc31e-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cc31e-161">See also</span></span>


- [<span data-ttu-id="cc31e-162">Opération GetReminders</span><span class="sxs-lookup"><span data-stu-id="cc31e-162">GetReminders operation</span></span>](getreminders-operation.md)
    

