---
title: Opération GetReminders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: Opération de recherche plus d’informations sur la GetReminders EWS.
ms.openlocfilehash: 803dabf51b94dbd8fb01f2709a42ff59a597bfd1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756727"
---
# <a name="getreminders-operation"></a><span data-ttu-id="d5cf3-103">Opération GetReminders</span><span class="sxs-lookup"><span data-stu-id="d5cf3-103">GetReminders operation</span></span>

<span data-ttu-id="d5cf3-104">Trouvez des informations sur l’opération EWS **GetReminders** .</span><span class="sxs-lookup"><span data-stu-id="d5cf3-104">Find information about the **GetReminders** EWS operation.</span></span> 
  
<span data-ttu-id="d5cf3-105">L’opération d’Exchange Web Services (EWS) **GetReminders** récupère les rappels pour les éléments de calendrier et des tâches.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-105">The **GetReminders** Exchange Web Services (EWS) operation retrieves reminders for calendar and task items.</span></span> 
  
<span data-ttu-id="d5cf3-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getreminders-operation"></a><span data-ttu-id="d5cf3-107">Utilisation de l’opération GetReminders</span><span class="sxs-lookup"><span data-stu-id="d5cf3-107">Using the GetReminders operation</span></span>

<span data-ttu-id="d5cf3-108">L’opération **GetReminders** Obtient les rappels pour actuel et futur de calendrier et les tâches dans la boîte aux lettres de l’utilisateur, selon les valeurs des éléments transmis dans la demande.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-108">The **GetReminders** operation gets reminders for current and future calendar and task items in the user's mailbox, depending on the element values passed in the request.</span></span> <span data-ttu-id="d5cf3-109">L’opération peut récupérer tous les éléments de calendrier actuels et futurs ainsi que les tâches qui ont un rappel à définir.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-109">The operation can retrieve all current and future calendar items as well as tasks that have a reminder set.</span></span> <span data-ttu-id="d5cf3-110">Éléments de calendrier privés sont inclus dans les réponses.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-110">Private calendar items are included in responses.</span></span> <span data-ttu-id="d5cf3-111">Tâches sans rappels ne sont pas inclus dans les réponses, ni sont des messages électroniques avec des rappels ou les indicateurs de suivi.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-111">Tasks without reminders are not included in responses, nor are emails with reminders or follow up flags.</span></span> 
  
<span data-ttu-id="d5cf3-112">Pour récupérer tous les rappels actifs, nous vous recommandons de définir la [ReminderType](remindertype.md) pour **toutes les** et l' [heure de fin](endtime-remindermessagedatatype.md) à l’heure actuelle.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-112">To retrieve all current reminders, we recommend setting the [ReminderType](remindertype.md) to **All** and the [EndTime](endtime-remindermessagedatatype.md) to the current time.</span></span> 
  
<span data-ttu-id="d5cf3-113">Si les éléments [BeginTime](begintime.md) et **EndTime** sont inclus dans la demande, la réponse inclut des rappels pour n’importe quel calendrier et éléments de tâche qui se produisent entre possèdent un rappel qui se produit entre le **BeginTime** et de **fin**.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-113">If the [BeginTime](begintime.md) and **EndTime** elements are included in the request, the response includes reminders for any calendar and task items that occur between have a reminder that occurs between the **BeginTime** and **EndTime**.</span></span>
  
<span data-ttu-id="d5cf3-114">Le tableau suivant décrit le comportement de l’élément **ReminderType** lorsque les éléments **BeginTime** et **l’heure de fin** sont inclus.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-114">The following table describes the behavior of the **ReminderType** element when the **BeginTime** and **EndTime** elements are included.</span></span> 
  
|<span data-ttu-id="d5cf3-115">** ReminderType élément valeur **</span><span class="sxs-lookup"><span data-stu-id="d5cf3-115">****ReminderType** element value**</span></span>|<span data-ttu-id="d5cf3-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="d5cf3-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d5cf3-117">Tous</span><span class="sxs-lookup"><span data-stu-id="d5cf3-117">All</span></span>  <br/> |<span data-ttu-id="d5cf3-118">Rappels qui se produisent entre le **BeginTime** et de **fin**.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-118">Reminders that occur between the **BeginTime** and **EndTime**.</span></span>  <br/> |
|<span data-ttu-id="d5cf3-119">En cours</span><span class="sxs-lookup"><span data-stu-id="d5cf3-119">Current</span></span>  <br/> |<span data-ttu-id="d5cf3-120">Rappels renvoyés par **tous les**, ainsi que les rappels qui sont antérieurs à la fenêtre de temps demandé, s’il est toujours en cours, ainsi que tous les rendez-vous, quel que soit l’âge.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-120">Reminders returned by **All**, plus reminders that are earlier than the requested time window if the event is still ongoing, plus all appointments regardless of age.</span></span>  <br/> |
|<span data-ttu-id="d5cf3-121">Ancienne</span><span class="sxs-lookup"><span data-stu-id="d5cf3-121">Old</span></span>  <br/> |<span data-ttu-id="d5cf3-122">Rappels retournées par **tous les**, moins les événements qui ne sont pas terminées, moins tous les rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-122">Reminders returned by **All**, minus events that haven't completed yet, minus all appointments.</span></span> <span data-ttu-id="d5cf3-123">Les éléments **BeginTime** et **l’heure de fin** doivent être définies à utiliser **l’ancienne** valeur.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-123">The **BeginTime** and **EndTime** elements must be set to use the **Old** value.</span></span>  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a><span data-ttu-id="d5cf3-124">En-têtes SOAP GetReminders opération</span><span class="sxs-lookup"><span data-stu-id="d5cf3-124">GetReminders operation SOAP headers</span></span>

<span data-ttu-id="d5cf3-125">L’opération **GetReminders** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-125">The **GetReminders** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d5cf3-126">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="d5cf3-126">**Header name**</span></span>|<span data-ttu-id="d5cf3-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d5cf3-127">**Element**</span></span>|<span data-ttu-id="d5cf3-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="d5cf3-128">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d5cf3-129">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="d5cf3-129">**Impersonation**</span></span> <br/> |[<span data-ttu-id="d5cf3-130">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="d5cf3-130">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="d5cf3-131">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-131">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="d5cf3-132">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-132">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d5cf3-133">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="d5cf3-133">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="d5cf3-134">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="d5cf3-134">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="d5cf3-135">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-135">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="d5cf3-136">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-136">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d5cf3-137">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d5cf3-137">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d5cf3-138">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d5cf3-138">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d5cf3-139">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-139">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d5cf3-140">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-140">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d5cf3-141">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d5cf3-141">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d5cf3-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d5cf3-142">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d5cf3-143">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-143">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d5cf3-144">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-144">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getreminders-operation-request-example"></a><span data-ttu-id="d5cf3-145">Exemple de requête d’opération GetReminders</span><span class="sxs-lookup"><span data-stu-id="d5cf3-145">GetReminders operation request example</span></span>

<span data-ttu-id="d5cf3-146">Une demande d’opération **GetReminders** l’exemple suivant montre comment extraire les éléments de cinq calendrier premier qui se produisent entre le **BeginTime** et de **fin**.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-146">The following example of a **GetReminders** operation request shows how to retrieve the first five calendar items that occur between the **BeginTime** and **EndTime**.</span></span>
  
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
    <m:GetReminders>
      <m:EndTime>2014-04-16T21:00:00Z</m:EndTime>
      <m:ReminderType>All</m:ReminderType>
    </m:GetReminders>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d5cf3-147">L’exemple de demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d5cf3-147">The example request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d5cf3-148">GetReminders</span><span class="sxs-lookup"><span data-stu-id="d5cf3-148">GetReminders</span></span>](getreminders.md)
    
- [<span data-ttu-id="d5cf3-149">Heure de fin</span><span class="sxs-lookup"><span data-stu-id="d5cf3-149">EndTime</span></span>](endtime-remindermessagedatatype.md)
    
- [<span data-ttu-id="d5cf3-150">ReminderType</span><span class="sxs-lookup"><span data-stu-id="d5cf3-150">ReminderType</span></span>](remindertype.md)
    
<span data-ttu-id="d5cf3-151">Le corps SOAP peut également contenir les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d5cf3-151">The SOAP body can also contain the following elements:</span></span>
  
- [<span data-ttu-id="d5cf3-152">BeginTime</span><span class="sxs-lookup"><span data-stu-id="d5cf3-152">BeginTime</span></span>](begintime.md)
    
- [<span data-ttu-id="d5cf3-153">MaxItems</span><span class="sxs-lookup"><span data-stu-id="d5cf3-153">MaxItems</span></span>](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a><span data-ttu-id="d5cf3-154">Réponse d’opération GetReminders réussie</span><span class="sxs-lookup"><span data-stu-id="d5cf3-154">Successful GetReminders operation response</span></span>

<span data-ttu-id="d5cf3-155">L’exemple suivant montre une réponse positive à une demande d’opération **GetReminders** .</span><span class="sxs-lookup"><span data-stu-id="d5cf3-155">The following example shows a successful response to a **GetReminders** operation request.</span></span> <span data-ttu-id="d5cf3-156">La réponse contient un rappel pour l’élément de calendrier « Réunion d’équipe » et un rappel pour la tâche « Tâches pour envoyer des notes de réunion ».</span><span class="sxs-lookup"><span data-stu-id="d5cf3-156">The response contains a reminder for the "Team meeting" calendar item and a reminder for the "Task to send meeting notes" task.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d5cf3-157">Les identificateurs ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-157">Identifiers have been shortened to preserve readability.</span></span> 
  
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
    <GetRemindersResponse ResponseClass="Success"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Reminders>
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="d5cf3-158">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d5cf3-158">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d5cf3-159">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="d5cf3-159">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="d5cf3-160">Rappels</span><span class="sxs-lookup"><span data-stu-id="d5cf3-160">Reminders</span></span>](reminders.md)
    
- [<span data-ttu-id="d5cf3-161">Rappel</span><span class="sxs-lookup"><span data-stu-id="d5cf3-161">Reminder</span></span>](reminder.md)
    
- [<span data-ttu-id="d5cf3-162">Objet</span><span class="sxs-lookup"><span data-stu-id="d5cf3-162">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="d5cf3-163">Location</span><span class="sxs-lookup"><span data-stu-id="d5cf3-163">Location</span></span>](location-remindermessagedatatype.md)
    
- [<span data-ttu-id="d5cf3-164">ReminderTime</span><span class="sxs-lookup"><span data-stu-id="d5cf3-164">ReminderTime</span></span>](remindertime.md)
    
- [<span data-ttu-id="d5cf3-165">Date de début</span><span class="sxs-lookup"><span data-stu-id="d5cf3-165">StartDate</span></span>](startdate.md)
    
- [<span data-ttu-id="d5cf3-166">Date de fin</span><span class="sxs-lookup"><span data-stu-id="d5cf3-166">EndDate</span></span>](enddate-remindertype.md)
    
- [<span data-ttu-id="d5cf3-167">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="d5cf3-167">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="d5cf3-168">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="d5cf3-168">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
    
- [<span data-ttu-id="d5cf3-169">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="d5cf3-169">ReminderGroup</span></span>](remindergroup.md)
    
- [<span data-ttu-id="d5cf3-170">UID</span><span class="sxs-lookup"><span data-stu-id="d5cf3-170">UID</span></span>](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a><span data-ttu-id="d5cf3-171">Exemple de réponse d’erreur opération GetReminders</span><span class="sxs-lookup"><span data-stu-id="d5cf3-171">GetReminders operation error response example</span></span>

<span data-ttu-id="d5cf3-172">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetReminders** .</span><span class="sxs-lookup"><span data-stu-id="d5cf3-172">The following example shows an error response to a **GetReminders** operation request.</span></span> <span data-ttu-id="d5cf3-173">Il s’agit d’une réponse à une demande dans laquelle la date de fin est antérieure à la date de début.</span><span class="sxs-lookup"><span data-stu-id="d5cf3-173">This is a response to a request in which the end date was earlier than the start date.</span></span> 
  
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
    <GetRemindersResponse ResponseClass="Error"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>EndDate is earlier than StartDate</MessageText>
      <ResponseCode>ErrorInvalidOperation</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="d5cf3-174">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d5cf3-174">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d5cf3-175">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="d5cf3-175">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="d5cf3-176">MessageText</span><span class="sxs-lookup"><span data-stu-id="d5cf3-176">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d5cf3-177">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d5cf3-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d5cf3-178">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d5cf3-178">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="d5cf3-179">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="d5cf3-179">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d5cf3-180">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d5cf3-180">See also</span></span>


- [<span data-ttu-id="d5cf3-181">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="d5cf3-181">PerformReminderAction</span></span>](performreminderaction.md)
    

