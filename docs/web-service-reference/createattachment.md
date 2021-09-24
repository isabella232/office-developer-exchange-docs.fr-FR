---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: L’élément CreateAttachment définit une demande de création d’une pièce jointe à un élément dans Exchange store.
ms.openlocfilehash: 6716a83b0d1ba9d7f39351da60f7009df04a3fa0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515872"
---
# <a name="createattachment"></a>CreateAttachment

**L’élément CreateAttachment** définit une demande de création d’une pièce jointe à un élément dans Exchange store. 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 **CreateAttachmentType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ParentItemId](parentitemid.md) <br/> |Identifie l’élément de Exchange parent qui contient la pièce jointe créée. [L’élément ParentItemId](parentitemid.md) doit fournir l’ID d’un élément Exchange magasin réel. Les éléments de la boutique réelle peuvent être récupérés à l’aide de [l’opération GetItem](getitem-operation.md); les pièces jointes sont récupérées à l’aide de [l’opération GetAttachment](getattachment-operation.md). Une erreur se produit si l’ID d’un fichier joint est transmis à [ParentItemId.](parentitemid.md) Si [l’élément ParentItemId](parentitemid.md) représente l’ID d’une pièce jointe d’élément existante, l’opération [CreateAttachment](createattachment-operation.md) ajoute la nouvelle pièce jointe à la pièce jointe existante.  <br/> Cet élément est requis pour [l’opération CreateAttachment](createattachment-operation.md).  <br/> |
|[Pièces jointes](attachments-ex15websvcsotherref.md) <br/> |Contient les éléments ou fichiers à joindre à un élément dans la Exchange store.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Une pièce jointe d’élément n’existe pas en tant qu’élément de magasin. Il existe uniquement en tant que pièce jointe à un élément ou une autre pièce jointe. Les pièces jointes d’élément peuvent uniquement être récupérées à l’aide de [la demande GetAttachment.](getattachment.md) 
  
Les pièces jointes d’élément suivantes peuvent être créées :
  
- Item
    
- Message
    
- CalendarItem
    
- Contact
    
- Tâche
    
- MeetingMessage
    
- MeetingRequest
    
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant montre comment créer et attacher un élément à un autre élément de la Exchange store.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="ASkAS"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>MyAttachment</t:Name>
          <t:Message>
            <t:ItemClass>IPM>Note</t:ItemClass>
            <t:Subject>My attachment subject</t:Subject>
            <t:Body BodyType="Text">My attachment body</t:Body>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CreateAttachment](createattachment-operation.md)
  
[Opération DeleteAttachment](deleteattachment-operation.md)
  
[Opération GetAttachment](getattachment-operation.md)

