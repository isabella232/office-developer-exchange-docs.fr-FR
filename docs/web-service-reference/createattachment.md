---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: L’élément CreateAttachment définit une demande pour créer une pièce jointe à un élément dans la banque d’informations Exchange.
ms.openlocfilehash: d403eb5ca15623d3a973f7b224dbcde5529cf1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755683"
---
# <a name="createattachment"></a>CreateAttachment

L’élément **CreateAttachment** définit une demande pour créer une pièce jointe à un élément dans la banque d’informations Exchange. 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 **CreateAttachmentType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ParentItemId](parentitemid.md) <br/> |Identifie l’élément de magasin Exchange parent qui contient la pièce jointe créée. L’élément [ParentItemId](parentitemid.md) doit fournir l’élément de magasin de l’ID d’un véritable Exchange. Éléments de la banque réel peuvent être récupérés à l’aide de l' [opération GetItem](getitem-operation.md); pièces jointes sont récupérées à l’aide de l' [opération GetAttachment](getattachment-operation.md). Une erreur se produit si le [ParentItemId](parentitemid.md) est transmis à l’ID d’une pièce jointe. Si le [ParentItemId](parentitemid.md) représente l’ID de pièce jointe d’élément existant, l' [opération CreateAttachment](createattachment-operation.md) ajoute la nouvelle pièce jointe à la pièce jointe existante.  <br/> Cet élément est requis pour l' [opération CreateAttachment](createattachment-operation.md).  <br/> |
|[Pièces jointes](attachments-ex15websvcsotherref.md) <br/> |Contient les éléments ou les fichiers pour attacher à un élément dans la banque d’informations Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Une pièce jointe d’élément n’existe pas comme un élément de magasin. Il existe uniquement en tant que pièce jointe à un élément ou une autre pièce jointe. Pièces jointes d’élément ne peuvent être extrait à l’aide de la demande [GetAttachment](getattachment.md) . 
  
Vous pouvez créer les pièces jointes d’éléments suivants :
  
- Élément
    
- Message
    
- CalendarItem
    
- Contact
    
- Tâche
    
- MeetingMessage
    
- MeetingRequest
    
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant montre comment créer et joindre un élément à un autre élément dans la banque d’informations Exchange.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CreateAttachment](createattachment-operation.md)
  
[Opération DeleteAttachment](deleteattachment-operation.md)
  
[Opération GetAttachment](getattachment-operation.md)

