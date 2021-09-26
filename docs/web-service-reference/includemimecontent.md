---
title: IncludeMimeContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IncludeMimeContent
api_type:
- schema
ms.assetid: 3f3c2300-55cd-41c0-900e-b470b290d52f
description: L’élément IncludeMimeContent spécifie si le contenu MIME (Multipurpose Internet Mail Extensions) d’un élément ou d’une pièce jointe est renvoyé dans la réponse.
ms.openlocfilehash: 04d015ea450907f3968200dcbb6f411eb6343681
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542175"
---
# <a name="includemimecontent"></a>IncludeMimeContent

**L’élément IncludeMimeContent** spécifie si le contenu MIME (Multipurpose Internet Mail Extensions) d’un élément ou d’une pièce jointe est renvoyé dans la réponse. 
  
```xml
<IncludeMimeContent>true or false</IncludeMimeContent>
```

 **boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> | Identifie les propriétés supplémentaires à renvoyer en réponse à une [demande GetAttachment.](getattachment.md)  <br/> <br/> Voici l’expression XPath de cet élément :  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés et le contenu de l’élément à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.  <br/> <br/> Les expressions XPath de cet élément sont les suivantes :<br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valeur texte

Cet élément peut être **vrai** ou **faux**. La valeur par défaut est **false**. Il s’agit d’un type de données booléen.
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant d’une requête montre comment définir **l’élément IncludeMimeContent.** 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

L’attribut id de pièce jointe est tronqué pour préserver la lisibilité.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

