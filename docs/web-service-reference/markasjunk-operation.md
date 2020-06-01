---
title: Opération MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Trouvez des informations sur l’opération EWS MarkAsJunk.
ms.openlocfilehash: 25d6b01dfff64c4e45f3382223311219d349c165
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468571"
---
# <a name="markasjunk-operation"></a>Opération MarkAsJunk

Trouvez des informations sur l’opération EWS **MarkAsJunk** . 
  
L’opération **MarkAsJunk** ajoute et supprime des utilisateurs de la liste de courriers bloqués et déplace les messages électroniques vers le dossier courrier indésirable. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-markasjunk-operation"></a>Utilisation de l’opération MarkAsJunk

L’opération **MarkAsJunk** contient deux options booléennes pour indiquer si un expéditeur de courrier électronique doit être ajouté à la liste des expéditeurs bloqués et si le message électronique cible doit être déplacé vers le dossier courrier indésirable par défaut ou le dossier boîte de réception. Les actions sont déterminées par les valeurs des attributs **IsJunk** et **MoveItem** . Voici les actions possibles basées sur les combinaisons de valeur pour les attributs **IsJunk** et **MoveItem** : 
  
- Si l’attribut **IsJunk** est défini sur **true**et si l’attribut **MoveItem** est défini sur **true**, l’expéditeur du message électronique cible est ajouté à la liste des expéditeurs bloqués et le message électronique est déplacé dans le dossier courrier indésirable.
    
- Si l’attribut **IsJunk** est défini sur **true**et si l’attribut **MoveItem** est défini sur **false**, l’expéditeur du message électronique cible est ajouté à la liste des expéditeurs bloqués et le message électronique n’est pas déplacé du dossier.
    
- Si l’attribut **IsJunk** est défini sur **false**et que l’attribut **MoveItem** est défini sur **true**, l’expéditeur du message électronique cible est supprimé de la liste des expéditeurs bloqués et le message électronique est déplacé vers le dossier boîte de réception.
    
- Si l’attribut **IsJunk** est défini sur **false**et que l’attribut **MoveItem** est défini sur **false**, l’expéditeur du message électronique cible est supprimé de la liste des expéditeurs bloqués et le message électronique n’est pas déplacé du dossier.
    
> [!IMPORTANT]
> Le contenu de la liste des expéditeurs bloqués ne peut pas être découvert depuis EWS. Si un expéditeur est ajouté à la liste des expéditeurs bloqués, vous devez conserver une copie d’un message électronique envoyé par l’expéditeur bloqué pour débloquer l’expéditeur à l’avenir. 
  
### <a name="markasjunk-operation-soap-headers"></a>En-têtes SOAP d’opération MarkAsJunk

L’opération **MarkAsJunk** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur qui emprunte l’identité de l’application cliente. Cet en-tête s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a>Exemple de requête d’opération MarkAsJunk : ajouter un expéditeur à la liste des expéditeurs bloqués

L’exemple suivant de demande d’opération **MarkAsJunk** indique comment ajouter l’expéditeur d’un message électronique à la liste des expéditeurs bloqués et déplacer le courrier électronique vers le dossier courrier indésirable. L’opération **MarkAsJunk** accepte l’identificateur unique de message électronique pour identifier le courrier électronique utilisé pour référencer l’expéditeur qui est ajouté à la liste des expéditeurs bloqués. 
  
> [!NOTE]
> Tous les identificateurs d’élément et clés de modification de cet article ont été raccourcies afin de préserver la lisibilité. 
  
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

Le corps SOAP de la demande contient les éléments suivants :
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a>Réponse de l’opération MarkAsJunk réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **MarkAsJunk** pour ajouter un expéditeur à la liste des expéditeurs bloqués et déplacer le message électronique dans le dossier courrier indésirable. 
  
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

Le corps SOAP de réponse contient les éléments suivants :
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [MovedItemId](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a>Exemple de requête d’opération MarkAsJunk : supprimer un expéditeur de la liste des expéditeurs bloqués

L’exemple suivant de demande d’opération **MarkAsJunk** montre comment supprimer l’expéditeur d’un message électronique de la liste des expéditeurs bloqués et déplacer le message électronique dans le dossier boîte de réception. Vous devez conserver un message électronique envoyé par l’expéditeur bloqué pour supprimer l’expéditeur de la liste des expéditeurs bloqués. L’adresse de messagerie de l’expéditeur est associée aux messages électroniques envoyés par l’expéditeur. La suppression d’un expéditeur de la liste des expéditeurs bloqués échoue si le message électronique de référence n’existe plus dans la boîte aux lettres de l’utilisateur. L’identificateur d’élément utilisé pour associer un message électronique à son expéditeur doit être associé à un élément qui existe dans la boîte aux lettres Exchange. Nous vous recommandons de créer un dossier masqué pour stocker les éléments envoyés par des expéditeurs précédemment bloqués de sorte que les expéditeurs puissent être débloqués de l’application cliente. Si un élément a été supprimé de la boîte aux lettres Exchange, un administrateur doit utiliser la console de gestion Exchange pour accéder à la liste des expéditeurs bloqués afin de supprimer un expéditeur de la liste. Pour plus d’informations sur le déblocage d’un utilisateur à l’aide de la console de gestion Exchange, consultez la rubrique relative à la configuration des paramètres des expéditeurs [approuvés et des expéditeurs bloqués dans Office 365](https://support.microsoft.com/kb/2545137).
  
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

Une réponse efficace lors de la suppression d’un expéditeur de la liste des expéditeurs bloqués est la même que la réponse à l’ajout d’un expéditeur à la liste des expéditeurs bloqués.
  
Le corps SOAP de la demande contient les éléments suivants :
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a>Réponse d’erreur d’opération MarkAsJunk

L’exemple suivant montre une réponse d’erreur à une demande d’opération **MarkAsJunk** . Réponse à une demande d’ajout ou de suppression d’un expéditeur de la liste des expéditeurs bloqués lorsque le message électronique spécifié par l’identificateur d’élément n’existe plus dans la boîte aux lettres. 
  
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

Le corps SOAP de la réponse d’erreur contient les éléments suivants :
  
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
    

