---
title: BodyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- BodyType
api_type:
- schema
ms.assetid: d42ec77b-fb9f-404a-9bf2-1801e8744676
description: L’élément BodyType identifie la façon dont le corps de texte est formaté dans la réponse.
ms.openlocfilehash: e8952ac2774589e031280ce982ea8671b736a87d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526840"
---
# <a name="bodytype"></a>BodyType

**L’élément BodyType** identifie la façon dont le corps de texte est formaté dans la réponse. 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

**BodyTypeResponseType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés et le contenu de l’élément à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.  <br/><br/>Les expressions XPath de cet élément sont les suivantes :<br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |Identifie d’autres propriétés d’élément étendu à renvoyer dans une réponse à [une demande GetAttachment.](getattachment.md)  <br/><br/>Voici l’expression XPath de cet élément :<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour **l’élément BodyType.** 
  
|**Valeur**|**Description**|
|:-----|:-----|
|Idéale  <br/> |La réponse retourne le contenu disponible le plus riche du corps de texte. Cela est utile s’il est inconnu si le contenu est du texte ou du code HTML.<br/><br/> Le corps renvoyé sera du texte si le corps stocké est en texte simple. Sinon, la réponse retourne du code HTML si le corps stocké est au format HTML ou RTF.<br/><br/> Il s’agit de la valeur par défaut.  <br/> |
|HTML  <br/> |La réponse retourne un corps d’élément au format HTML.  <br/> |
|Texte  <br/> |La réponse retourne un corps d’élément sous forme de texte simple.  <br/> |
   
## <a name="remarks"></a>Remarques

Vous pouvez identifier le type de corps renvoyé dans la réponse en vérifiant l’attribut **BodyType** de [l’élément Body.](body.md) **L’attribut BodyType** identifie le corps au format HTML ou texte. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant d’une requête indique l’endroit où un **élément BodyType** est utilisé. 
  
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
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

L’attribut ID a été raccourci pour préserver la lisibilité.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

