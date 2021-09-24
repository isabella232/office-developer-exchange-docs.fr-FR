---
title: Opération MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Trouvez des informations sur l’opération EWS MarkAsJunk.
ms.openlocfilehash: b165b415ce9380846b49d15dd321bfddba72b749
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524734"
---
# <a name="markasjunk-operation"></a>Opération MarkAsJunk

Trouvez des informations sur l’opération EWS **MarkAsJunk.** 
  
**L’opération MarkAsJunk** ajoute et supprime les utilisateurs de la liste des messages bloqués et déplace les messages électroniques vers le dossier Courrier indésirable. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-markasjunk-operation"></a>Utilisation de l’opération MarkAsJunk

L’opération **MarkAsJunk** contient deux options booléques pour indiquer si un expéditeur de courrier électronique doit être ajouté à la liste des expéditeurs bloqués et si le message électronique cible doit être déplacé vers le dossier Courrier indésirable par défaut ou le dossier Boîte de réception. Les actions sont déterminées par les valeurs des **attributs IsJunk** et **MoveItem.** Les actions possibles basées sur les combinaisons de valeurs pour les attributs **IsJunk** et **MoveItem** sont les suivantes : 
  
- Si l’attribut **IsJunk** est définie sur true et que l’attribut **MoveItem** est définie sur **true,** l’expéditeur du message électronique cible est ajouté à la liste des expéditeurs bloqués et le message électronique est déplacé vers le dossier Courrier indésirable. 
    
- Si l’attribut **IsJunk** est définie sur **true** et l’attribut **MoveItem** sur **false,** l’expéditeur du message électronique cible est ajouté à la liste des expéditeurs bloqués et le message électronique n’est pas déplacé à partir du dossier.
    
- Si l’attribut **IsJunk** est définie sur **false** et que l’attribut **MoveItem** est définie sur **true,** l’expéditeur du message électronique cible est supprimé de la liste des expéditeurs bloqués et le message électronique est déplacé vers le dossier Boîte de réception.
    
- Si l’attribut **IsJunk** est définie sur **false** et que l’attribut **MoveItem** est définie sur **false,** l’expéditeur du message électronique cible est supprimé de la liste des expéditeurs bloqués et le message électronique n’est pas déplacé du dossier.
    
> [!IMPORTANT]
> Le contenu de la liste des expéditeurs bloqués n’est pas découvrable à partir d’EWS. Si un expéditeur est ajouté à la liste des expéditeurs bloqués, vous devez conserver une copie d’un message électronique envoyé par l’expéditeur bloqué pour débloquer l’expéditeur à l’avenir. 
  
### <a name="markasjunk-operation-soap-headers"></a>En-têtes SOAP d’opération MarkAsJunk

**L’opération MarkAsJunk** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur dont l’application cliente usurpe l’identité. Cet en-tête s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, telle que définie dans la RFC 3066, « Balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a>Exemple de demande d’opération MarkAsJunk : ajouter un expéditeur à la liste des expéditeurs bloqués

L’exemple suivant d’une demande d’opération **MarkAsJunk** montre comment ajouter l’expéditeur d’un message électronique à la liste des expéditeurs bloqués et déplacer le courrier vers le dossier de courrier indésirable. **L’opération MarkAsJunk** accepte l’identificateur de message électronique unique pour identifier le courrier électronique utilisé pour référencer l’expéditeur ajouté à la liste des expéditeurs bloqués. 
  
> [!NOTE]
> Tous les identificateurs d’élément et les touches de modification de cet article ont été raccourcis pour préserver la lisibilité. 
  
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
        <m:MarkAsJunk IsJunk="true" MoveItem="true">
            <m:ItemIds>
                <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYA" />
            </m:ItemIds>
        </m:MarkAsJunk>
    </soap:Body>
</soap:Envelope>

```

Le corps SOAP de la requête contient les éléments suivants :
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a>Réponse de l’opération MarkAsJunk réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **MarkAsJunk** pour ajouter un expéditeur à la liste des expéditeurs bloqués et déplacer le message électronique vers le dossier Courrier indésirable. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                             MinorVersion="0" 
                             MajorBuildNumber="545" 
                             MinorBuildNumber="11" 
                             Version="Exchange2013" 
                             xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                             xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
        <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Le corps SOAP de la réponse contient les éléments suivants :
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [MovedItemId](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a>Exemple de demande d’opération MarkAsJunk : supprimer un expéditeur de la liste des expéditeurs bloqués

L’exemple suivant d’une demande d’opération **MarkAsJunk** montre comment supprimer l’expéditeur d’un message électronique de la liste des expéditeurs bloqués et déplacer le message électronique vers le dossier Boîte de réception. Vous devez conserver un message électronique envoyé par l’expéditeur bloqué pour supprimer l’expéditeur de la liste des expéditeurs bloqués. L’adresse e-mail de l’expéditeur est associée aux messages électroniques envoyés par l’expéditeur. La suppression d’un expéditeur de la liste des expéditeurs bloqués ne réussira pas si le message électronique de référence n’existe plus dans la boîte aux lettres de l’utilisateur. L’identificateur d’élément utilisé pour associer un message électronique à son expéditeur doit être associé à un élément qui existe dans la boîte aux lettres Exchange’utilisateur. Nous vous recommandons de créer un dossier masqué pour stocker les éléments envoyés par des expéditeurs précédemment bloqués afin que les expéditeurs soient débloqués à partir de l’application cliente. Dans le cas où un élément a été supprimé de la boîte aux lettres Exchange, un administrateur doit utiliser le console de gestion Exchange pour accéder à la liste des expéditeurs bloqués afin de supprimer un expéditeur de la liste. Pour plus d’informations sur le déblocage d’un utilisateur à l’aide du console de gestion Exchange, voir Comment configurer les paramètres des expéditeurs sûrs et [bloqués](https://support.microsoft.com/kb/2545137)dans Office 365 .
  
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
      <m:MarkAsJunk IsJunk="false" MoveItem="true">
        <m:ItemIds>
          <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
        </m:ItemIds>
      </m:MarkAsJunk>
    </soap:Body>
 </soap:Envelope>

```

Une réponse réussie pour supprimer un expéditeur de la liste des expéditeurs bloqués est identique à la réponse d’ajout d’un expéditeur à la liste des expéditeurs bloqués.
  
Le corps SOAP de la requête contient les éléments suivants :
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a>Réponse d’erreur d’opération MarkAsJunk

L’exemple suivant montre une réponse d’erreur à une **demande d’opération MarkAsJunk.** Il s’agit d’une réponse à une demande d’ajout ou de suppression d’un expéditeur de la liste des expéditeurs bloqués lorsque le message électronique spécifié par l’identificateur d’élément n’existe plus dans la boîte aux lettres. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="545" 
                         MinorBuildNumber="11" 
                         Version="Exchange2013" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Le corps SOAP de réponse d’erreur contient les éléments suivants :
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération GetItem](getitem-operation.md) Opération GetItem 
    
- [Opération FindItem](finditem-operation.md)
    

