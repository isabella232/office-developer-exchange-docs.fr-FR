---
title: Opération GetReminders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: Trouvez des informations sur l’opération EWS GetReminders.
ms.openlocfilehash: dcbe20c674d7524a7776d374fa6964899abf472f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458305"
---
# <a name="getreminders-operation"></a><span data-ttu-id="c18c8-103">Opération GetReminders</span><span class="sxs-lookup"><span data-stu-id="c18c8-103">GetReminders operation</span></span>

<span data-ttu-id="c18c8-104">Trouvez des informations sur l’opération EWS **GetReminders** .</span><span class="sxs-lookup"><span data-stu-id="c18c8-104">Find information about the **GetReminders** EWS operation.</span></span> 
  
<span data-ttu-id="c18c8-105">L’opération **GetReminders** les services Web Exchange (EWS) récupère les rappels pour les éléments de calendrier et de tâche.</span><span class="sxs-lookup"><span data-stu-id="c18c8-105">The **GetReminders** Exchange Web Services (EWS) operation retrieves reminders for calendar and task items.</span></span> 
  
<span data-ttu-id="c18c8-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c18c8-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getreminders-operation"></a><span data-ttu-id="c18c8-107">Utilisation de l’opération GetReminders</span><span class="sxs-lookup"><span data-stu-id="c18c8-107">Using the GetReminders operation</span></span>

<span data-ttu-id="c18c8-108">L’opération **GetReminders** obtient des rappels pour les éléments de calendrier et de tâche actuels et futurs dans la boîte aux lettres de l’utilisateur, en fonction des valeurs d’élément transmises dans la demande.</span><span class="sxs-lookup"><span data-stu-id="c18c8-108">The **GetReminders** operation gets reminders for current and future calendar and task items in the user's mailbox, depending on the element values passed in the request.</span></span> <span data-ttu-id="c18c8-109">L’opération peut récupérer tous les éléments de calendrier actuels et futurs, ainsi que les tâches qui ont un rappel défini.</span><span class="sxs-lookup"><span data-stu-id="c18c8-109">The operation can retrieve all current and future calendar items as well as tasks that have a reminder set.</span></span> <span data-ttu-id="c18c8-110">Les éléments de calendrier privés sont inclus dans les réponses.</span><span class="sxs-lookup"><span data-stu-id="c18c8-110">Private calendar items are included in responses.</span></span> <span data-ttu-id="c18c8-111">Les tâches sans rappel ne sont pas incluses dans les réponses, ni dans les messages avec des rappels ou avec des indicateurs de suivi.</span><span class="sxs-lookup"><span data-stu-id="c18c8-111">Tasks without reminders are not included in responses, nor are emails with reminders or follow up flags.</span></span> 
  
<span data-ttu-id="c18c8-112">Pour récupérer tous les rappels en cours, nous vous recommandons de définir [ReminderType](remindertype.md) sur **All** [et l’heure](endtime-remindermessagedatatype.md) de fin sur l’heure actuelle.</span><span class="sxs-lookup"><span data-stu-id="c18c8-112">To retrieve all current reminders, we recommend setting the [ReminderType](remindertype.md) to **All** and the [EndTime](endtime-remindermessagedatatype.md) to the current time.</span></span> 
  
<span data-ttu-id="c18c8-113">Si les éléments [BeginTime](begintime.md) et **EndTime** sont inclus dans la demande, la réponse inclut des rappels pour tous les éléments de calendrier et de tâche qui se produisent entre les ont un rappel qui se produit entre **BeginTime** et **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="c18c8-113">If the [BeginTime](begintime.md) and **EndTime** elements are included in the request, the response includes reminders for any calendar and task items that occur between have a reminder that occurs between the **BeginTime** and **EndTime**.</span></span>
  
<span data-ttu-id="c18c8-114">Le tableau suivant décrit le comportement de l’élément **ReminderType** lorsque les éléments **BeginTime** et **EndTime** sont inclus.</span><span class="sxs-lookup"><span data-stu-id="c18c8-114">The following table describes the behavior of the **ReminderType** element when the **BeginTime** and **EndTime** elements are included.</span></span> 
  
|<span data-ttu-id="c18c8-115">ReminderType \* \* valeur de l’élément \* \*</span><span class="sxs-lookup"><span data-stu-id="c18c8-115">\*\*\*\*ReminderType\*\* element value\*\*</span></span>|<span data-ttu-id="c18c8-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="c18c8-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c18c8-117">Tous</span><span class="sxs-lookup"><span data-stu-id="c18c8-117">All</span></span>  <br/> |<span data-ttu-id="c18c8-118">Rappels qui se produisent entre **BeginTime** et **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="c18c8-118">Reminders that occur between the **BeginTime** and **EndTime**.</span></span>  <br/> |
|<span data-ttu-id="c18c8-119">Current</span><span class="sxs-lookup"><span data-stu-id="c18c8-119">Current</span></span>  <br/> |<span data-ttu-id="c18c8-120">Rappels retournés par **tous**, plus rappels qui sont antérieurs à la fenêtre de temps demandée si l’événement est encore en cours, plus tous les rendez-vous, quel que soit leur âge.</span><span class="sxs-lookup"><span data-stu-id="c18c8-120">Reminders returned by **All**, plus reminders that are earlier than the requested time window if the event is still ongoing, plus all appointments regardless of age.</span></span>  <br/> |
|<span data-ttu-id="c18c8-121">Ancien</span><span class="sxs-lookup"><span data-stu-id="c18c8-121">Old</span></span>  <br/> |<span data-ttu-id="c18c8-122">Rappels renvoyés par **tous les**, moins les événements qui n’ont pas encore été terminés, moins tous les rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="c18c8-122">Reminders returned by **All**, minus events that haven't completed yet, minus all appointments.</span></span> <span data-ttu-id="c18c8-123">Les éléments **BeginTime** et **EndTime** doivent être définis pour utiliser l' **ancienne** valeur.</span><span class="sxs-lookup"><span data-stu-id="c18c8-123">The **BeginTime** and **EndTime** elements must be set to use the **Old** value.</span></span>  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a><span data-ttu-id="c18c8-124">En-têtes SOAP d’opération GetReminders</span><span class="sxs-lookup"><span data-stu-id="c18c8-124">GetReminders operation SOAP headers</span></span>

<span data-ttu-id="c18c8-125">L’opération **GetReminders** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="c18c8-125">The **GetReminders** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="c18c8-126">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="c18c8-126">**Header name**</span></span>|<span data-ttu-id="c18c8-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c18c8-127">**Element**</span></span>|<span data-ttu-id="c18c8-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="c18c8-128">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c18c8-129">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="c18c8-129">**Impersonation**</span></span> <br/> |[<span data-ttu-id="c18c8-130">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="c18c8-130">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="c18c8-131">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="c18c8-131">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="c18c8-132">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="c18c8-132">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c18c8-133">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="c18c8-133">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="c18c8-134">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="c18c8-134">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="c18c8-135">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c18c8-135">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="c18c8-136">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="c18c8-136">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c18c8-137">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="c18c8-137">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="c18c8-138">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c18c8-138">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="c18c8-139">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="c18c8-139">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="c18c8-140">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="c18c8-140">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c18c8-141">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="c18c8-141">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="c18c8-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c18c8-142">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c18c8-143">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="c18c8-143">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="c18c8-144">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="c18c8-144">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getreminders-operation-request-example"></a><span data-ttu-id="c18c8-145">Exemple de requête d’opération GetReminders</span><span class="sxs-lookup"><span data-stu-id="c18c8-145">GetReminders operation request example</span></span>

<span data-ttu-id="c18c8-146">L’exemple suivant de demande d’opération **GetReminders** indique comment récupérer les cinq premiers éléments de calendrier qui se produisent entre **BeginTime** et **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="c18c8-146">The following example of a **GetReminders** operation request shows how to retrieve the first five calendar items that occur between the **BeginTime** and **EndTime**.</span></span>
  
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
    <m:GetReminders>
      <m:EndTime>2014-04-16T21:00:00Z</m:EndTime>
      <m:ReminderType>All</m:ReminderType>
    </m:GetReminders>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c18c8-147">Le corps SOAP de requête de l’exemple contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="c18c8-147">The example request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c18c8-148">GetReminders</span><span class="sxs-lookup"><span data-stu-id="c18c8-148">GetReminders</span></span>](getreminders.md)
    
- [<span data-ttu-id="c18c8-149">EndTime</span><span class="sxs-lookup"><span data-stu-id="c18c8-149">EndTime</span></span>](endtime-remindermessagedatatype.md)
    
- [<span data-ttu-id="c18c8-150">ReminderType</span><span class="sxs-lookup"><span data-stu-id="c18c8-150">ReminderType</span></span>](remindertype.md)
    
<span data-ttu-id="c18c8-151">Le corps SOAP peut également contenir les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="c18c8-151">The SOAP body can also contain the following elements:</span></span>
  
- [<span data-ttu-id="c18c8-152">BeginTime</span><span class="sxs-lookup"><span data-stu-id="c18c8-152">BeginTime</span></span>](begintime.md)
    
- [<span data-ttu-id="c18c8-153">MaxItems</span><span class="sxs-lookup"><span data-stu-id="c18c8-153">MaxItems</span></span>](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a><span data-ttu-id="c18c8-154">Réponse de l’opération GetReminders réussie</span><span class="sxs-lookup"><span data-stu-id="c18c8-154">Successful GetReminders operation response</span></span>

<span data-ttu-id="c18c8-155">L’exemple suivant montre une réponse réussie à une demande d’opération **GetReminders** .</span><span class="sxs-lookup"><span data-stu-id="c18c8-155">The following example shows a successful response to a **GetReminders** operation request.</span></span> <span data-ttu-id="c18c8-156">La réponse contient un rappel pour l’élément de calendrier « réunion d’équipe » et un rappel pour la tâche « tâche d’envoi de notes de réunion ».</span><span class="sxs-lookup"><span data-stu-id="c18c8-156">The response contains a reminder for the "Team meeting" calendar item and a reminder for the "Task to send meeting notes" task.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c18c8-157">Les identificateurs ont été raccourcis pour conserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c18c8-157">Identifiers have been shortened to preserve readability.</span></span> 
  
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
    <GetRemindersResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Reminders>
        <Reminder xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Team meeting</Subject>
          <Location />
          <ReminderTime>2014-04-15T21:00:00Z</ReminderTime>
          <StartDate>2014-04-15T21:00:00Z</StartDate>
          <EndDate>2014-04-15T21:30:00Z</EndDate>
          <ItemId Id="vQAAAA=="
                  ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV4" />
          <RecurringMasterItemId Id="K7u5AAA=" ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV0" />
          <ReminderGroup>Calendar</ReminderGroup>
          <UID>6CF2FA62</UID>
        </Reminder>
        <Reminder xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Task to send meeting notes</Subject>
          <Location />
          <ReminderTime>2014-04-16T14:00:00Z</ReminderTime>
          <StartDate>0001-01-02T00:00:00Z</StartDate>
          <EndDate>0001-01-02T00:00:00Z</EndDate>
          <ItemId Id="vAAAAA=="
                  ChangeKey="EwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAIDg==" />
          <ReminderGroup>Task</ReminderGroup>
          <UID>vAAAAA==</UID>
        </Reminder>
      </Reminders>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="c18c8-158">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="c18c8-158">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c18c8-159">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="c18c8-159">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="c18c8-160">Reminders</span><span class="sxs-lookup"><span data-stu-id="c18c8-160">Reminders</span></span>](reminders.md)
    
- [<span data-ttu-id="c18c8-161">Reminder</span><span class="sxs-lookup"><span data-stu-id="c18c8-161">Reminder</span></span>](reminder.md)
    
- [<span data-ttu-id="c18c8-162">Subject</span><span class="sxs-lookup"><span data-stu-id="c18c8-162">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="c18c8-163">Emplacement</span><span class="sxs-lookup"><span data-stu-id="c18c8-163">Location</span></span>](location-remindermessagedatatype.md)
    
- [<span data-ttu-id="c18c8-164">ReminderTime</span><span class="sxs-lookup"><span data-stu-id="c18c8-164">ReminderTime</span></span>](remindertime.md)
    
- [<span data-ttu-id="c18c8-165">StartDate</span><span class="sxs-lookup"><span data-stu-id="c18c8-165">StartDate</span></span>](startdate.md)
    
- [<span data-ttu-id="c18c8-166">EndDate</span><span class="sxs-lookup"><span data-stu-id="c18c8-166">EndDate</span></span>](enddate-remindertype.md)
    
- [<span data-ttu-id="c18c8-167">ItemId</span><span class="sxs-lookup"><span data-stu-id="c18c8-167">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="c18c8-168">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="c18c8-168">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
    
- [<span data-ttu-id="c18c8-169">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="c18c8-169">ReminderGroup</span></span>](remindergroup.md)
    
- [<span data-ttu-id="c18c8-170">UID</span><span class="sxs-lookup"><span data-stu-id="c18c8-170">UID</span></span>](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a><span data-ttu-id="c18c8-171">Exemple de réponse d’erreur d’opération GetReminders</span><span class="sxs-lookup"><span data-stu-id="c18c8-171">GetReminders operation error response example</span></span>

<span data-ttu-id="c18c8-172">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetReminders** .</span><span class="sxs-lookup"><span data-stu-id="c18c8-172">The following example shows an error response to a **GetReminders** operation request.</span></span> <span data-ttu-id="c18c8-173">Il s’agit d’une réponse à une demande dans laquelle la date de fin était antérieure à la date de début.</span><span class="sxs-lookup"><span data-stu-id="c18c8-173">This is a response to a request in which the end date was earlier than the start date.</span></span> 
  
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
    <GetRemindersResponse ResponseClass="Error"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>EndDate is earlier than StartDate</MessageText>
      <ResponseCode>ErrorInvalidOperation</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="c18c8-174">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="c18c8-174">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c18c8-175">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="c18c8-175">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="c18c8-176">MessageText</span><span class="sxs-lookup"><span data-stu-id="c18c8-176">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c18c8-177">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c18c8-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c18c8-178">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c18c8-178">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="c18c8-179">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="c18c8-179">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="c18c8-180">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c18c8-180">See also</span></span>


- [<span data-ttu-id="c18c8-181">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="c18c8-181">PerformReminderAction</span></span>](performreminderaction.md)
    

