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
description: L’élément BodyType identifie la façon dont le corps de texte est mis en forme dans la réponse.
ms.openlocfilehash: 448d20ac54b09a2f4f6a273a1099519371ac7f5b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465946"
---
# <a name="bodytype"></a>BodyType

L’élément **BodyType** identifie la façon dont le corps de texte est mis en forme dans la réponse. 
  
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
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés d’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.  <br/><br/>Voici les expressions XPath de cet élément :<br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |Identifie les propriétés d’élément étendue supplémentaires à renvoyer dans une réponse à une demande [GetAttachment](getattachment.md) .  <br/><br/>Voici l’expression XPath de cet élément :<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **BodyType** . 
  
|**Valeur**|**Description**|
|:-----|:-----|
|Idéale  <br/> |La réponse renverra le contenu disponible le plus riche du corps de texte. Ceci est utile s’il n’est pas connu si le contenu est du texte ou du code HTML.<br/><br/> Le corps renvoyé sera du texte si le corps stocké est en texte brut. Dans le cas contraire, la réponse renvoie HTML si le corps stocké est au format HTML ou RTF.<br/><br/> Il s’agit de la valeur par défaut.  <br/> |
|HTML  <br/> |La réponse renvoie un corps d’élément au format HTML.  <br/> |
|Texte  <br/> |La réponse renvoie un corps d’élément sous forme de texte brut.  <br/> |
   
## <a name="remarks"></a>Remarques

Vous pouvez identifier le type de corps renvoyé dans la réponse en vérifiant l’attribut **BodyType** de l’élément [Body](body.md) . L’attribut **BodyType** identifie le corps au format HTML ou texte. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant d’une requête indique où un élément **BodyType** est utilisé. 
  
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

L’attribut ID a été raccourci pour conserver la lisibilité.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

