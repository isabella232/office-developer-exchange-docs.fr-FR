---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: L’élément MimeContent contient le flux MIME ASCII d’un objet qui est représenté dans le format base64Binary et prend en charge [RFC2045].
ms.openlocfilehash: 60f2d42f09347611559137c494d93036f1192829
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828465"
---
# <a name="mimecontent"></a>MimeContent

L’élément **MimeContent** contient le flux MIME ASCII d’un objet qui est représenté dans le format base64Binary et prend en charge [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).
  
```xml
<MimeContent CharacterSet="" />
```

 **MimeContentType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Jeu de caractères** <br/> |Si la valeur, la valeur de cet attribut est ignorée par le serveur.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [élément](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [ MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [tâche](task.md)
  
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente un flux de données MIME base64Binary est obligatoire si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Le contenu du message transite par les trois niveaux de codage avant d’être stocké dans la valeur **MimeContent** suivants : 
  
1. Texte du message : il s’agit de l’organisme codage, tel qu’iso-2022-jp pour les caractères japonais.
    
2. Flux de données MIME — il s’agit de l’encodage ASCII du texte du message pour l’élément **MimeContent** , ou le codage UTF-8 du texte du message pour l’élément [MimeContentUTF8](mimecontentutf8.md) . 
    
3. Document XML — il s’agit toujours le flux ASCII codé en base64 du flux de données MIME, où caractères tels que «\<», qui sont significatif au format XML, sont masquées à partir d’analyseurs XML.
    
Chaque niveau est indépendante du niveau qui le précède.
  
L’élément **MimeContent** peut contenir les mêmes données qui contiennent des autres propriétés qui sont renvoyées avec un élément. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

