---
title: Opération DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 3e26c416-fa12-476e-bfd2-5c1f4bb7b348
description: L’opération DeleteItem supprime les éléments de la Exchange store.
ms.openlocfilehash: b62655b9046678d27ed0f24bc92d1840f3e3b343
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545411"
---
# <a name="deleteitem-operation"></a>Opération DeleteItem

**L’opération DeleteItem** supprime les éléments de la Exchange store. 
  
> [!NOTE]
> Une réponse d’erreur qui inclut le code d’erreur ErrorCannotDeleteObject est renvoyée pour une opération **DeleteItem** lorsqu’un délégué tente de supprimer un élément dans la boîte aux lettres du principal en délégant le paramètre DisposalType sur MoveToDeletedItems. Pour supprimer un élément en le déplaçant vers le dossier Éléments supprimés, un délégué doit utiliser [l’opération MoveItem](moveitem-operation.md). 
  
## <a name="deleteitem-request-example"></a>Exemple de requête DeleteItem

### <a name="description"></a>Description

L’exemple suivant **d’une demande DeleteItem** montre comment effectuer une suppression d’un élément d’une boîte aux lettres. 
  
> [!NOTE]
> L’ID d’élément a été raccourci pour préserver la lisibilité. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteItem DeleteType="HardDelete" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemIds>
        <t:ItemId Id="AS4AUn=="/>
      </ItemIds>
    </DeleteItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [DeleteItem](deleteitem.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
Pour rechercher d’autres options pour le message de demande de **l’opération DeleteItem,** explorez la hiérarchie de schéma. Commencez à [l’élément DeleteItem.](deleteitem.md) 
  
## <a name="successful-deleteitem-response"></a>Réponse DeleteItem réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à **la demande DeleteItem.** 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteItemResponse](deleteitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteItemResponseMessage](deleteitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
Pour rechercher d’autres options pour le message de réponse de **l’opération DeleteItem,** explorez la hiérarchie de schéma. Commencez par [l’élément DeleteItemResponse.](deleteitemresponse.md) 
  
## <a name="deleteitem-error-response"></a>Réponse d’erreur DeleteItem

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à **une demande DeleteItem.** L’erreur a été créée car l’opération a tenté de supprimer un élément qui n’a pas été trouvé dans Exchange store. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteItemResponse](deleteitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteItemResponseMessage](deleteitemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour rechercher d’autres options pour le message de réponse d’erreur de **l’opération DeleteItem,** explorez la hiérarchie du schéma. Commencez par [l’élément DeleteItemResponse.](deleteitemresponse.md) 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Deleting Contacts](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)  
- [Suppression de messages électroniques](https://msdn.microsoft.com/library/c40f2f0b-dae0-412f-b716-727e8c0949b4%28Office.15%29.aspx) 
- [Suppression de tâches](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

