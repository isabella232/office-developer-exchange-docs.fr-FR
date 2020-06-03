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
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a>Vérification des résultats d’un appel EWS ou API managée EWS

Découvrez comment vérifier les résultats de vos appels EWS ou API managée EWS.
  
Lorsque les éléments ne fonctionnent pas correctement, il est utile de voir ce qui se passe en examinant les demandes SOAP que votre application envoie sur le réseau et les réponses renvoyées par le serveur. L’article [Outils et ressources pour la résolution des problèmes liés aux applications EWS](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) inclut des liens vers des outils permettant de capturer et d’afficher ces demandes SOAP. Une fois que vous avez reçu les requêtes et les réponses, comment vérifier que la demande que vous avez envoyée au serveur a été correctement traitée ? Lisez la suite pour en savoir plus. 
  
Si vous envoyez des demandes EWS, vous allez démarrer votre vérification en vérifiant l’attribut **ResponseClass** pour chaque message de réponse dans la réponse. Cela vous permettra de savoir si l’opération s’est terminée avec succès sur chaque élément. 
  
En fonction de l’objet que votre méthode appelle, si vous utilisez l’API managée EWS pour envoyer des demandes, vous pouvez effectuer une vérification à l’aide des objets Response. Toutefois, étant donné que la réponse SOAP contient un sur-ensemble de ce qui est inclus dans les objets de réponse de l’API managée EWS, vous pouvez également consulter la réponse SOAP. Étant donné que la réponse SOAP peut souvent contenir plus d’informations que les objets de réponse de l’API managée EWS, commencez votre vérification avec la réponse SOAP.
  
## <a name="verifying-the-results-of-a-soap-response"></a>Vérification des résultats d’une réponse SOAP
<a name="bk_verifysoap"> </a>

Lorsque vous recevez une réponse SOAP, la première chose à examiner est l’attribut **ResponseClass** . Cet attribut est inclus dans chaque instance **ResponseMessageType** de l’élément [ResponseMessages](https://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) , comme illustré dans l’exemple suivant. 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

Étant donné qu’une réponse SOAP peut contenir plusieurs messages de réponse dans une réponse SOAP unique, il est important de vérifier chaque message de réponse individuellement.
  
Si vous utilisez une opération qui inclut un **ResponseClass** dans le cadre de la réponse de l’opération, comme suit, vous pouvez être tenté de vérifier uniquement les **ResponseClass** de l’opération. 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

Toutefois, l’état de l’opération reflète uniquement la forme de la réponse de niveau supérieur et ne reflète pas l’état de toutes les réponses de message individuelles. Dans l’exemple suivant, l’opération [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) a un **ResponseClass** de **succès**, mais l’élément [DelegateUserResponseMessageType](https://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) sous-jacent a une valeur **ResponseClass** de l' **erreur**.
  
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

Ainsi, pour les réponses de SOAP EWS, vous ne pouvez pas compter sur le **ResponseClass** de l’opération : vous devez examiner les **ResponseClass** de chaque message de réponse pour déterminer si l’opération a rencontré des erreurs lors du traitement des éléments. 
  
### <a name="verifying-success"></a>Vérification de la réussite

Si chaque attribut **ResponseClass** de chaque attribut **ResponseMessage** est défini sur **Success**, l’opération s’est terminée avec succès sur tous les éléments, et vous pouvez passer à votre tâche suivante.
  
L’exemple suivant montre une réponse réussie à une demande d’opération [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) pour récupérer un élément unique. Notez que lorsque **ResponseClass** est défini sur **Success**, le [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) associé est toujours défini sur **NOERROR**.
  
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

Voici une réponse réussie à une demande d’opération **GetItem** pour récupérer plusieurs éléments. Chacun des éléments [GetItemResponseMessage](https://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) a une **ResponseClass** de **réussite**.
  
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

### <a name="handling-errors-and-warnings"></a>Gestion des erreurs et des avertissements

Lorsque vous recevez une réponse et que l’attribut **ResponseClass** est défini sur **Error**, l’opération ne s’est pas terminée correctement sur un ou plusieurs éléments. Corrigez le problème et renouvelez votre demande, ou la partie de votre demande qui a échoué. La valeur d' **Avertissement** d’un attribut **ResponseClass** est renvoyée par l’opération [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) uniquement et indique que l’entité n’a pas pu être résolue en une identité unique. Vous pouvez l’ignorer pour toutes les autres opérations. 
  
Dans la réponse suivante, l’attribut **ResponseClass** a une valeur d' **erreur**.
  
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

Dans cet exemple, EWS fournit des indices pour déboguer le problème. Lorsque l’attribut **ResponseClass** a une valeur d' **erreur**, les éléments supplémentaires suivants sont inclus dans la réponse, le cas échéant :
  
- [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — décrit l’erreur. 
    
- [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — contient le code d’erreur, qui peut être utilisé pour trouver des ressources de résolution des problèmes supplémentaires. 
    
- [Messagexml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — identifie les éléments à l’origine de l’erreur. 
    
- [DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) : non utilisé. 
    
Vous pouvez utiliser les informations fournies dans ces éléments pour examiner votre problème. Dans l’exemple précédent, l' **MessageText** indique que la propriété n’est pas valide pour le type d’objet. La demande consistait à obtenir un message électronique, mais le jeu de propriétés comprenait **AssociatedCalendarItemId**, ce qui est uniquement valide pour les éléments de rendez-vous.
  
L’exemple suivant montre une erreur qui a été reçue dans le cadre d’une opération par lots pour obtenir plusieurs éléments de courrier électronique. Le premier élément a été récupéré avec succès et **ResponseClass** est défini sur **Success**. Le deuxième élément est introuvable et **ResponseClass** est défini sur **erreur**.
  
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

Lorsqu’un ou plusieurs éléments d’une demande groupée ne peuvent pas être traités comme demandé, une erreur est renvoyée pour chaque élément ayant échoué et le reste des éléments dans le lot est traité comme prévu. Des défaillances dans le traitement par lots peuvent se produire si l’élément a été supprimé et, par conséquent, ne peut pas être envoyé, récupéré ou mis à jour, ou si l’élément a été déplacé vers un autre dossier, et par conséquent dispose d’un nouvel ID d’élément. Étant donné que l’opération se termine pour certains éléments et qu’elle ne renvoie pas d’erreur lorsqu’un ou plusieurs éléments ne peuvent pas être traités, il est important de vérifier chaque attribut **ResponseClass** avant de passer à l’opération suivante. 
  
Si les informations fournies par les éléments de réponse ne vous permettent pas de corriger votre demande ou de vous débloquer, consultez les [étapes suivantes](#bk_nextsteps).
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a>Vérification des résultats d’un appel de méthode d’API managée EWS
<a name="bk_successful"> </a>

Si vous utilisez l’API managée EWS et appelez une méthode sur un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , votre méthode renverra probablement un objet [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) , qui contient une collection d’objets [ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) ou une collection d’objets dérivés des objets **ServiceResponse** . Les objets **ServiceResponseCollection** et included **ServiceResponse** contiennent des informations sur le résultat de l’appel de méthode, que vous pouvez utiliser pour vérifier vos résultats. 
  
Si vous utilisez l’API managée EWS et appelez une méthode sur un objet d' [élément](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , ou l’un des objets dérivés, la méthode ne renvoie probablement pas d’objet de réponse pour vérifier la réussite, mais lève une [exception](https://msdn.microsoft.com/library/c18k6c59) si la méthode ne se termine pas correctement. 
  
### <a name="verifying-success"></a>Vérification de la réussite

L’un des avantages de l’API managée EWS est qu’elle fournit un état global lorsqu’elle traite plusieurs éléments dans une réponse. Par conséquent, si la méthode appelée renvoie un **ServiceResponseCollection**, vous pouvez vérifier que la propriété [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) de l' **ServiceResponseCollection** est égale à [ServiceResult. Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx). Si c’est le cas, tous les éléments du processus en lot ont été correctement exécutés ; vous n’avez pas à vérifier chaque objet **ServiceResponse** individuellement. Si la propriété **OverallResult** n’est pas définie sur **ServiceResult. Success**, vous devez [gérer l’erreur ou l’avertissement](#bk_ewsmaerrors).
  
Si la méthode que vous appelez ne renvoie pas d' **ServiceResponseCollection**, mais renvoie un objet **ServiceResponse** , vous devez vérifier la valeur de la propriété **result** . Si la valeur du **résultat** est définie sur **Success**, vous êtes conscient que la méthode a été exécutée avec succès.
  
Si la méthode que vous appelez n’a pas de valeur de retour, il n’existe pas de moyen de vérifier la réussite via l’API managée EWS. Tant qu’une exception n’est pas levée, vous pouvez supposer que la méthode a été exécutée avec succès. Pour une validation supplémentaire, vous pouvez également [consulter la réponse SOAP pour vérifier les résultats](#bk_verifysoap).
  
### <a name="handling-errors-warnings-and-exceptions"></a>Gestion des erreurs, des avertissements et des exceptions
<a name="bk_ewsmaerrors"> </a>

Si votre code d’API managée EWS génère une **exception**, vous pouvez utiliser la valeur d' [exception. message](https://msdn.microsoft.com/library/9btwf6wk) pour déterminer la source de l’erreur. La propriété **message** contient le contenu de l’élément [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) dans la réponse SOAP sous-jacente. En outre, si l’exception est de type [ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) Object, l’une des [exceptions les plus](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) courantes, vous pouvez également récupérer le code d’erreur contenu dans l’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) SOAP sous-jacent et la propriété [Response](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) qui identifie l’objet [ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) associé. Le code suivant montre comment intercepter et afficher le contenu d’un **ServiceResponseException**. 
  
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

Si la méthode appelée renvoie un **ServiceResponseCollection**et que la valeur de la propriété **OverallResult** est égale à **Warning** ou **Error**, vous devrez parcourir chaque objet dans l' **ServiceResponseCollection** pour trouver l’erreur. La propriété **OverallResult** est définie sur **Warning** si au moins une réponse a sa valeur de **résultat** définie sur **Warning** et toutes les autres réponses ont leurs valeurs de **résultat** définies sur **Success**. La propriété **OverallResult** est définie sur **erreur** si au moins une réponse a sa valeur de **résultat** définie sur **erreur**. Lorsque **OverallResult** est défini sur **Warning** ou **Error**, les propriétés suivantes sont définies sur les objets **ServiceResponse** , selon le cas : 
  
- [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — contient le code d’erreur, qui peut être utilisé pour trouver des ressources de résolution des problèmes supplémentaires. 
    
- [ErrorDetails](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) : contient les détails relatifs à l’erreur pour certains **errorCodes**. Par exemple, lorsque le code d’erreur est **ErrorRecurrenceHasNoOccurrence**, le **ErrorDetails** contient des clés pour **EffectiveStartDate** et **EffectiveEndDate**. 
    
- [ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — décrit l’erreur. 
    
- [ErrorProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — le cas échéant, identifie les propriétés à l’origine de l’erreur. Par exemple, lorsque le code d’erreur est **ErrorInvalidPropertyForOperation**, **ErrorProperties** contient la définition de la propriété qui n’était pas valide pour la demande. 
    
- [Result](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — contient une **erreur** ou un **Avertissement** lorsqu’un problème est rencontré. 
    
Si les informations fournies par les propriétés **ServiceResponse** ne fournissent pas suffisamment d’informations pour corriger votre appel de méthode ou vous débloquer, consultez les [étapes suivantes](#bk_nextsteps) pour plus d’informations sur les valeurs **ErrorCode** . 
  
## 
<a name="bk_nextsteps"> </a>

Vous pouvez rechercher des informations de dépannage supplémentaires dans les rubriques suivantes :
  
- Élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 
    
- [ServiceError](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) , énumération 
    
- [Erreurs liées aux propriétés EWS](ews-property-related-errors.md)
    
En outre, en fonction de ce que vous essayez d’effectuer dans votre demande, vous trouverez des informations utiles supplémentaires sur le code d’erreur dans les rubriques suivantes :
  
- [Gestion des messages d'erreur de découverte automatique](handling-autodiscover-error-messages.md)
    
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la synchronisation dans EWS dans Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Outils et ressources pour la résolution des applications EWS pour Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

