---
title: Vérification des résultats d’un appel EWS ou API managées
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78a1741c-1bbe-4cb4-9331-9d6d3171fc11
description: Découvrez comment vérifier les résultats de vos appels API managées EWS.
ms.openlocfilehash: 077dd923710a1a7f5cad4c822cbbd58ab3603661
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755077"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a>Vérification des résultats d’un appel EWS ou API managées

Découvrez comment vérifier les résultats de vos appels API managées EWS.
  
Lorsque les choses ne fonctionnent pas correctement, il est utile de voir ce qui se passe en examinant les demandes SOAP qui envoie sur le réseau et les réponses que le serveur envoie dans votre application. L’article [Outils et ressources pour la résolution des problèmes des applications EWS](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) inclut des liens vers les outils permettant de capturer et d’afficher les demandes SOAP. Une fois que vous avez les demandes et les réponses, comment vérifier que la demande que vous avez envoyée au serveur a été correctement traitée ? Découvrez. 
  
Si vous envoyez des demandes EWS, vous allez démarrer la vérification en vérifiant l’attribut **ResponseClass** pour chaque message de réponse dans la réponse. Qui indique si l’opération terminée avec succès sur chaque élément. 
  
En fonction de l’objet que votre méthode d’appel, si vous utilisez l’API managée EWS pour envoyer des demandes, vous pouvez effectuer une vérification à l’aide des objets de la réponse. Mais étant donné que la réponse SOAP contient un sur-ensemble de ce qui est inclus dans les objets de réponse d’API managées, vous voudrez peut-être examiner ainsi que la réponse SOAP. Étant donné que la réponse SOAP peut contenir souvent davantage d’informations que les objets de réponse d’API managées, démarrez la vérification de votre avec la réponse SOAP.
  
## <a name="verifying-the-results-of-a-soap-response"></a>Vérification des résultats d’une réponse SOAP
<a name="bk_verifysoap"> </a>

Lorsque vous recevez une réponse SOAP, la première chose à examiner est l’attribut **ResponseClass** . Cet attribut est inclus dans chaque instance **ResponseMessageType** dans l’élément [ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) , comme illustré dans l’exemple suivant. 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

Car une réponse SOAP peut contenir plusieurs messages de réponse à une réponse SOAP unique, il est important de vérifier chaque message de réponse individuellement.
  
Si vous travaillez avec une opération qui inclut un **ResponseClass** dans le cadre de la réponse de l’opération, l’exemple suivant, vous pouvez être tenté de ne vérifier que le **ResponseClass** de l’opération. 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

Toutefois, l’état d’opération reflète la forme de la réponse de niveau supérieur uniquement et ne reflète pas l’état de toutes les réponses de chaque message. Dans l’exemple suivant, l’opération [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) a un **ResponseClass** de **succès**, mais l’élément [DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) sous-jacent a la valeur **ResponseClass** **erreur**.
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Donc pour les réponses SOAP EWS, vous ne pouvez pas s’appuient sur le **ResponseClass** de l’opération : vous devez consulter la **ResponseClass** de chaque message de réponse pour déterminer si l’opération a rencontré des erreurs de traitement des éléments. 
  
### <a name="verifying-success"></a>Vérification de la réussite

Si chaque attribut **ResponseClass** pour chaque attribut **ResponseMessage** est défini sur **succès**, l’opération correctement effectuée sur tous les éléments, et vous pouvez passer à la tâche suivante.
  
L’exemple suivant montre une réponse positive à une demande d’opération [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) pour récupérer un seul élément. Notez que lorsque la **ResponseClass** est défini sur **succès**, le associée [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) est toujours définie sur **NoError**.
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Vous trouverez ci-dessous une réponse positive à une demande d’opération **GetItem** pour récupérer plusieurs éléments. Chacun des éléments de [GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) a un **ResponseClass** de **succès**.
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="handling-errors-and-warnings"></a>Gestion des erreurs et avertissements

Lorsque vous recevez une réponse et l’attribut **ResponseClass** est définie sur **erreur**, l’opération a échoué sur un ou plusieurs éléments. Corriger le problème et réessayez votre demande, ou la partie de votre demande a échoué. Une valeur de l’attribut **ResponseClass** de valeur **d’Avertissement** est renvoyée uniquement par l’opération [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) et indique que l’entité ne peut pas être résolue en une identité unique. Vous pouvez ignorer pour toutes les autres opérations. 
  
Dans la réponse suivante, l’attribut **ResponseClass** a une valeur **d’erreur**.
  
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

Dans cet exemple, EWS fournit des indications pour déboguer le problème. Lorsque l’attribut **ResponseClass** a la valeur **d’erreur**, les éléments supplémentaires suivants sont inclus dans la réponse, le cas échéant :
  
- [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — décrit l’erreur. 
    
- [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — contient le code d’erreur qui peut être utilisé pour rechercher des ressources de dépannage supplémentaires. 
    
- [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — identifie les éléments qui a provoqué l’erreur. 
    
- [DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — inutilisés. 
    
Vous pouvez utiliser les informations fournies dans ces éléments à étudier votre problème. Dans l’exemple précédent, le **MessageText** indique que la propriété n’est pas valide pour le type d’objet. La demande a été pour obtenir un message électronique, mais le jeu de propriétés inclus **AssociatedCalendarItemId**, qui est uniquement valide pour les éléments de rendez-vous.
  
L’exemple suivant montre une erreur qui a été reçue dans le cadre d’une opération par lot pour obtenir plusieurs éléments de courrier électronique. Le premier élément a été récupéré avec succès et le **ResponseClass** est défini sur **succès**. Impossible de trouver le deuxième élément, et le **ResponseClass** est définie sur **l’erreur**.
  
```XML
<m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Lorsqu’un ou plusieurs éléments dans une requête par lot ne peut pas être traités, une erreur est renvoyée pour chaque élément qui a échoué, et le reste des éléments dans le lot sont traitées comme prévu. Échecs dans le traitement par lots peuvent se produire si l’élément a été supprimé et par conséquent ne peut pas être envoyé, récupéré ou mis à jour, ou si l’élément déplacé vers un autre dossier et par conséquent ne possède un nouvel ID d’élément. Étant donné que l’opération sera exécuté pour certains éléments et renvoie pas d’erreur lorsqu’un ou plusieurs éléments ne peuvent pas être traitées, il est important de vérifier chaque attribut **ResponseClass** avant de passer à l’opération suivante. 
  
Si les informations fournies par les éléments de réponse ne vous aider à résoudre votre demande ou débloquer sinon vous, voir les [étapes suivantes](#bk_nextsteps).
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a>Vérification des résultats d’un appel de méthode d’API managées
<a name="bk_successful"> </a>

Si vous êtes à l’aide de l’API managée EWS et appelez une méthode sur un objet [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , votre méthode renverra probablement un objet [ServiceResponseCollection](http://msdn.microsoft.com/EN-US/library/dd633715%28v=exchg.80%29.aspx) , qui contient une collection d’objets [ServiceResponse](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) , soit une collection de objets dérivés à partir des objets **ServiceResponse** . Les **ServiceResponseCollection** et les objets **ServiceResponse** inclus contiennent des informations sur le résultat de l’appel de méthode, vous pouvez utiliser pour vérifier les résultats. 
  
Si vous êtes à l’aide de l’API managée EWS et appelez une méthode sur un objet [d’élément](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , ou un des objets dérivés, la méthode susceptible de ne renvoie pas un objet de réponse pour vérifier le succès, mais lève une [Exception](http://msdn.microsoft.com/EN-US/library/c18k6c59) si la méthode ne se termine pas avec succès. 
  
### <a name="verifying-success"></a>Vérification de la réussite

L’un des avantages de l’utilisation de l’API managée EWS sont qu’il fournit un état global lorsque vous travaillez avec plusieurs éléments dans une réponse. Ainsi, si la méthode que vous avez appelé renvoie une **ServiceResponseCollection**, vous pouvez vérifier que la propriété [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) de la **ServiceResponseCollection** est égale à [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx). Dans ce cas, tous les éléments dans le processus de mise en lots ont été correctement effectuées ; vous n’êtes pas obligé de vérifier chaque objet **ServiceResponse** individuellement. Si la propriété **OverallResult** n’est pas définie à **ServiceResult.Success**, vous devez [gérer l’erreur ou avertissement](#bk_ewsmaerrors).
  
Si la méthode que vous appelez ne renvoie pas un **ServiceResponseCollection**, mais renvoie un objet **ServiceResponse** , vous devez vérifier la valeur de la propriété **Result** . Si la valeur de **résultat de** **Réussite**, vous connaissez la méthode s’est terminée correctement.
  
Si la méthode que vous appelez ne renvoie aucune valeur, il n’est vraiment aucun moyen de vérifier le succès via l’API managée EWS. Dans la mesure où une exception est levée pas, vous pouvez supposer que la méthode s’est terminée correctement. Pour une validation supplémentaire, vous pouvez également [vérifier la réponse SOAP pour vérifier les résultats](#bk_verifysoap).
  
### <a name="handling-errors-warnings-and-exceptions"></a>Gestion des erreurs, avertissements et exceptions
<a name="bk_ewsmaerrors"> </a>

Si votre code d’API managées lève une **Exception**, vous pouvez utiliser la valeur [Exception.Message](http://msdn.microsoft.com/EN-US/library/9btwf6wk) pour déterminer la source de l’erreur. La propriété **Message** contient le contenu de l’élément [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) dans la réponse SOAP sous-jacent. En outre, si l’exception est de type object [ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) , une des exceptions plus courantes, vous pouvez également récupérer [ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contenues dans l’élément SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) sous-jacent et de la [réponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) propriété qui identifie l’objet [ServiceResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) associé. Le code suivant montre comment intercepter et afficher le contenu d’un **ServiceResponseException**. 
  
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

Si la méthode appelée renvoie une **ServiceResponseCollection**, et la valeur de la propriété **OverallResult** est égale à **Avertissement** ou **erreur**, vous devrez une boucle sur chaque objet de la **ServiceResponseCollection** à Recherchez l’erreur. La propriété **OverallResult** est définie à **Avertissement** si au moins une réponse a la valeur **résultat** **Avertissement** et toutes les autres réponses que leurs valeurs **résultat** **Réussite**. La propriété **OverallResult** est définie à une **erreur** si au moins une réponse a la valeur **résultat** à **l’erreur**. Lorsque **OverallResult** est défini sur **Avertissement** ou **erreur**, les propriétés suivantes sont définies sur les objets **ServiceResponse** selon le cas : 
  
- [ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — contient le code d’erreur qui peut être utilisé pour rechercher des ressources de dépannage supplémentaires. 
    
- [ErrorDetails](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — contient plus d’informations sur l’erreur pour certains **ErrorCodes**. Par exemple, lorsque le code d’erreur est **ErrorRecurrenceHasNoOccurrence**, **ErrorDetails** contiendra des clés pour **EffectiveStartDate** et **EffectiveEndDate**. 
    
- [ErrorMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — décrit l’erreur. 
    
- [ErrorProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — si elle est disponible, identifie les propriétés qui a provoqué l’erreur. Par exemple, lorsque le code d’erreur est **ErrorInvalidPropertyForOperation**, **ErrorProperties** contient la définition de la propriété qui n’était pas valide pour la demande. 
    
- [Résultat](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — contient **erreur** ou **Avertissement** lorsqu’un problème est détecté. 
    
Si les informations fournies par les propriétés **ServiceResponse** ne fournissent pas suffisamment d’informations pour corriger votre appel de méthode ou vous débloquer, voir les [étapes](#bk_nextsteps) récupère des plus d’informations sur les valeurs de **code d’erreur** . 
  
## 
<a name="bk_nextsteps"> </a>

Vous pouvez rechercher des informations de dépannage supplémentaires dans les rubriques suivantes :
  
- Élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 
    
- Énumération [constatez](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 
    
- [Erreurs liées à la propriété EWS](ews-property-related-errors.md)
    
En outre, selon ce que vous cherchez à exécuter dans votre requête, vous pouvez trouver plus d’informations utiles sur le code d’erreur dans les rubriques suivantes :
  
- [Gestion des messages d'erreur de découverte automatique](handling-autodiscover-error-messages.md)
    
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la synchronisation dans EWS dans Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées aux suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Outils et ressources pour la résolution des applications EWS pour Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

