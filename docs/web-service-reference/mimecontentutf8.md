---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: L’élément MimeContentUTF8 contient le flux MIME UTF-8 d’un objet qui est représenté dans le format base64Binary et internationalisation des adresses de messagerie prend en charge et [RFC6530].
ms.openlocfilehash: 47599b6634738fd488e5b020f69e36d5fcf550a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828466"
---
# <a name="mimecontentutf8"></a>MimeContentUTF8

L’élément **MimeContentUTF8** contient le flux MIME UTF-8 d’un objet qui est représenté dans le format base64Binary et prend en charge internationalisation des adresses de messagerie et [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).
  
```XML
<MimeContentUTF8 CharacterSet="" />
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

Une valeur de texte qui représente un flux de données MIME base64binary est obligatoire si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Le contenu du message transite par les trois niveaux de codage avant d’être stocké dans la valeur **MimeContentUTF8** suivants : 
  
1. Texte du message : il s’agit de l’organisme codage, tel qu’iso-2022-jp pour les caractères japonais.
    
2. Flux de données MIME — il s’agit de l’encodage UTF-8 du texte du message pour l’élément **MimeContentUTF8** , ou le codage ASCII du texte du message pour l’élément [MimeContent](mimecontent.md) . 
    
3. Document XML — il s’agit toujours le flux ASCII codé en base64 du flux de données MIME, où caractères tels que «\<», qui sont significatif au format XML, sont masquées à partir d’analyseurs XML.
    
Chaque niveau est indépendante du niveau qui le précède.
  
L’élément **MimeContentUTF8** peut contenir les mêmes données qui contiennent des autres propriétés qui sont renvoyées avec un élément. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
### <a name="version-differences"></a>Différences entre les versions

Cet élément est disponible dans les versions d’Exchange commençant par build 15.00.0986.00.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

