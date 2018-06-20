---
title: Opération CreateItem (tâche)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 12c5da4d-290c-4a8a-a965-0bf5d55c7978
description: L’opération CreateItem crée des éléments de tâche dans la banque d’informations Exchange.
ms.openlocfilehash: 5a5203202071ae9391faa9348902424317ee96d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755722"
---
# <a name="createitem-operation-task"></a><span data-ttu-id="20891-103">Opération CreateItem (tâche)</span><span class="sxs-lookup"><span data-stu-id="20891-103">CreateItem operation (task)</span></span>

<span data-ttu-id="20891-104">L’opération CreateItem crée des éléments de tâche dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="20891-104">The CreateItem operation creates task items in the Exchange store.</span></span>
  
## <a name="task-createitem-request"></a><span data-ttu-id="20891-105">CreateItem demande de tâche</span><span class="sxs-lookup"><span data-stu-id="20891-105">Task CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="20891-106">Description</span><span class="sxs-lookup"><span data-stu-id="20891-106">Description</span></span>

<span data-ttu-id="20891-107">Une demande CreateItem l’exemple suivant montre comment créer un élément de tâche dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="20891-107">The following example of a CreateItem request shows how to create a task item in a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="20891-108">Code</span><span class="sxs-lookup"><span data-stu-id="20891-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                MessageDisposition="SaveOnly">
      <Items>
        <t:Task>
          <t:Subject>My task</t:Subject>
          <t:DueDate>2006-10-26T21:32:52</t:DueDate>
          <t:Status>NotStarted</t:Status>
        </t:Task>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="20891-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="20891-109">Comments</span></span>

<span data-ttu-id="20891-110">Demandes de tâches périodiques soient modifiées quand ils sont reçus par l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="20891-110">Requests for recurring tasks are altered when they are received by the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span> <span data-ttu-id="20891-111">Les modifications suivantes se produisent :</span><span class="sxs-lookup"><span data-stu-id="20891-111">The following changes occur:</span></span>
  
- <span data-ttu-id="20891-112">Seule la date est enregistrée pour la propriété [StartDate (périodicité)](startdate-recurrence.md) de la plage de périodicité de la tâche.</span><span class="sxs-lookup"><span data-stu-id="20891-112">Only the date is saved for the [StartDate (Recurrence)](startdate-recurrence.md) property of the recurrence range of the task.</span></span> <span data-ttu-id="20891-113">La partie heure est tronquée.</span><span class="sxs-lookup"><span data-stu-id="20891-113">The time part is truncated.</span></span> 
    
- <span data-ttu-id="20891-114">La propriété [StartDate (périodicité)](startdate-recurrence.md) peut-être être ajustée en fonction de la périodicité.</span><span class="sxs-lookup"><span data-stu-id="20891-114">The [StartDate (Recurrence)](startdate-recurrence.md) property may be adjusted, depending on the recurrence pattern.</span></span> <span data-ttu-id="20891-115">Par exemple, si la périodicité est spécifiée comme tous les lundis et StartDate est défini sur le 26 octobre 2006, qui est un jeudi, StartDate est réglé à 30 octobre 2006, qui est le lundi.</span><span class="sxs-lookup"><span data-stu-id="20891-115">For example, if the recurrence pattern is specified as every Monday and the StartDate is set to October 26, 2006, which is a Thursday, StartDate is adjusted to October 30, 2006, which is the next Monday.</span></span> 
    
- <span data-ttu-id="20891-116">Si la propriété [date de début](startdate.md) de la tâche est définie, il est mis à jour pour correspondre à la [date de début (périodicité)](startdate-recurrence.md) de la plage de périodicité.</span><span class="sxs-lookup"><span data-stu-id="20891-116">If the [StartDate](startdate.md) property of the task is set, it is updated to match the [StartDate (Recurrence)](startdate-recurrence.md) of the recurrence range.</span></span> <span data-ttu-id="20891-117">La propriété [DueDate](duedate.md) de la tâche est également mis à jour en fonction de la nouvelle [date de début](startdate.md).</span><span class="sxs-lookup"><span data-stu-id="20891-117">The [DueDate](duedate.md) property of the task is also updated based on the new [StartDate](startdate.md).</span></span>
    
- <span data-ttu-id="20891-118">Si [date_début](startdate.md) n’est pas définie, seule la propriété [DueDate](duedate.md) est mis à jour pour correspondre à la [date de début (périodicité)](startdate-recurrence.md) de la plage de périodicité.</span><span class="sxs-lookup"><span data-stu-id="20891-118">If the [StartDate](startdate.md) is not set, only the [DueDate](duedate.md) property is updated to match the [StartDate (Recurrence)](startdate-recurrence.md) of the recurrence range.</span></span> 
    
<span data-ttu-id="20891-119">Le tableau suivant présente les modifications apportées par le serveur d’accès au Client à une tâche périodique ayant un Task.Recurrence.Pattern de tous les lundis.</span><span class="sxs-lookup"><span data-stu-id="20891-119">The following table shows the changes that the Client Access server makes to a recurring task that has a Task.Recurrence.Pattern of every Monday.</span></span>
  
<span data-ttu-id="20891-120">**Modifications apportées à une tâche périodique**</span><span class="sxs-lookup"><span data-stu-id="20891-120">**Changes to a recurring task**</span></span>

|<span data-ttu-id="20891-121">**Propriété**</span><span class="sxs-lookup"><span data-stu-id="20891-121">**Property**</span></span>|<span data-ttu-id="20891-122">**Valeur d’origine**</span><span class="sxs-lookup"><span data-stu-id="20891-122">**Original Value**</span></span>|<span data-ttu-id="20891-123">**Valeur mise à jour**</span><span class="sxs-lookup"><span data-stu-id="20891-123">**Updated Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="20891-124">Task.StartDate</span><span class="sxs-lookup"><span data-stu-id="20891-124">Task.StartDate</span></span>  <br/> |<span data-ttu-id="20891-125">1er janvier 2006</span><span class="sxs-lookup"><span data-stu-id="20891-125">January 1, 2006</span></span>  <br/> |<span data-ttu-id="20891-126">30 octobre 2006</span><span class="sxs-lookup"><span data-stu-id="20891-126">October 30, 2006</span></span>  <br/> |
|<span data-ttu-id="20891-127">Task.DueDate</span><span class="sxs-lookup"><span data-stu-id="20891-127">Task.DueDate</span></span>  <br/> |<span data-ttu-id="20891-128">3 janvier 2006</span><span class="sxs-lookup"><span data-stu-id="20891-128">January 3, 2006</span></span>  <br/> |<span data-ttu-id="20891-129">1er novembre 2006</span><span class="sxs-lookup"><span data-stu-id="20891-129">November 1, 2006</span></span>  <br/> |
|<span data-ttu-id="20891-130">Task.Recurrence.Range.StartDate</span><span class="sxs-lookup"><span data-stu-id="20891-130">Task.Recurrence.Range.StartDate</span></span>  <br/> |<span data-ttu-id="20891-131">26 octobre 2006</span><span class="sxs-lookup"><span data-stu-id="20891-131">October 26, 2006</span></span>  <br/> |<span data-ttu-id="20891-132">30 octobre 2006</span><span class="sxs-lookup"><span data-stu-id="20891-132">October 30, 2006</span></span>  <br/> |
   
<span data-ttu-id="20891-133">Par défaut, si un dossier de destination n’est pas spécifié, les éléments de tâche sont créés dans le dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="20891-133">By default, if a destination folder is not specified, task items are created in the Tasks folder.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="20891-134">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="20891-134">Request elements</span></span>

<span data-ttu-id="20891-135">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="20891-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="20891-136">CreateItem</span><span class="sxs-lookup"><span data-stu-id="20891-136">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="20891-137">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="20891-137">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="20891-138">Tâche</span><span class="sxs-lookup"><span data-stu-id="20891-138">Task</span></span>](task.md)
    
- [<span data-ttu-id="20891-139">Objet</span><span class="sxs-lookup"><span data-stu-id="20891-139">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="20891-140">DueDate</span><span class="sxs-lookup"><span data-stu-id="20891-140">DueDate</span></span>](duedate.md)
    
- [<span data-ttu-id="20891-141">Status</span><span class="sxs-lookup"><span data-stu-id="20891-141">Status</span></span>](status.md)
    
## <a name="successful-task-createitem-response"></a><span data-ttu-id="20891-142">Réponse CreateItem réussie</span><span class="sxs-lookup"><span data-stu-id="20891-142">Successful Task CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="20891-143">Description</span><span class="sxs-lookup"><span data-stu-id="20891-143">Description</span></span>

<span data-ttu-id="20891-144">L’exemple suivant montre une réponse positive à la demande CreateItem.</span><span class="sxs-lookup"><span data-stu-id="20891-144">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="20891-145">Code</span><span class="sxs-lookup"><span data-stu-id="20891-145">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Task>
              <t:ItemId Id="AAAtAE=" ChangeKey="EwAAABYA"/>
            </t:Task>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="20891-146">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="20891-146">Successful response elements</span></span>

<span data-ttu-id="20891-147">Les éléments suivants sont inclus dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="20891-147">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="20891-148">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="20891-148">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="20891-149">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="20891-149">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="20891-150">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="20891-150">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="20891-151">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="20891-151">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="20891-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="20891-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="20891-153">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="20891-153">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="20891-154">Tâche</span><span class="sxs-lookup"><span data-stu-id="20891-154">Task</span></span>](task.md)
    
- [<span data-ttu-id="20891-155">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="20891-155">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="20891-156">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="20891-156">See also</span></span>



[<span data-ttu-id="20891-157">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="20891-157">CreateItem operation</span></span>](createitem-operation.md)


[<span data-ttu-id="20891-158">Création de tâches</span><span class="sxs-lookup"><span data-stu-id="20891-158">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="20891-159">Mise à jour de tâches</span><span class="sxs-lookup"><span data-stu-id="20891-159">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[<span data-ttu-id="20891-160">Suppression de tâches</span><span class="sxs-lookup"><span data-stu-id="20891-160">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

