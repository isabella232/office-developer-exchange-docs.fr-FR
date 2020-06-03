---
title: Vérification des résultats d’un appel EWS ou API managée EWS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: 78a1741c-1bbe-4cb4-9331-9d6d3171fc11
description: Découvrez comment vérifier les résultats de vos appels EWS ou API managée EWS.
localization_priority: Priority
ms.openlocfilehash: be8e76898dd111a6dec33d4a57d9d50a2a935390
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457395"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a><span data-ttu-id="29a76-103">Vérification des résultats d’un appel EWS ou API managée EWS</span><span class="sxs-lookup"><span data-stu-id="29a76-103">Verifying the results of an EWS or EWS Managed API call</span></span>

<span data-ttu-id="29a76-104">Découvrez comment vérifier les résultats de vos appels EWS ou API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="29a76-104">Learn how to verify the results of your EWS or EWS Managed API calls.</span></span>
  
<span data-ttu-id="29a76-105">Lorsque les éléments ne fonctionnent pas correctement, il est utile de voir ce qui se passe en examinant les demandes SOAP que votre application envoie sur le réseau et les réponses renvoyées par le serveur.</span><span class="sxs-lookup"><span data-stu-id="29a76-105">When things aren't working correctly, it helps to see what's going on by examining the SOAP requests that your application is sending over the network and the responses that the server is sending back.</span></span> <span data-ttu-id="29a76-106">L’article [Outils et ressources pour la résolution des problèmes liés aux applications EWS](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) inclut des liens vers des outils permettant de capturer et d’afficher ces demandes SOAP.</span><span class="sxs-lookup"><span data-stu-id="29a76-106">The [tools and resources for troubleshooting EWS applications](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) article includes links to tools to help capture and view those SOAP requests.</span></span> <span data-ttu-id="29a76-107">Une fois que vous avez reçu les requêtes et les réponses, comment vérifier que la demande que vous avez envoyée au serveur a été correctement traitée ?</span><span class="sxs-lookup"><span data-stu-id="29a76-107">After you've got the requests and the responses, how do you verify that the request you sent to the server was processed correctly?</span></span> <span data-ttu-id="29a76-108">Lisez la suite pour en savoir plus.</span><span class="sxs-lookup"><span data-stu-id="29a76-108">Read on to find out.</span></span> 
  
<span data-ttu-id="29a76-109">Si vous envoyez des demandes EWS, vous allez démarrer votre vérification en vérifiant l’attribut **ResponseClass** pour chaque message de réponse dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="29a76-109">If you're sending EWS requests, you're going to start your verification by checking the **ResponseClass** attribute for each response message in the response.</span></span> <span data-ttu-id="29a76-110">Cela vous permettra de savoir si l’opération s’est terminée avec succès sur chaque élément.</span><span class="sxs-lookup"><span data-stu-id="29a76-110">That will tell you whether the operation completed successfully on each item.</span></span> 
  
<span data-ttu-id="29a76-111">En fonction de l’objet que votre méthode appelle, si vous utilisez l’API managée EWS pour envoyer des demandes, vous pouvez effectuer une vérification à l’aide des objets Response.</span><span class="sxs-lookup"><span data-stu-id="29a76-111">Depending on the object that your method is calling, if you're using the EWS Managed API to send requests, you can do some verification using the response objects.</span></span> <span data-ttu-id="29a76-112">Toutefois, étant donné que la réponse SOAP contient un sur-ensemble de ce qui est inclus dans les objets de réponse de l’API managée EWS, vous pouvez également consulter la réponse SOAP.</span><span class="sxs-lookup"><span data-stu-id="29a76-112">But because the SOAP response contains a superset of what's included in the EWS Managed API response objects, you might want to look at the SOAP response as well.</span></span> <span data-ttu-id="29a76-113">Étant donné que la réponse SOAP peut souvent contenir plus d’informations que les objets de réponse de l’API managée EWS, commencez votre vérification avec la réponse SOAP.</span><span class="sxs-lookup"><span data-stu-id="29a76-113">Because the SOAP response can often contain more information than the EWS Managed API response objects, start your verification with the SOAP response.</span></span>
  
## <a name="verifying-the-results-of-a-soap-response"></a><span data-ttu-id="29a76-114">Vérification des résultats d’une réponse SOAP</span><span class="sxs-lookup"><span data-stu-id="29a76-114">Verifying the results of a SOAP response</span></span>
<span data-ttu-id="29a76-115"><a name="bk_verifysoap"> </a></span><span class="sxs-lookup"><span data-stu-id="29a76-115"><a name="bk_verifysoap"> </a></span></span>

<span data-ttu-id="29a76-116">Lorsque vous recevez une réponse SOAP, la première chose à examiner est l’attribut **ResponseClass** .</span><span class="sxs-lookup"><span data-stu-id="29a76-116">When you receive a SOAP response, the first thing to look at is the **ResponseClass** attribute.</span></span> <span data-ttu-id="29a76-117">Cet attribut est inclus dans chaque instance **ResponseMessageType** de l’élément [ResponseMessages](https://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="29a76-117">This attribute is included in each **ResponseMessageType** instance in the [ResponseMessages](https://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) element, as shown in the following example.</span></span> 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

<span data-ttu-id="29a76-118">Étant donné qu’une réponse SOAP peut contenir plusieurs messages de réponse dans une réponse SOAP unique, il est important de vérifier chaque message de réponse individuellement.</span><span class="sxs-lookup"><span data-stu-id="29a76-118">Because a SOAP response might contain multiple response messages in a single SOAP response, it's important to check each response message individually.</span></span>
  
<span data-ttu-id="29a76-119">Si vous utilisez une opération qui inclut un **ResponseClass** dans le cadre de la réponse de l’opération, comme suit, vous pouvez être tenté de vérifier uniquement les **ResponseClass** de l’opération.</span><span class="sxs-lookup"><span data-stu-id="29a76-119">If you're working with an operation that includes a **ResponseClass** as part of the operation response, like the following, you might be tempted to only check the **ResponseClass** of the operation.</span></span> 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

<span data-ttu-id="29a76-120">Toutefois, l’état de l’opération reflète uniquement la forme de la réponse de niveau supérieur et ne reflète pas l’état de toutes les réponses de message individuelles.</span><span class="sxs-lookup"><span data-stu-id="29a76-120">However, the operation status only reflects the shape of the top-level response and does not reflect the status of all the individual message responses.</span></span> <span data-ttu-id="29a76-121">Dans l’exemple suivant, l’opération [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) a un **ResponseClass** de **succès**, mais l’élément [DelegateUserResponseMessageType](https://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) sous-jacent a une valeur **ResponseClass** de l' **erreur**.</span><span class="sxs-lookup"><span data-stu-id="29a76-121">In the following example, the [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) operation has a **ResponseClass** of **Success**, but the underlying [DelegateUserResponseMessageType](https://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) element has a **ResponseClass** value of **Error**.</span></span>
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseCode>NoError</m:ResponseCode>
    <m:ResponseMessages>
      <m:DelegateUserResponseMessageType ResponseClass="Error">
        <m:MessageText>The user is already a delegate for the mailbox.</m:MessageText>
        <m:ResponseCode>ErrorDelegateAlreadyExists</m:ResponseCode>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      </m:DelegateUserResponseMessageType>
    </m:ResponseMessages>
  </m:AddDelegateResponse>
</soap:Body>
```

<span data-ttu-id="29a76-122">Ainsi, pour les réponses de SOAP EWS, vous ne pouvez pas compter sur le **ResponseClass** de l’opération : vous devez examiner les **ResponseClass** de chaque message de réponse pour déterminer si l’opération a rencontré des erreurs lors du traitement des éléments.</span><span class="sxs-lookup"><span data-stu-id="29a76-122">So for SOAP EWS responses, you can't rely on the **ResponseClass** of the operation - you have to look at the **ResponseClass** of each response message to determine whether the operation encountered any errors processing the items.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="29a76-123">Vérification de la réussite</span><span class="sxs-lookup"><span data-stu-id="29a76-123">Verifying success</span></span>

<span data-ttu-id="29a76-124">Si chaque attribut **ResponseClass** de chaque attribut **ResponseMessage** est défini sur **Success**, l’opération s’est terminée avec succès sur tous les éléments, et vous pouvez passer à votre tâche suivante.</span><span class="sxs-lookup"><span data-stu-id="29a76-124">If each **ResponseClass** attribute for each **ResponseMessage** attribute is set to **Success**, the operation completed successfully on all the items, and you can move on to your next task.</span></span>
  
<span data-ttu-id="29a76-125">L’exemple suivant montre une réponse réussie à une demande d’opération [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) pour récupérer un élément unique.</span><span class="sxs-lookup"><span data-stu-id="29a76-125">The following example shows a successful response to a [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation request to retrieve a single item.</span></span> <span data-ttu-id="29a76-126">Notez que lorsque **ResponseClass** est défini sur **Success**, le [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) associé est toujours défini sur **NOERROR**.</span><span class="sxs-lookup"><span data-stu-id="29a76-126">Note that when the **ResponseClass** is set to **Success**, the associated [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) is always set to **NoError**.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
            <m:ResponseCode>NoError</m:ResponseCode>
            <m:Items>
              <t:Message>
                <t:ItemId Id="Er5bAAA=" 
                          ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" />
                <t:Subject>Dinner Party</t:Subject>
              </t:Message>
            </m:Items>
          </m:GetItemResponseMessage>
        </m:ResponseMessages>
      </m:GetItemResponse>
    </s:Body>
```

<span data-ttu-id="29a76-127">Voici une réponse réussie à une demande d’opération **GetItem** pour récupérer plusieurs éléments.</span><span class="sxs-lookup"><span data-stu-id="29a76-127">The following is a successful response to a **GetItem** operation request to retrieve multiple items.</span></span> <span data-ttu-id="29a76-128">Chacun des éléments [GetItemResponseMessage](https://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) a une **ResponseClass** de **réussite**.</span><span class="sxs-lookup"><span data-stu-id="29a76-128">Each of the [GetItemResponseMessage](https://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) elements has a **ResponseClass** of **Success**.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
    <m:ResponseMessages>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="Er5bAAA=" 
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" /
            <t:Subject>Dinner Party</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="3c66AAA="
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAc3kqm" />
            <t:Subject>Company Soccer Team</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
    </m:ResponseMessages>
  </m:GetItemResponse>
</s:Body>
```

### <a name="handling-errors-and-warnings"></a><span data-ttu-id="29a76-129">Gestion des erreurs et des avertissements</span><span class="sxs-lookup"><span data-stu-id="29a76-129">Handling errors and warnings</span></span>

<span data-ttu-id="29a76-130">Lorsque vous recevez une réponse et que l’attribut **ResponseClass** est défini sur **Error**, l’opération ne s’est pas terminée correctement sur un ou plusieurs éléments.</span><span class="sxs-lookup"><span data-stu-id="29a76-130">When you receive a response and the **ResponseClass** attribute is set to **Error**, the operation did not complete successfully on one or more items.</span></span> <span data-ttu-id="29a76-131">Corrigez le problème et renouvelez votre demande, ou la partie de votre demande qui a échoué.</span><span class="sxs-lookup"><span data-stu-id="29a76-131">Correct the issue and retry your request, or the part of your request that failed.</span></span> <span data-ttu-id="29a76-132">La valeur d' **Avertissement** d’un attribut **ResponseClass** est renvoyée par l’opération [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) uniquement et indique que l’entité n’a pas pu être résolue en une identité unique.</span><span class="sxs-lookup"><span data-stu-id="29a76-132">A **ResponseClass** attribute value of **Warning** value is only returned by the [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation, and indicates that the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="29a76-133">Vous pouvez l’ignorer pour toutes les autres opérations.</span><span class="sxs-lookup"><span data-stu-id="29a76-133">You can ignore it for all other operations.</span></span> 
  
<span data-ttu-id="29a76-134">Dans la réponse suivante, l’attribut **ResponseClass** a une valeur d' **erreur**.</span><span class="sxs-lookup"><span data-stu-id="29a76-134">In the following response, the **ResponseClass** attribute has a value of **Error**.</span></span>
  
```XML
<m:GetItemResponseMessage ResponseClass="Error">
  <m:MessageText>Property is not valid for this object type.</m:MessageText>
  <m:ResponseCode>ErrorInvalidPropertyRequest</m:ResponseCode>
  <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
  <m:MessageXml>
    <t:FieldURI FieldURI="meeting:AssociatedCalendarItemId" />
  </m:MessageXml>
  <m:Items />
</m:GetItemResponseMessage>
```

<span data-ttu-id="29a76-135">Dans cet exemple, EWS fournit des indices pour déboguer le problème.</span><span class="sxs-lookup"><span data-stu-id="29a76-135">In this example, EWS provides clues to debug the issue.</span></span> <span data-ttu-id="29a76-136">Lorsque l’attribut **ResponseClass** a une valeur d' **erreur**, les éléments supplémentaires suivants sont inclus dans la réponse, le cas échéant :</span><span class="sxs-lookup"><span data-stu-id="29a76-136">When the **ResponseClass** attribute has a value of **Error**, the following additional elements are included in the response when applicable:</span></span>
  
- <span data-ttu-id="29a76-137">[MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — décrit l’erreur.</span><span class="sxs-lookup"><span data-stu-id="29a76-137">[MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="29a76-138">[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — contient le code d’erreur, qui peut être utilisé pour trouver des ressources de résolution des problèmes supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="29a76-138">[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="29a76-139">[Messagexml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — identifie les éléments à l’origine de l’erreur.</span><span class="sxs-lookup"><span data-stu-id="29a76-139">[MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — Identifies the elements that caused the error.</span></span> 
    
- <span data-ttu-id="29a76-140">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) : non utilisé.</span><span class="sxs-lookup"><span data-stu-id="29a76-140">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — Unused.</span></span> 
    
<span data-ttu-id="29a76-141">Vous pouvez utiliser les informations fournies dans ces éléments pour examiner votre problème.</span><span class="sxs-lookup"><span data-stu-id="29a76-141">You can use the information provided in these elements to investigate your issue.</span></span> <span data-ttu-id="29a76-142">Dans l’exemple précédent, l' **MessageText** indique que la propriété n’est pas valide pour le type d’objet.</span><span class="sxs-lookup"><span data-stu-id="29a76-142">In the previous example, the **MessageText** indicates that the property isn't valid for the object type.</span></span> <span data-ttu-id="29a76-143">La demande consistait à obtenir un message électronique, mais le jeu de propriétés comprenait **AssociatedCalendarItemId**, ce qui est uniquement valide pour les éléments de rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="29a76-143">The request was to get an email message, but the property set included the **AssociatedCalendarItemId**, which is only valid for appointment items.</span></span>
  
<span data-ttu-id="29a76-144">L’exemple suivant montre une erreur qui a été reçue dans le cadre d’une opération par lots pour obtenir plusieurs éléments de courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="29a76-144">The following example shows an error that was received as part of a batched operation to get multiple email items.</span></span> <span data-ttu-id="29a76-145">Le premier élément a été récupéré avec succès et **ResponseClass** est défini sur **Success**.</span><span class="sxs-lookup"><span data-stu-id="29a76-145">The first item was retrieved successfully and the **ResponseClass** is set to **Success**.</span></span> <span data-ttu-id="29a76-146">Le deuxième élément est introuvable et **ResponseClass** est défini sur **erreur**.</span><span class="sxs-lookup"><span data-stu-id="29a76-146">The second item could not be found, and the **ResponseClass** is set to **Error**.</span></span>
  
```XML
<m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <m:ResponseMessages>
    <m:GetItemResponseMessage ResponseClass="Success">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:Items>
        <t:Message>
          <t:ItemId Id="Er5cAAA="
                    ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/O" />
          <t:Subject>Business plans</t:Subject>
        </t:Message>
      </m:Items>
    </m:GetItemResponseMessage>
    <m:GetItemResponseMessage ResponseClass="Error">
      <m:MessageText>The specified object was not found in the store.</m:MessageText>
      <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      <m:Items />
    </m:GetItemResponseMessage>
  </m:ResponseMessages>
</m:GetItemResponse>
```

<span data-ttu-id="29a76-147">Lorsqu’un ou plusieurs éléments d’une demande groupée ne peuvent pas être traités comme demandé, une erreur est renvoyée pour chaque élément ayant échoué et le reste des éléments dans le lot est traité comme prévu.</span><span class="sxs-lookup"><span data-stu-id="29a76-147">When one or more items in a batched request can't be processed as requested, an error is returned for each item that failed, and the rest of the items in the batch are processed as expected.</span></span> <span data-ttu-id="29a76-148">Des défaillances dans le traitement par lots peuvent se produire si l’élément a été supprimé et, par conséquent, ne peut pas être envoyé, récupéré ou mis à jour, ou si l’élément a été déplacé vers un autre dossier, et par conséquent dispose d’un nouvel ID d’élément.</span><span class="sxs-lookup"><span data-stu-id="29a76-148">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID.</span></span> <span data-ttu-id="29a76-149">Étant donné que l’opération se termine pour certains éléments et qu’elle ne renvoie pas d’erreur lorsqu’un ou plusieurs éléments ne peuvent pas être traités, il est important de vérifier chaque attribut **ResponseClass** avant de passer à l’opération suivante.</span><span class="sxs-lookup"><span data-stu-id="29a76-149">Because the operation will complete for some items and not return an error when one or more items can't be processed, it's important to check each **ResponseClass** attribute before you move on to your next operation.</span></span> 
  
<span data-ttu-id="29a76-150">Si les informations fournies par les éléments de réponse ne vous permettent pas de corriger votre demande ou de vous débloquer, consultez les [étapes suivantes](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="29a76-150">If the information provided by the response elements doesn't help you correct your request or otherwise unblock you, see [Next steps](#bk_nextsteps).</span></span>
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a><span data-ttu-id="29a76-151">Vérification des résultats d’un appel de méthode d’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="29a76-151">Verifying the results of an EWS Managed API method call</span></span>
<span data-ttu-id="29a76-152"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="29a76-152"><a name="bk_successful"> </a></span></span>

<span data-ttu-id="29a76-153">Si vous utilisez l’API managée EWS et appelez une méthode sur un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , votre méthode renverra probablement un objet [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) , qui contient une collection d’objets [ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) ou une collection d’objets dérivés des objets **ServiceResponse** .</span><span class="sxs-lookup"><span data-stu-id="29a76-153">If you're using the EWS Managed API and calling a method on an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, your method will likely return a [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) object, which contains a collection of [ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) objects, or a collection of objects derived from the **ServiceResponse** objects.</span></span> <span data-ttu-id="29a76-154">Les objets **ServiceResponseCollection** et included **ServiceResponse** contiennent des informations sur le résultat de l’appel de méthode, que vous pouvez utiliser pour vérifier vos résultats.</span><span class="sxs-lookup"><span data-stu-id="29a76-154">The **ServiceResponseCollection** and included **ServiceResponse** objects contain information about the result of the method call, which you can use to verify your results.</span></span> 
  
<span data-ttu-id="29a76-155">Si vous utilisez l’API managée EWS et appelez une méthode sur un objet d' [élément](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , ou l’un des objets dérivés, la méthode ne renvoie probablement pas d’objet de réponse pour vérifier la réussite, mais lève une [exception](https://msdn.microsoft.com/library/c18k6c59) si la méthode ne se termine pas correctement.</span><span class="sxs-lookup"><span data-stu-id="29a76-155">If you're using the EWS Managed API and calling a method on an [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object, or one of the derived objects, the method likely does not return a response object to check for success, but does throw an [Exception](https://msdn.microsoft.com/library/c18k6c59) if the method does not complete successfully.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="29a76-156">Vérification de la réussite</span><span class="sxs-lookup"><span data-stu-id="29a76-156">Verifying success</span></span>

<span data-ttu-id="29a76-157">L’un des avantages de l’API managée EWS est qu’elle fournit un état global lorsqu’elle traite plusieurs éléments dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="29a76-157">One benefit of using the EWS Managed API is that it provides an overall status when dealing with multiple items in one response.</span></span> <span data-ttu-id="29a76-158">Par conséquent, si la méthode appelée renvoie un **ServiceResponseCollection**, vous pouvez vérifier que la propriété [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) de l' **ServiceResponseCollection** est égale à [ServiceResult. Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="29a76-158">So if the method you called returns a **ServiceResponseCollection**, you can check that the [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) property of the **ServiceResponseCollection** is equal to [ServiceResult.Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="29a76-159">Si c’est le cas, tous les éléments du processus en lot ont été correctement exécutés ; vous n’avez pas à vérifier chaque objet **ServiceResponse** individuellement.</span><span class="sxs-lookup"><span data-stu-id="29a76-159">If so, all the items in the batched process were completed successfully; you don't have to check each **ServiceResponse** object individually.</span></span> <span data-ttu-id="29a76-160">Si la propriété **OverallResult** n’est pas définie sur **ServiceResult. Success**, vous devez [gérer l’erreur ou l’avertissement](#bk_ewsmaerrors).</span><span class="sxs-lookup"><span data-stu-id="29a76-160">If the **OverallResult** property is not set to **ServiceResult.Success**, you have to [handle the error or warning](#bk_ewsmaerrors).</span></span>
  
<span data-ttu-id="29a76-161">Si la méthode que vous appelez ne renvoie pas d' **ServiceResponseCollection**, mais renvoie un objet **ServiceResponse** , vous devez vérifier la valeur de la propriété **result** .</span><span class="sxs-lookup"><span data-stu-id="29a76-161">If the method you're calling does not return a **ServiceResponseCollection**, but does return a **ServiceResponse** object, you have to check the value of the **Result** property.</span></span> <span data-ttu-id="29a76-162">Si la valeur du **résultat** est définie sur **Success**, vous êtes conscient que la méthode a été exécutée avec succès.</span><span class="sxs-lookup"><span data-stu-id="29a76-162">If the **Result** value is set to **Success**, you know the method completed successfully.</span></span>
  
<span data-ttu-id="29a76-163">Si la méthode que vous appelez n’a pas de valeur de retour, il n’existe pas de moyen de vérifier la réussite via l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="29a76-163">If the method you're calling has no return value, there's really no way to check for success via the EWS Managed API.</span></span> <span data-ttu-id="29a76-164">Tant qu’une exception n’est pas levée, vous pouvez supposer que la méthode a été exécutée avec succès.</span><span class="sxs-lookup"><span data-stu-id="29a76-164">As long as an exception is not thrown, you can assume the method completed successfully.</span></span> <span data-ttu-id="29a76-165">Pour une validation supplémentaire, vous pouvez également [consulter la réponse SOAP pour vérifier les résultats](#bk_verifysoap).</span><span class="sxs-lookup"><span data-stu-id="29a76-165">For additional validation, you can also [check the SOAP response to verify the results](#bk_verifysoap).</span></span>
  
### <a name="handling-errors-warnings-and-exceptions"></a><span data-ttu-id="29a76-166">Gestion des erreurs, des avertissements et des exceptions</span><span class="sxs-lookup"><span data-stu-id="29a76-166">Handling errors, warnings, and exceptions</span></span>
<span data-ttu-id="29a76-167"><a name="bk_ewsmaerrors"> </a></span><span class="sxs-lookup"><span data-stu-id="29a76-167"><a name="bk_ewsmaerrors"> </a></span></span>

<span data-ttu-id="29a76-168">Si votre code d’API managée EWS génère une **exception**, vous pouvez utiliser la valeur d' [exception. message](https://msdn.microsoft.com/library/9btwf6wk) pour déterminer la source de l’erreur.</span><span class="sxs-lookup"><span data-stu-id="29a76-168">If your EWS Managed API code throws an **Exception**, you can use the [Exception.Message](https://msdn.microsoft.com/library/9btwf6wk) value to determine the source of the error.</span></span> <span data-ttu-id="29a76-169">La propriété **message** contient le contenu de l’élément [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) dans la réponse SOAP sous-jacente.</span><span class="sxs-lookup"><span data-stu-id="29a76-169">The **Message** property contains the contents of the [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) element in the underlying SOAP response.</span></span> <span data-ttu-id="29a76-170">En outre, si l’exception est de type [ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) Object, l’une des [exceptions les plus](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) courantes, vous pouvez également récupérer le code d’erreur contenu dans l’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) SOAP sous-jacent et la propriété [Response](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) qui identifie l’objet [ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) associé.</span><span class="sxs-lookup"><span data-stu-id="29a76-170">In addition, if the exception is of type [ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) object, one of the most common exceptions, you can also retrieve the [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contained in the underlying SOAP [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element, and the [Response](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) property that identifies the associated [ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="29a76-171">Le code suivant montre comment intercepter et afficher le contenu d’un **ServiceResponseException**.</span><span class="sxs-lookup"><span data-stu-id="29a76-171">The following code shows how to catch and display the contents of a **ServiceResponseException**.</span></span> 
  
```cs
try
    {
         …
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error code: " + ex.ErrorCode);
        Console.WriteLine("Error message: " + ex.Message);
        Console.WriteLine("Response: " + ex.Response);
    }
```

<span data-ttu-id="29a76-172">Si la méthode appelée renvoie un **ServiceResponseCollection**et que la valeur de la propriété **OverallResult** est égale à **Warning** ou **Error**, vous devrez parcourir chaque objet dans l' **ServiceResponseCollection** pour trouver l’erreur.</span><span class="sxs-lookup"><span data-stu-id="29a76-172">If the method you called returns a **ServiceResponseCollection**, and the value of the **OverallResult** property is equal to **Warning** or **Error**, you'll have to loop through each object in the **ServiceResponseCollection** to find the error.</span></span> <span data-ttu-id="29a76-173">La propriété **OverallResult** est définie sur **Warning** si au moins une réponse a sa valeur de **résultat** définie sur **Warning** et toutes les autres réponses ont leurs valeurs de **résultat** définies sur **Success**.</span><span class="sxs-lookup"><span data-stu-id="29a76-173">The **OverallResult** property is set to **Warning** if at least one response has its **Result** value set to **Warning** and all other responses have their **Result** values set to **Success**.</span></span> <span data-ttu-id="29a76-174">La propriété **OverallResult** est définie sur **erreur** si au moins une réponse a sa valeur de **résultat** définie sur **erreur**.</span><span class="sxs-lookup"><span data-stu-id="29a76-174">The **OverallResult** property is set to **Error** if at least one response has its **Result** value set to **Error**.</span></span> <span data-ttu-id="29a76-175">Lorsque **OverallResult** est défini sur **Warning** ou **Error**, les propriétés suivantes sont définies sur les objets **ServiceResponse** , selon le cas :</span><span class="sxs-lookup"><span data-stu-id="29a76-175">When the **OverallResult** is set to **Warning** or **Error**, the following properties are set on the **ServiceResponse** objects as appropriate:</span></span> 
  
- <span data-ttu-id="29a76-176">[ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — contient le code d’erreur, qui peut être utilisé pour trouver des ressources de résolution des problèmes supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="29a76-176">[ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="29a76-177">[ErrorDetails](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) : contient les détails relatifs à l’erreur pour certains **errorCodes**.</span><span class="sxs-lookup"><span data-stu-id="29a76-177">[ErrorDetails](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — Contains details about the error for some **ErrorCodes**.</span></span> <span data-ttu-id="29a76-178">Par exemple, lorsque le code d’erreur est **ErrorRecurrenceHasNoOccurrence**, le **ErrorDetails** contient des clés pour **EffectiveStartDate** et **EffectiveEndDate**.</span><span class="sxs-lookup"><span data-stu-id="29a76-178">For example, when the error code is **ErrorRecurrenceHasNoOccurrence**, the **ErrorDetails** will contain keys for **EffectiveStartDate** and **EffectiveEndDate**.</span></span> 
    
- <span data-ttu-id="29a76-179">[ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — décrit l’erreur.</span><span class="sxs-lookup"><span data-stu-id="29a76-179">[ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="29a76-180">[ErrorProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — le cas échéant, identifie les propriétés à l’origine de l’erreur.</span><span class="sxs-lookup"><span data-stu-id="29a76-180">[ErrorProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — If available, identifies the properties that caused the error.</span></span> <span data-ttu-id="29a76-181">Par exemple, lorsque le code d’erreur est **ErrorInvalidPropertyForOperation**, **ErrorProperties** contient la définition de la propriété qui n’était pas valide pour la demande.</span><span class="sxs-lookup"><span data-stu-id="29a76-181">For example, when the error code is **ErrorInvalidPropertyForOperation**, **ErrorProperties** contains the definition of the property that was invalid for the request.</span></span> 
    
- <span data-ttu-id="29a76-182">[Result](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — contient une **erreur** ou un **Avertissement** lorsqu’un problème est rencontré.</span><span class="sxs-lookup"><span data-stu-id="29a76-182">[Result](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — Contains **Error** or **Warning** when an issue is encountered.</span></span> 
    
<span data-ttu-id="29a76-183">Si les informations fournies par les propriétés **ServiceResponse** ne fournissent pas suffisamment d’informations pour corriger votre appel de méthode ou vous débloquer, consultez les [étapes suivantes](#bk_nextsteps) pour plus d’informations sur les valeurs **ErrorCode** .</span><span class="sxs-lookup"><span data-stu-id="29a76-183">If the information provided by the **ServiceResponse** properties doesn't provide enough information to correct your method call or unblock you, see [Next steps](#bk_nextsteps) to dig up more information on **ErrorCode** values.</span></span> 
  
## 
<span data-ttu-id="29a76-184"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="29a76-184"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="29a76-185">Vous pouvez rechercher des informations de dépannage supplémentaires dans les rubriques suivantes :</span><span class="sxs-lookup"><span data-stu-id="29a76-185">You can look up additional troubleshooting information in the following topics:</span></span>
  
- <span data-ttu-id="29a76-186">Élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="29a76-186">[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element</span></span> 
    
- <span data-ttu-id="29a76-187">[ServiceError](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) , énumération</span><span class="sxs-lookup"><span data-stu-id="29a76-187">[ServiceError](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) enumeration</span></span> 
    
- [<span data-ttu-id="29a76-188">Erreurs liées aux propriétés EWS</span><span class="sxs-lookup"><span data-stu-id="29a76-188">EWS property-related errors</span></span>](ews-property-related-errors.md)
    
<span data-ttu-id="29a76-189">En outre, en fonction de ce que vous essayez d’effectuer dans votre demande, vous trouverez des informations utiles supplémentaires sur le code d’erreur dans les rubriques suivantes :</span><span class="sxs-lookup"><span data-stu-id="29a76-189">In addition, depending on what you're trying to accomplish in your request, you might find additional helpful information about the error code in the following topics:</span></span>
  
- [<span data-ttu-id="29a76-190">Gestion des messages d'erreur de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="29a76-190">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="29a76-191">Gestion des erreurs liées à la notification dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="29a76-191">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="29a76-192">Gestion des erreurs liées à la synchronisation dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="29a76-192">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="29a76-193">Gestion des erreurs liées à la suppression dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="29a76-193">Handling deletion-related errors in EWS in Exchange</span></span>](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="29a76-194">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="29a76-194">See also</span></span>


- [<span data-ttu-id="29a76-195">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="29a76-195">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="29a76-196">Outils et ressources pour la résolution des applications EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="29a76-196">Tools and resources for troubleshooting EWS applications for Exchange</span></span>](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

