---
title: IncludeMimeContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludeMimeContent
api_type:
- schema
ms.assetid: 3f3c2300-55cd-41c0-900e-b470b290d52f
description: L’élément IncludeMimeContent Spécifie si le contenu Multipurpose Internet Mail Extensions (MIME) d’un élément ou d’une pièce jointe est retourné dans la réponse.
ms.openlocfilehash: ddd6988be93231ac7c574a2e19c9ba4b562c7d0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827903"
---
# <a name="includemimecontent"></a>IncludeMimeContent

L’élément **IncludeMimeContent** Spécifie si le contenu Multipurpose Internet Mail Extensions (MIME) d’un élément ou d’une pièce jointe est retourné dans la réponse. 
  
```xml
<IncludeMimeContent>true or false</IncludeMimeContent>
```

 **boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> | Identifie les propriétés supplémentaires pour retourner une réponse à une demande [GetAttachment](getattachment.md) .  <br/> <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés de l’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.  <br/> <br/> Les expressions XPath pour cet élément sont les suivantes :<br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Cet élément peut être **true** ou **false**. La valeur par défaut est **false**. Il s’agit d’un type de données Boolean.
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

Une demande de l’exemple suivant montre une procédure pour définir l’élément **IncludeMimeContent** . 
  
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

L’attribut Id de pièce jointe est tronqué afin de préserver la lisibilité.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

