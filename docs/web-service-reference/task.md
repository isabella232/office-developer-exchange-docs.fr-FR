---
title: Tâche
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Task
api_type:
- schema
ms.assetid: 7c84927e-db28-4c5d-b0b5-cbcc2b88d869
description: L’élément de tâche représente une tâche dans la banque d’informations Exchange.
ms.openlocfilehash: 2c61fca6ac85290e34f1365b0cb9e841e1fe279f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838679"
---
# <a name="task"></a><span data-ttu-id="ed66b-103">Tâche</span><span class="sxs-lookup"><span data-stu-id="ed66b-103">Task</span></span>

<span data-ttu-id="ed66b-104">L’élément de **tâche** représente une tâche dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed66b-104">The **Task** element represents a task in the Exchange store.</span></span> 
  
```xml
<Task>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <ActualWork/>
   <AssignedTime/>
   <BillingInformation/>
   <ChangeCount/>
   <Companies/>
   <CompleteDate/>
   <Contacts/>
   <DelegationState/>
   <Delegator/>
   <DueDate/>
   <IsAssignmentEditable/>
   <IsComplete/>
   <IsRecurring/>
   <IsTeamTask/>
   <Mileage/>
   <Owner/>
   <PercentComplete/>
   <Recurrence/>
   <StartDate/>
   <Status/>
   <StatusDescription/>
   <TotalWork/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</Task>
```

<span data-ttu-id="ed66b-105">**TaskType**</span><span class="sxs-lookup"><span data-stu-id="ed66b-105">**TaskType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ed66b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ed66b-106">Attributes and elements</span></span>

<span data-ttu-id="ed66b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ed66b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed66b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ed66b-108">Attributes</span></span>

<span data-ttu-id="ed66b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ed66b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed66b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ed66b-110">Child elements</span></span>

|<span data-ttu-id="ed66b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ed66b-111">**Element**</span></span>|<span data-ttu-id="ed66b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ed66b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed66b-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="ed66b-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="ed66b-114">Contient le flux MIME (Multipurpose Internet Mail Extensions) natif d'un objet représenté au format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="ed66b-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-115">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="ed66b-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ed66b-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed66b-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ed66b-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ed66b-118">Représente l'identificateur du dossier parent qui contient l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="ed66b-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="ed66b-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="ed66b-120">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="ed66b-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-121">Objet</span><span class="sxs-lookup"><span data-stu-id="ed66b-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="ed66b-122">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="ed66b-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="ed66b-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="ed66b-124">Contient l’état de la sensibilité d’un élément.</span><span class="sxs-lookup"><span data-stu-id="ed66b-124">Contains the status for an item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-125">Corps</span><span class="sxs-lookup"><span data-stu-id="ed66b-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="ed66b-126">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="ed66b-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-127">Attachments</span><span class="sxs-lookup"><span data-stu-id="ed66b-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ed66b-128">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed66b-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="ed66b-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="ed66b-130">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="ed66b-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-131">Taille</span><span class="sxs-lookup"><span data-stu-id="ed66b-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="ed66b-132">Représente la taille, en octets, d’un élément.</span><span class="sxs-lookup"><span data-stu-id="ed66b-132">Represents the size, in bytes, of an item.</span></span> <span data-ttu-id="ed66b-133">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="ed66b-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-134">Categories</span><span class="sxs-lookup"><span data-stu-id="ed66b-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ed66b-135">Représente une collection de chaînes qui identifie les catégories auxquelles un élément de la boîte aux lettres appartient.</span><span class="sxs-lookup"><span data-stu-id="ed66b-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-136">Importance</span><span class="sxs-lookup"><span data-stu-id="ed66b-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="ed66b-137">Décrit l'importance d'un élément.</span><span class="sxs-lookup"><span data-stu-id="ed66b-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="ed66b-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="ed66b-139">Représente l'identificateur de l'élément dont cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="ed66b-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="ed66b-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="ed66b-141">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="ed66b-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="ed66b-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="ed66b-143">Indique si un élément n'a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="ed66b-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="ed66b-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="ed66b-145">Indique si un utilisateur a envoyé un élément pour lui ou elle-même.</span><span class="sxs-lookup"><span data-stu-id="ed66b-145">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="ed66b-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="ed66b-147">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="ed66b-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="ed66b-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="ed66b-149">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="ed66b-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="ed66b-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="ed66b-151">Représente la collection de tous les en-têtes de message Internet contenus dans un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed66b-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="ed66b-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="ed66b-153">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="ed66b-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="ed66b-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="ed66b-155">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="ed66b-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="ed66b-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="ed66b-157">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed66b-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="ed66b-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="ed66b-p102">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="ed66b-p102">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="ed66b-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="ed66b-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="ed66b-162">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed66b-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="ed66b-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="ed66b-164">Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.</span><span class="sxs-lookup"><span data-stu-id="ed66b-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="ed66b-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="ed66b-166">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone Cc.</span><span class="sxs-lookup"><span data-stu-id="ed66b-166">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="ed66b-167">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.</span><span class="sxs-lookup"><span data-stu-id="ed66b-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="ed66b-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="ed66b-169">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone à.</span><span class="sxs-lookup"><span data-stu-id="ed66b-169">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="ed66b-170">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="ed66b-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="ed66b-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="ed66b-p105">Représente une propriété définie sur **true** si un élément comporte au moins une pièce jointe visible. Cette propriété est en lecture seule.  </span><span class="sxs-lookup"><span data-stu-id="ed66b-p105">Represents a property that is set to **true** if an item has at least one visible attachment. This property is read-only.  </span></span><br/> |
|[<span data-ttu-id="ed66b-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="ed66b-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="ed66b-175">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="ed66b-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-176">Culture</span><span class="sxs-lookup"><span data-stu-id="ed66b-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="ed66b-177">Représente la culture d'un élément donné dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed66b-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-178">La propriété ActualWork</span><span class="sxs-lookup"><span data-stu-id="ed66b-178">ActualWork</span></span>](actualwork.md) <br/> |<span data-ttu-id="ed66b-179">Représente la valeur effective de temps passé sur une tâche.</span><span class="sxs-lookup"><span data-stu-id="ed66b-179">Represents the actual amount of time that is spent on a task.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-180">AssignedTime</span><span class="sxs-lookup"><span data-stu-id="ed66b-180">AssignedTime</span></span>](assignedtime.md) <br/> |<span data-ttu-id="ed66b-181">Représente le temps lorsqu’une tâche est affectée à un contact.</span><span class="sxs-lookup"><span data-stu-id="ed66b-181">Represents the time when a task is assigned to a contact.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-182">BillingInformation</span><span class="sxs-lookup"><span data-stu-id="ed66b-182">BillingInformation</span></span>](billinginformation.md) <br/> |<span data-ttu-id="ed66b-183">Contient les informations pour une tâche de facturation.</span><span class="sxs-lookup"><span data-stu-id="ed66b-183">Holds billing information for a task.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-184">ChangeCount</span><span class="sxs-lookup"><span data-stu-id="ed66b-184">ChangeCount</span></span>](changecount.md) <br/> |<span data-ttu-id="ed66b-185">Spécifie la version de la tâche.</span><span class="sxs-lookup"><span data-stu-id="ed66b-185">Specifies the version of the task.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-186">Companies</span><span class="sxs-lookup"><span data-stu-id="ed66b-186">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="ed66b-187">Représente la collection des sociétés qui sont associés à un contact ou une tâche.</span><span class="sxs-lookup"><span data-stu-id="ed66b-187">Represents the collection of companies that are associated with a contact or task.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-188">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="ed66b-188">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="ed66b-189">Représente la date à laquelle une tâche est terminée.</span><span class="sxs-lookup"><span data-stu-id="ed66b-189">Represents the date on which a task is completed.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-190">Contacts</span><span class="sxs-lookup"><span data-stu-id="ed66b-190">Contacts</span></span>](contacts-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ed66b-191">Contient une liste des contacts qui sont associés à une tâche.</span><span class="sxs-lookup"><span data-stu-id="ed66b-191">Contains a list of contacts that are associated with a task.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-192">DelegationState</span><span class="sxs-lookup"><span data-stu-id="ed66b-192">DelegationState</span></span>](delegationstate.md) <br/> |<span data-ttu-id="ed66b-193">Représente l’état d’une tâche déléguée.</span><span class="sxs-lookup"><span data-stu-id="ed66b-193">Represents the status of a delegated task.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-194">Personne</span><span class="sxs-lookup"><span data-stu-id="ed66b-194">Delegator</span></span>](delegator.md) <br/> |<span data-ttu-id="ed66b-195">Contient le nom de la personne qui a attribué la tâche.</span><span class="sxs-lookup"><span data-stu-id="ed66b-195">Contains the name of the delegator who assigned the task.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-196">DueDate</span><span class="sxs-lookup"><span data-stu-id="ed66b-196">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="ed66b-197">Représente la date à laquelle un élément de tâche est due.</span><span class="sxs-lookup"><span data-stu-id="ed66b-197">Represents the date when a task item is due.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-198">IsAssignmentEditable</span><span class="sxs-lookup"><span data-stu-id="ed66b-198">IsAssignmentEditable</span></span>](isassignmenteditable.md) <br/> |<span data-ttu-id="ed66b-199">Indique si la tâche est modifiable ou non.</span><span class="sxs-lookup"><span data-stu-id="ed66b-199">Indicates whether the task is editable or not.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-200">Avertisse</span><span class="sxs-lookup"><span data-stu-id="ed66b-200">IsComplete</span></span>](iscomplete.md) <br/> |<span data-ttu-id="ed66b-201">Indique si la tâche est terminée ou non.</span><span class="sxs-lookup"><span data-stu-id="ed66b-201">Indicates whether the task has been completed or not.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-202">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="ed66b-202">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="ed66b-203">Indique si une tâche fait partie d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="ed66b-203">Indicates whether a task is part of a recurring item.</span></span> <span data-ttu-id="ed66b-204">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="ed66b-204">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-205">IsTeamTask</span><span class="sxs-lookup"><span data-stu-id="ed66b-205">IsTeamTask</span></span>](isteamtask.md) <br/> |<span data-ttu-id="ed66b-206">Indique si la tâche appartient à une équipe ou non.</span><span class="sxs-lookup"><span data-stu-id="ed66b-206">Indicates whether the task is owned by a team or not.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-207">Mileage</span><span class="sxs-lookup"><span data-stu-id="ed66b-207">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="ed66b-208">Représente le mileage pour un élément de tâche.</span><span class="sxs-lookup"><span data-stu-id="ed66b-208">Represents mileage for a task item.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-209">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="ed66b-209">Owner</span></span>](owner.md) <br/> |<span data-ttu-id="ed66b-210">Représente le propriétaire d’une tâche.</span><span class="sxs-lookup"><span data-stu-id="ed66b-210">Represents the owner of a task.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-211">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="ed66b-211">PercentComplete</span></span>](percentcomplete.md) <br/> |<span data-ttu-id="ed66b-212">Décrit l’état d’achèvement d’une tâche.</span><span class="sxs-lookup"><span data-stu-id="ed66b-212">Describes the completion status of a task.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-213">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="ed66b-213">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="ed66b-214">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="ed66b-214">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-215">Date de début</span><span class="sxs-lookup"><span data-stu-id="ed66b-215">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="ed66b-216">Représente la date de début d’un élément de tâche.</span><span class="sxs-lookup"><span data-stu-id="ed66b-216">Represents the start date of a task item.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-217">Status</span><span class="sxs-lookup"><span data-stu-id="ed66b-217">Status</span></span>](status.md) <br/> |<span data-ttu-id="ed66b-218">Représente l’état d’un élément de tâche.</span><span class="sxs-lookup"><span data-stu-id="ed66b-218">Represents the status of a task item.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-219">StatusDescription</span><span class="sxs-lookup"><span data-stu-id="ed66b-219">StatusDescription</span></span>](statusdescription.md) <br/> |<span data-ttu-id="ed66b-220">Contient une explication de l’état de la tâche.</span><span class="sxs-lookup"><span data-stu-id="ed66b-220">Contains an explanation of the task status.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-221">TotalWork</span><span class="sxs-lookup"><span data-stu-id="ed66b-221">TotalWork</span></span>](totalwork.md) <br/> |<span data-ttu-id="ed66b-222">Contient une description de la quantité de travail est associé à un élément.</span><span class="sxs-lookup"><span data-stu-id="ed66b-222">Contains a description of how much work is associated with an item.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-223">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="ed66b-223">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="ed66b-224">Contient les droits du client en fonction des paramètres d’autorisation pour l’élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="ed66b-224">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="ed66b-225">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="ed66b-225">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-226">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="ed66b-226">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="ed66b-227">Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.</span><span class="sxs-lookup"><span data-stu-id="ed66b-227">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-228">Heure de dernière modification</span><span class="sxs-lookup"><span data-stu-id="ed66b-228">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="ed66b-229">Indique quand un élément a été modifié pour la dernière fois.</span><span class="sxs-lookup"><span data-stu-id="ed66b-229">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-230">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="ed66b-230">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="ed66b-231">Indique si l'élément est associé à un dossier.</span><span class="sxs-lookup"><span data-stu-id="ed66b-231">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-232">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="ed66b-232">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="ed66b-233">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ed66b-233">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-234">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="ed66b-234">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="ed66b-235">Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ed66b-235">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-236">ConversationId</span><span class="sxs-lookup"><span data-stu-id="ed66b-236">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="ed66b-237">Contient l'identificateur d'un élément ou d'une conversation.</span><span class="sxs-lookup"><span data-stu-id="ed66b-237">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-238">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="ed66b-238">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="ed66b-239">Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="ed66b-239">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed66b-240">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ed66b-240">Parent elements</span></span>

|<span data-ttu-id="ed66b-241">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ed66b-241">**Element**</span></span>|<span data-ttu-id="ed66b-242">**Description**</span><span class="sxs-lookup"><span data-stu-id="ed66b-242">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed66b-243">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="ed66b-243">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="ed66b-244">Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="ed66b-244">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-245">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ed66b-245">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="ed66b-246">Identifie les données à ajouter à une propriété d’un élément/dossier lors d’une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ed66b-246">Identifies data to append to a single property of an item/folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ed66b-247">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="ed66b-247">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="ed66b-248">Identifie tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="ed66b-248">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-249">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ed66b-249">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="ed66b-250">Identifie un élément unique à créer dans le magasin du client local.</span><span class="sxs-lookup"><span data-stu-id="ed66b-250">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-251">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="ed66b-251">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="ed66b-252">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed66b-252">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-253">Items</span><span class="sxs-lookup"><span data-stu-id="ed66b-253">Items</span></span>](items.md) <br/> |<span data-ttu-id="ed66b-254">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="ed66b-254">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="ed66b-255">SetItemField</span><span class="sxs-lookup"><span data-stu-id="ed66b-255">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="ed66b-256">Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ed66b-256">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ed66b-257">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ed66b-257">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="ed66b-258">Identifie un élément unique à mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="ed66b-258">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ed66b-259">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ed66b-259">Text value</span></span>

<span data-ttu-id="ed66b-260">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ed66b-260">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ed66b-261">Remarques</span><span class="sxs-lookup"><span data-stu-id="ed66b-261">Remarks</span></span>

<span data-ttu-id="ed66b-262">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed66b-262">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed66b-263">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ed66b-263">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed66b-264">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ed66b-264">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed66b-265">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ed66b-265">Schema name</span></span>  <br/> |<span data-ttu-id="ed66b-266">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ed66b-266">Types schema</span></span>  <br/> |
|<span data-ttu-id="ed66b-267">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ed66b-267">Validation file</span></span>  <br/> |<span data-ttu-id="ed66b-268">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ed66b-268">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed66b-269">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ed66b-269">Can be empty</span></span>  <br/> |<span data-ttu-id="ed66b-270">False</span><span class="sxs-lookup"><span data-stu-id="ed66b-270">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed66b-271">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ed66b-271">See also</span></span>

- [<span data-ttu-id="ed66b-272">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ed66b-272">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="ed66b-273">Création de tâches</span><span class="sxs-lookup"><span data-stu-id="ed66b-273">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
- [<span data-ttu-id="ed66b-274">Suppression de tâches</span><span class="sxs-lookup"><span data-stu-id="ed66b-274">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

