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
description: L’élément CreateAttachment définit une demande de création d’une pièce jointe à un élément dans la Banque d’Exchange.
ms.openlocfilehash: 4cba1b8865dae5da58b9617b249a29314c67331a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466436"
---
# <a name="createattachment"></a>CreateAttachment

L’élément **CreateAttachment** définit une demande de création d’une pièce jointe à un élément dans la Banque d’Exchange. 
  
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
|[ParentItemId](parentitemid.md) <br/> |Identifie l’élément de la banque Exchange parente qui contient la pièce jointe créée. L’élément [parentItemId](parentitemid.md) doit fournir l’ID d’un élément réel de la Banque d’identités Exchange. Les éléments de magasin réel peuvent être récupérés à l’aide de l' [opération GetItem](getitem-operation.md); les pièces jointes sont récupérées à l’aide de l' [opération GetAttachment](getattachment-operation.md). Une erreur se produit si l’ID d’une pièce jointe est transmis à [parentItemId](parentitemid.md) . Si le [parentItemId](parentitemid.md) représente l’ID d’une pièce jointe d’un élément existant, l' [opération CreateAttachment](createattachment-operation.md) ajoute la nouvelle pièce jointe à la pièce jointe existante.  <br/> Cet élément est requis pour l' [opération CreateAttachment](createattachment-operation.md).  <br/> |
|[Attachments](attachments-ex15websvcsotherref.md) <br/> |Contient les éléments ou les fichiers à joindre à un élément dans la Banque d’Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Une pièce jointe d’élément n’existe pas en tant qu’élément de la boutique. Il existe uniquement en tant que pièce jointe à un élément ou à une autre pièce jointe. Les pièces jointes d’éléments ne peuvent être récupérées qu’à l’aide de la demande [GetAttachment](getattachment.md) . 
  
Les pièces jointes d’éléments suivantes peuvent être créées :
  
- Option
    
- Message
    
- CalendarItem
    
- Contact
    
- Tâche
    
- MeetingMessage
    
- Propriété meetingrequest
    
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant montre comment créer et attacher un élément à un autre élément dans la Banque d’informations Exchange.
  
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
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CreateAttachment](createattachment-operation.md)
  
[Opération DeleteAttachment](deleteattachment-operation.md)
  
[Opération GetAttachment](getattachment-operation.md)

