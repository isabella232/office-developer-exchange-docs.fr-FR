---
title: Opération de GetItem (tâche)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 8265dd06-1752-4470-8074-5f0e3e970f52
description: L’opération GetItem est utilisée pour obtenir des tâches à partir de la banque d’informations Exchange.
ms.openlocfilehash: 412710f32ed8702e1a28a596833c3a7e47e3ed76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756666"
---
# <a name="getitem-operation-task"></a><span data-ttu-id="bf4cc-103">Opération de GetItem (tâche)</span><span class="sxs-lookup"><span data-stu-id="bf4cc-103">GetItem operation (task)</span></span>

<span data-ttu-id="bf4cc-104">L’opération GetItem est utilisée pour obtenir des tâches à partir de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf4cc-104">The GetItem operation is used to get tasks from the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bf4cc-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="bf4cc-105">Remarks</span></span>

<span data-ttu-id="bf4cc-106">Le format de la demande de GetItem pour les tâches est identique à GetItem pour tout autre type d’élément.</span><span class="sxs-lookup"><span data-stu-id="bf4cc-106">The format of the GetItem request for tasks is the same as GetItem for any other item type.</span></span> <span data-ttu-id="bf4cc-107">La seule différence réside dans lequel il sont possible de demander des propriétés supplémentaires au sein de la forme de réponse.</span><span class="sxs-lookup"><span data-stu-id="bf4cc-107">The only difference is in which additional properties can be requested within the response shape.</span></span> <span data-ttu-id="bf4cc-108">Ces propriétés supplémentaires doivent être propriétés liées aux tâches ou les propriétés étendues.</span><span class="sxs-lookup"><span data-stu-id="bf4cc-108">Such additional properties must either be task-related properties or extended properties.</span></span>
  
## <a name="task-getitem-request-example"></a><span data-ttu-id="bf4cc-109">Exemple de requête GetItem des tâches</span><span class="sxs-lookup"><span data-stu-id="bf4cc-109">Task GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="bf4cc-110">Description</span><span class="sxs-lookup"><span data-stu-id="bf4cc-110">Description</span></span>

<span data-ttu-id="bf4cc-111">Une demande de GetItem l’exemple suivant montre comment obtenir un élément de tâche.</span><span class="sxs-lookup"><span data-stu-id="bf4cc-111">The following example of a GetItem request shows how to get a task item.</span></span>
  
### <a name="code"></a><span data-ttu-id="bf4cc-112">Code</span><span class="sxs-lookup"><span data-stu-id="bf4cc-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAEFkb..."/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="bf4cc-113">Commentaires</span><span class="sxs-lookup"><span data-stu-id="bf4cc-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="bf4cc-114">L’identificateur d’élément et modifier la clé ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="bf4cc-114">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="bf4cc-115">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="bf4cc-115">Request elements</span></span>

<span data-ttu-id="bf4cc-116">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="bf4cc-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="bf4cc-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="bf4cc-117">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="bf4cc-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="bf4cc-118">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="bf4cc-119">BaseShape</span><span class="sxs-lookup"><span data-stu-id="bf4cc-119">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="bf4cc-120">ItemId</span><span class="sxs-lookup"><span data-stu-id="bf4cc-120">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="bf4cc-121">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="bf4cc-121">ItemId</span></span>](itemid.md)
    
## <a name="task-getitem-response-example"></a><span data-ttu-id="bf4cc-122">Exemple de réponse GetItem des tâches</span><span class="sxs-lookup"><span data-stu-id="bf4cc-122">Task GetItem response example</span></span>

### <a name="description"></a><span data-ttu-id="bf4cc-123">Description</span><span class="sxs-lookup"><span data-stu-id="bf4cc-123">Description</span></span>

<span data-ttu-id="bf4cc-124">L’exemple suivant montre une réponse positive à une demande de GetItem.</span><span class="sxs-lookup"><span data-stu-id="bf4cc-124">The following example shows a successful response to a GetItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="bf4cc-125">Code</span><span class="sxs-lookup"><span data-stu-id="bf4cc-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Task>
              <t:ItemId Id="AAAtAEA=" ChangeKey="EwAAAB"/>
              <t:ParentFolderId Id="AAAtAEFkbWl=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Task</t:ItemClass>
              <t:Subject>Buy new shoes</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text"/>
              <t:DateTimeReceived>2006-09-15T15:23:08Z</t:DateTimeReceived>
              <t:Size>153</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>true</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-09-15T15:23:08Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-09-15T15:23:08Z</t:DateTimeCreated>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en-US</t:Culture>
              <t:ChangeCount>1</t:ChangeCount>
              <t:IsComplete>false</t:IsComplete>
              <t:IsRecurring>false</t:IsRecurring>
              <t:PercentComplete>0</t:PercentComplete>
              <t:Status>NotStarted</t:Status>
              <t:StatusDescription>Not Started</t:StatusDescription>
            </t:Task>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="bf4cc-126">Commentaires</span><span class="sxs-lookup"><span data-stu-id="bf4cc-126">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="bf4cc-127">Les identificateurs d’éléments et dossiers et les touches de modification ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="bf4cc-127">The item and folder identifiers and change keys have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="bf4cc-128">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="bf4cc-128">Successful response elements</span></span>

<span data-ttu-id="bf4cc-129">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="bf4cc-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="bf4cc-130">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bf4cc-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="bf4cc-131">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="bf4cc-131">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="bf4cc-132">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bf4cc-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bf4cc-133">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bf4cc-133">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="bf4cc-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bf4cc-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bf4cc-135">Items</span><span class="sxs-lookup"><span data-stu-id="bf4cc-135">Items</span></span>](items.md)
    
- [<span data-ttu-id="bf4cc-136">Tâche</span><span class="sxs-lookup"><span data-stu-id="bf4cc-136">Task</span></span>](task.md)
    
- [<span data-ttu-id="bf4cc-137">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="bf4cc-137">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="bf4cc-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="bf4cc-138">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="bf4cc-139">ItemClass</span><span class="sxs-lookup"><span data-stu-id="bf4cc-139">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="bf4cc-140">Objet</span><span class="sxs-lookup"><span data-stu-id="bf4cc-140">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="bf4cc-141">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="bf4cc-141">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="bf4cc-142">Corps</span><span class="sxs-lookup"><span data-stu-id="bf4cc-142">Body</span></span>](body.md)
    
- [<span data-ttu-id="bf4cc-143">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="bf4cc-143">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="bf4cc-144">Taille</span><span class="sxs-lookup"><span data-stu-id="bf4cc-144">Size</span></span>](size.md)
    
- [<span data-ttu-id="bf4cc-145">Importance</span><span class="sxs-lookup"><span data-stu-id="bf4cc-145">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="bf4cc-146">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="bf4cc-146">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="bf4cc-147">IsDraft</span><span class="sxs-lookup"><span data-stu-id="bf4cc-147">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="bf4cc-148">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="bf4cc-148">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="bf4cc-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="bf4cc-149">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="bf4cc-150">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="bf4cc-150">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="bf4cc-151">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="bf4cc-151">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="bf4cc-152">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="bf4cc-152">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="bf4cc-153">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="bf4cc-153">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="bf4cc-154">Culture</span><span class="sxs-lookup"><span data-stu-id="bf4cc-154">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="bf4cc-155">ChangeCount</span><span class="sxs-lookup"><span data-stu-id="bf4cc-155">ChangeCount</span></span>](changecount.md)
    
- [<span data-ttu-id="bf4cc-156">Avertisse</span><span class="sxs-lookup"><span data-stu-id="bf4cc-156">IsComplete</span></span>](iscomplete.md)
    
- [<span data-ttu-id="bf4cc-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="bf4cc-157">IsRecurring</span></span>](isrecurring.md)
    
- [<span data-ttu-id="bf4cc-158">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="bf4cc-158">PercentComplete</span></span>](percentcomplete.md)
    
- [<span data-ttu-id="bf4cc-159">Status</span><span class="sxs-lookup"><span data-stu-id="bf4cc-159">Status</span></span>](status.md)
    
- [<span data-ttu-id="bf4cc-160">StatusDescription</span><span class="sxs-lookup"><span data-stu-id="bf4cc-160">StatusDescription</span></span>](statusdescription.md)
    
## <a name="see-also"></a><span data-ttu-id="bf4cc-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bf4cc-161">See also</span></span>



[<span data-ttu-id="bf4cc-162">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="bf4cc-162">GetItem operation</span></span>](getitem-operation.md)


[<span data-ttu-id="bf4cc-163">Création de tâches</span><span class="sxs-lookup"><span data-stu-id="bf4cc-163">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="bf4cc-164">Mise à jour de tâches</span><span class="sxs-lookup"><span data-stu-id="bf4cc-164">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[<span data-ttu-id="bf4cc-165">Suppression de tâches</span><span class="sxs-lookup"><span data-stu-id="bf4cc-165">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

