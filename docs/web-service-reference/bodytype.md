---
title: BodyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BodyType
api_type:
- schema
ms.assetid: d42ec77b-fb9f-404a-9bf2-1801e8744676
description: L’élément BodyType identifie la mise en forme le corps du texte dans la réponse.
ms.openlocfilehash: f8be2e96390b40faa367cf0d34c533accc3b8afb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755421"
---
# <a name="bodytype"></a>BodyType

L’élément **BodyType** identifie la mise en forme le corps du texte dans la réponse. 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

**BodyTypeResponseType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés de l’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.  <br/><br/>Les expressions XPath pour cet élément sont les suivantes :<br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |Identifie les propriétés totale de l’article à renvoyer dans une réponse à une demande [GetAttachment](getattachment.md) .  <br/><br/>Vous trouverez ci-dessous l’expression XPath pour cet élément :<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **BodyType** . 
  
|**Valeur**|**Description**|
|:-----|:-----|
|Recommandé  <br/> |La réponse renvoie le contenu disponible plus riche du corps de texte. Cela est utile si elle est inconnue ou non le contenu est texte ou HTML.<br/><br/> Le corps retourné sera texte si le corps stocké est en texte brut. Dans le cas contraire, la réponse renverra HTML si le corps stocké est au format HTML ou RTF.<br/><br/> Il s'agit de la valeur par défaut.  <br/> |
|HTML  <br/> |La réponse renvoie un corps de l’élément au format HTML.  <br/> |
|Texte  <br/> |La réponse renvoie un corps de l’élément en tant que texte brut.  <br/> |
   
## <a name="remarks"></a>Remarques

Vous pouvez identifier le type de corps retourné dans la réponse en vérifiant l’attribut **BodyType** de l’élément [Body](body.md) . L’attribut **BodyType** identifie le corps HTML ou texte. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant d’une demande montre où un élément **BodyType** est utilisé. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

L’attribut Id a été raccourcie afin de préserver la lisibilité.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

