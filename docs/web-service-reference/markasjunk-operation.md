---
title: MarkAsJunk Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Opération de recherche plus d’informations sur la MarkAsJunk EWS.
ms.openlocfilehash: b9d79e6fbec87ce41030b4981f3c16f2f9ce9507
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828353"
---
# <a name="markasjunk-operation"></a>MarkAsJunk Operation

Trouvez des informations sur l’opération EWS **MarkAsJunk** . 
  
L’opération **MarkAsJunk** ajoute et supprime les utilisateurs de la liste de courrier électronique bloqué et déplace les messages électroniques vers le dossier courrier indésirable. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-markasjunk-operation"></a>Utilisation de l’opération MarkAsJunk

L’opération **MarkAsJunk** contient deux options de type Boolean pour indiquer si un expéditeur de courrier électronique doit être ajouté à la liste des expéditeurs bloqués et si le message électronique cible doit être déplacé vers le dossier de courrier indésirable par défaut ou le dossier boîte de réception. Les actions sont déterminées par les valeurs des attributs **IsJunk** et **MoveItem** . Basée sur les combinaisons de valeurs pour les attributs **IsJunk** et **MoveItem** actions possibles sont les suivantes : 
  
- Si l’attribut **IsJunk** est défini sur **true**, et l’attribut **MoveItem** est défini sur **true**, l’expéditeur du message électronique cible est ajouté à la liste des expéditeurs bloqués et le message électronique est déplacé vers le dossier Dmail indésirable.
    
- Si l’attribut **IsJunk** est défini sur **true**, et l’attribut **MoveItem** est défini sur **false**, l’expéditeur du message électronique cible est ajouté à la liste des expéditeurs bloqués et le message électronique n’est pas déplacé à partir du dossier.
    
- Si l’attribut **IsJunk** a la valeur **false**et la **MoveItem** attribut est défini sur **true**, l’expéditeur de le messageis de messagerie cible supprimé de la liste des expéditeurs bloqués et le message électronique est déplacé vers le dossier boîte de réception.
    
- Si l’attribut **IsJunk** est défini sur **false**, et l’attribut **MoveItem** est défini sur **false**, l’expéditeur du message électronique cible est supprimé de la liste des expéditeurs bloqués et le message électronique n’est pas déplacé à partir du dossier.
    
> [!IMPORTANT]
> Le contenu de la liste des expéditeurs bloqués n’est pas accessibles à partir de EWS. Si un expéditeur est ajouté à la liste des expéditeurs bloqués, vous devez conserver une copie d’un message électronique envoyé par l’expéditeur bloqué à débloquer l’expéditeur à l’avenir. 
  
### <a name="markasjunk-operation-soap-headers"></a>En-têtes SOAP MarkAsJunk opération

L’opération **MarkAsJunk** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente. Cet en-tête est applicable à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête est applicable à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a>Exemple de requête d’opération MarkAsJunk : ajouter un expéditeur à la liste des expéditeurs bloqués

Une demande d’opération **MarkAsJunk** l’exemple suivant montre comment ajouter l’expéditeur d’un message électronique à la liste des expéditeurs bloqués et déplacer le courrier électronique vers le dossier courrier indésirable. L’opération **MarkAsJunk** accepte l’identificateur de message électronique unique pour identifier le courrier électronique qui est utilisé pour faire référence à l’expéditeur est ajouté à la liste des expéditeurs bloqués. 
  
> [!NOTE]
> Tous les identificateurs d’article et modifier des clés dans cet article ont été réduits afin de préserver la lisibilité. 
  
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
        <m:MarkAsJunk IsJunk="true" MoveItem="true">
            <m:ItemIds>
                <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYA" />
            </m:ItemIds>
        </m:MarkAsJunk>
    </soap:Body>
</soap:Envelope>

```

La demande SOAP body contient les éléments suivants :
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemId](itemids.md)
    
- [ID d’élément](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a>Réponse d’opération MarkAsJunk réussie

L’exemple suivant montre une réponse positive à une demande d’opération **MarkAsJunk** pour ajouter un expéditeur à la liste des expéditeurs bloqués et de déplacer le message vers le dossier courrier indésirable. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                             MinorVersion="0" 
                             MajorBuildNumber="545" 
                             MinorBuildNumber="11" 
                             Version="Exchange2013" 
                             xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                             xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
        <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
           <m:ResponseMessages>
               <m:MarkAsJunkResponseMessage ResponseClass="Success">
                  <m:ResponseCode>NoError</m:ResponseCode>
                 <m:MovedItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
               </m:MarkAsJunkResponseMessage>
           </m:ResponseMessages>
        </m:MarkAsJunkResponse>
    </s:Body>
</s:Envelope>
```

La réponse SOAP body contient les éléments suivants :
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [MovedItemId](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a>Exemple de requête d’opération MarkAsJunk : supprimer un expéditeur de la liste des expéditeurs bloqués

Une demande d’opération **MarkAsJunk** l’exemple suivant montre comment supprimer l’expéditeur d’un message électronique à partir de la liste des expéditeurs bloqués et de déplacer le message électronique vers le dossier boîte de réception. Vous devez conserver un message électronique envoyé par l’expéditeur bloqué pour supprimer l’expéditeur de la liste des expéditeurs bloqués. Adresse de messagerie de l’expéditeur est associé à des messages électroniques qui ont été envoyés par l’expéditeur. Suppression d’un expéditeur dans la liste des expéditeurs bloqués ne fonctionnera pas si le message électronique de référence n’existe plus dans la boîte aux lettres de l’utilisateur. L’identificateur d’élément utilisé pour associer un message électronique à l’expéditeur doit être associé à un élément qui existe dans la boîte aux lettres Exchange. Nous vous conseillons de créer un dossier masqué pour stocker les éléments envoyés par des expéditeurs bloqués précédemment afin que les expéditeurs peuvent être non bloqués à partir de l’application cliente. Dans le cas où un élément est supprimé de la boîte aux lettres Exchange, un administrateur doit utiliser la Console de gestion Exchange pour accéder à la liste des expéditeurs bloqués pour supprimer un expéditeur de la liste. Pour plus d’informations sur comment débloquer un utilisateur à l’aide de la Console de gestion Exchange, voir [comment configurer l’expéditeurs fiables et expéditeurs bloqués dans Office 365](http://support.microsoft.com/kb/2545137).
  
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
      <m:MarkAsJunk IsJunk="false" MoveItem="true">
        <m:ItemIds>
          <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
        </m:ItemIds>
      </m:MarkAsJunk>
    </soap:Body>
 </soap:Envelope>

```

Une réponse positive de suppression d’un expéditeur dans la liste des expéditeurs bloqués est la même que la réponse à l’ajout d’un expéditeur à la liste des expéditeurs bloqués.
  
La demande SOAP body contient les éléments suivants :
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemId](itemids.md)
    
- [ID d’élément](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a>Réponse d’erreur d’opération MarkAsJunk

L’exemple suivant montre une réponse d’erreur à une demande d’opération **MarkAsJunk** . Il s’agit d’une réponse à une demande pour ajouter ou supprimer un expéditeur dans la liste des expéditeurs bloqués lorsque le message électronique spécifié par l’identificateur d’élément n’existe plus dans la boîte aux lettres. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="545" 
                         MinorBuildNumber="11" 
                         Version="Exchange2013" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

La réponse d’erreur corps SOAP contient les éléments suivants :
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [GetItem operation](getitem-operation.md) Opération GetItem 
    
- [Opération FindItem](finditem-operation.md)
    

